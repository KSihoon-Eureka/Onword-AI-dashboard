# Implementation Spec — MVP UDS ERP/Dashboard Ingestion

## Scope

This MVP is an order/product/ERP dashboard schema, not a full ERP. It normalizes the five already-extracted channels only: Coupang, Cafe24, Naver Smart Store, Gmarket/Auction, and SSG Mall. Future channels are researched separately and must not be inserted into the MVP mapping until their dictionaries are extracted.

## Relational model

Recommended application tables:

1. `orders` — one row per channel order/payment container.
2. `order_items` — one row per purchased product line. This is the primary dashboard grain for sales, fulfillment, margin, claims, and reconciliation.
3. `shipments` — one row per channel shipment/box/invoice group.
4. `claims` — one row per cancellation/return/exchange/refund claim.
5. `products` — one row per channel product/SKU snapshot, linkable to an internal product master later.
6. `inventory_snapshots` — append-only observed inventory by channel product/option and timestamp.
7. `settlements` — settlement/payable rows by channel order/item/date when available.
8. `customers_receivers` — buyer/receiver PII isolated from operational facts.
9. `cs_threads` and later `cs_messages` — product Q&A, inquiries, notes, and replies.

Raw/ops tables:

- `raw_channel_payloads(id, channel, endpoint, request_params, payload_json, payload_hash, fetched_at, source_file_path)`
- `channel_sync_state(channel, connector_name, cursor_type, cursor_value, last_success_at, last_error_at, status)`
- `order_item_change_events(id, channel, channel_order_item_key, previous_hash, new_hash, changed_columns, changed_at)`

## Primary keys and stable channel keys

Use internal UUID primary keys plus deterministic channel keys.

- Coupang order-item key: `COUPANG:{shipmentBoxId}:{orderId}:{vendorItemId}` where present. If shipment box is absent for pre-shipment rows, temporarily use `COUPANG:{orderId}:{vendorItemId}` and re-key through an alias table when shipment box arrives.
- Naver Smart Store order-item key: `NAVER:{productOrderId}`. Naver's product order is the natural core unit.
- Cafe24 order-item key: `CAFE24:{mall_id}:{shop_no}:{order_id}:{order_item_code}`.
- Gmarket/Auction order-item key: `ESM:{siteType}:{orderNo_or_packNo}:{orderDetailNo_or_skuId_or_itemNo}`. Confirm exact detail identifier during connector implementation because ESM endpoints vary by order/claim/shipping API.
- SSG order-item key: `SSG:{orOrdNo}:{ordItemSeq_or_ordItemId}:{shppNo_or_boxNo}` when shipping IDs are available; otherwise omit the shipment segment and keep a key-alias table.

## Upsert rules

1. Store raw response/file first in `raw_channel_payloads` before normalization.
2. Normalize to order-item grain.
3. Build deterministic key and `row_hash` from business fields excluding `last_seen_at`, ingest timestamp, and raw payload ID.
4. If key does not exist: insert facts and `first_seen_at = last_seen_at = now()`.
5. If key exists and hash is unchanged: update `last_seen_at` only.
6. If key exists and hash changed: update current row, insert `order_item_change_events`, and keep previous raw payload reference.
7. Never hard-delete disappeared rows. Mark stale/missing through reconciliation status.

## Normalization rules

- Amounts: store numeric in KRW unless source explicitly provides another currency; preserve source currency in `currency_code`.
- Datetimes: parse source timezone and store UTC plus a KST presentation layer. If the source only gives a date, store date in date columns or midnight KST with a precision flag later.
- Statuses: keep raw status code/name in mapped columns for MVP; add normalized enums (`order_lifecycle_status`, `claim_lifecycle_status`) in phase 2.
- PII: isolate buyer/receiver fields in `customers_receivers`; apply masking/encryption policy before BI export.
- Products: do not treat channel product IDs as internal master IDs. Use `product_id` as an internal future master key and maintain channel product mappings.
- Inventory: use append-only snapshots first. Move to `inventory_events` only after channels provide reliable transaction-level stock deltas.
- CS: use `cs_threads` for MVP; split `cs_messages` when channel APIs expose multi-message thread history.

## Dashboard-oriented MVP metrics

- 주문/매출: paid amount, item amount, discount amount, quantity by day/channel/product.
- 처리 필요: unconfirmed orders, unshipped orders, delayed shipments, missing invoices.
- 클레임: claim count, claim amount, claim reason, return/exchange/cancel queue.
- 재고: low stock by channel SKU, zero-stock risks, products with sales but no inventory snapshot.
- 정산: gross/net settlement, fees, settlement exceptions.
- CS: unanswered inquiries and aged CS threads.

## Implementation sequence

1. Create database tables from `uds_core_schema.json` plus raw/ops tables.
2. Implement local CSV dictionary-backed mapping validation tests.
3. Build connectors in this order: Naver Smart Store, Cafe24, Coupang, then Gmarket/Auction and SSG.
4. Backfill 30–90 days order-item history where API limits allow.
5. Run every-5-minute incremental sync for API channels; nightly 7-day reconciliation.
6. Add future channels only after their API/raw dictionaries are extracted and reviewed.
