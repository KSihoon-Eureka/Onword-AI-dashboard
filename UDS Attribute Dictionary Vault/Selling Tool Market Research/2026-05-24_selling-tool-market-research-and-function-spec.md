---
title: Selling Tool Market Research — Multichannel Ecommerce Operations Platforms
created: 2026-05-24
status: draft-v1
category: market-research
scope: Korean and global selling tools / OMS / ecommerce ERP
---

# Selling Tool Market Research — Multichannel Ecommerce Operations Platforms

## 0. Executive Summary

**Definition:** A selling tool company is not just a dashboard company. In Korea, the mature pattern is an **OMS + product/listing manager + inventory/WMS + shipping/invoice + CS/claim + settlement/reporting + automation** platform that connects many marketplaces and lets sellers operate from one place.

The Korean market already has strong incumbents:

- **사방넷 / Sabangnet** — broadest visible Korean channel coverage; OMS + WMS + CS + AI add-ons.
- **플레이오토 / PlayAuto** — broad multichannel + overseas + API/developer positioning under ConnectWave.
- **샵링커 / Shoplinker** — low-cost entry + product/order/CS/claims/API + AI add-ons.
- **셀메이트 / Sellmate** — warehouse/barcode/picking/CS-heavy operations for high-SKU sellers.
- **셀피아 / Sellpia** — low-cost online/offline inventory and order integration under ConnectWave.
- **이지어드민 / EasyAdmin** — WMS/logistics/CS/enterprise customization-heavy.
- **Cafe24 Market Plus**, **Naver SmartStore Center**, **Coupang Wing**, **ESM PLUS** — native/channel-specific tools, not full cross-channel selling tools.

Global platforms show the mature end-state:

- **Rithum/ChannelAdvisor, Linnworks, Sellercloud, Zentail, Sellbrite, Shopify Marketplace Connect, ShipStation, Extensiv, Cin7, Brightpearl, NetSuite**.
- Mature systems converge on the same modules: catalog/listing, order, inventory, fulfillment, shipping, claims/returns, CS, settlement/accounting, analytics, automation/rules, API.

**Strategic conclusion for Onword:** Competing head-on as “another OMS with 600 integrations” is a bad first wedge. The best wedge is an **AI-native selling operations command center** that:

1. Ingests orders/products/inventory/claims/settlements/CS from marketplaces and/or existing OMS tools.
2. Normalizes data into UDS.
3. Shows manager-facing exception dashboards.
4. Recommends and eventually executes actions: fix listing, reorder stock, respond to CS, resolve claim, sync invoice/tracking, investigate settlement mismatch, pause channel inventory, etc.

The product should be **workflow-first, not chart-first**. Store managers need to know **what needs action now**, not just “sales were up 12%.”

---

## 1. Market Map: Korean Selling Tools

### 1.1 Korean Competitor Matrix

| Tool | Operator / Entity | Core Positioning | Key Functions | Channel / Integration Coverage | Pricing Signal | Strategic Read |
|---|---|---|---|---|---|---|
| **Sabangnet / 사방넷** | Daou Tech / 다우기술 | Broad Korean multichannel OMS + WMS | Product registration/edit, order collection, CS/inquiry/claim collection, invoice printing/transmission, WMS, returns, inventory, image hosting, scheduler, API, AlimTalk, chatbot, AI recommendations | Public support page showed ~687 total malls; open market, social, general mall, specialty mall, home shopping, welfare mall, overseas | Plans visible from ~150k KRW/mo + setup fees; add-ons for scheduler/API/AlimTalk/chatbot | Strong incumbent. Channel breadth + Daou trust = moat. Weakness: legacy complexity, AI as add-on not core OS. |
| **PlayAuto / 플레이오토 / PLTO** | ConnectWave / 커넥트웨이브 | Multichannel domestic/overseas selling automation | Product registration, transfer, order collection, invoice transmission, inquiry, settlement collection, API/dev center, scheduler, mobile, AI product-name optimization | Support table had ~308 rows; broad domestic + overseas channels including SmartStore, Coupang, 11st, Gmarket/Auction, GS, LotteON, CJ, SSG, Cafe24, Kurly, Temu, AliExpress | Standard/Growth pricing roughly 128k–299k KRW/mo depending plan/discount/setup | Strong competitor for marketplace sellers; better API/global positioning than many Korean tools. |
| **Shoplinker / 샵링커** | Shoplinker G&C | Low-to-mid cost product/order/CS integration | Product, order, CS/claims, API, inventory, gifts, migration, AlimTalk, scheduling, invoice, custom dev, AI product registration/insight/review | Support table ~166 rows; major Korean/open/social/global channels | Free/Beginner low-cost tiers; automation/API add-ons; API integration can be expensive | Good low-cost wedge; AI add-ons exist; limits/add-ons can fragment value. |
| **Sellmate / 셀메이트** | Sellmate Inc. | Warehouse/high-SKU operation system | Sales-channel order management, barcode inventory, CS, purchase/vendor ordering, auto order bot, same-day outbound, picking, WMS, POS, mobile logistics, API, RFID, inventory sync | Public channel count less transparent; plans include many seller-channel registrations | ~300k–600k KRW/mo + setup; API/mobile/market inventory sync add-ons | Strong for apparel/high-SKU warehouse workflows. Less transparent channel coverage; not primarily executive analytics. |
| **Sellpia / 셀피아** | ConnectWave | Low-cost online/offline inventory + order tool | Online/offline inventory, marketplace product registration, order auto-collection, invoice/return integration, picking routes, low-stock alerts, barcode inventory, PO, CS, stats | Sales page ~155 integration rows; includes SmartStore, Coupang, 11st, Auction, Gmarket, AliExpress, GS, LotteON, CJ, SSG, Kurly, Kakao Gift, Zigzag/Ably/Queenit, Cafe24 | Free tier, then 50k/100k/200k KRW/mo | Very price competitive; good for SME wedge. May have less enterprise depth than Sabangnet/PlayAuto/EasyAdmin. |
| **EasyAdmin / 이지어드민** | PIMZ / 핌즈 | WMS/logistics/CS-heavy OMS | Order collection, inventory, delivery, CS, enterprise customization, WMS, online/offline inventory+CRM, API, inventory sync, AlimTalk, multi-location, mobile warehouse, returns, tracking | Integration table ~113 rows; includes major malls | Pricing not clearly public | Deep operations/WMS. Less transparent/modern; likely enterprise/ops-heavy. |
| **Cafe24 Market Plus** | Cafe24 | Cafe24-native multi-market integration | Manage external marketplaces from Cafe24 self-mall context: products/orders across Naver/Coupang/Gmarket/11st etc. | Multi-market, exact count unclear from accessible pages | Bundled/add-on style | Strong if merchant is Cafe24-first; not enough as broad independent OMS. |
| **ESM PLUS** | Gmarket/Auction native | Native seller center for Gmarket/Auction | Deep native Gmarket/Auction product/order/settlement ops | Gmarket + Auction only | Free seller tool, fees separate | Required native source but not cross-channel. |
| **Naver SmartStore Center** | Naver | Native seller center for Naver SmartStore | Naver Pay, TalkTalk, SmartStore product/order/customer ops, education | Naver ecosystem only | Free seller tool, fees separate | Deep single-channel; no cross-channel UDS. |
| **Coupang Wing / Marketplace** | Coupang | Native Coupang seller center | Coupang product/order/shipping/settlement ops | Coupang only | Free seller tool, commission/logistics fees separate | Necessary for Coupang-specific operations; no cross-channel layer. |

### 1.2 What Korean Tools Actually Sell

The Korean category is not “dashboard SaaS.” It is closer to:

```text
Marketplace integration + product registration + order collection + invoice/tracking + inventory + claims/CS + WMS + reporting + automation/add-ons
```

Common visible monetization levers:

- monthly order count
- product DB/SKU count
- connected mall/channel IDs
- user IDs
- setup fee
- scheduler/automation add-on
- API add-on
- mobile/WMS add-on
- AlimTalk/message cost
- custom development/integration fee

### 1.3 Korean Market Gap

Most incumbents are **operations table systems**. They help sellers do work, but they rarely feel like an AI-native command center that tells the manager:

- “These 14 orders will miss SLA unless shipped by 4 PM.”
- “SKU X will stock out in 2.3 days; Coupang sales velocity is up 38%.”
- “Gmarket settlement for order group Y is 37,200 KRW lower than expected.”
- “Return reason spike is concentrated in product option Z.”
- “CS tickets about 냄새/포장불량 are rising for supplier batch B.”
- “Naver listing is missing attribute A; Coupang listing image rejected; SSG stock sync failed.”

That is the wedge.

---

## 2. Global Benchmark Platforms

| Platform | Core Modules | What Onword Should Learn |
|---|---|---|
| **Rithum / ChannelAdvisor** | Marketplace listings, inventory, order management, commerce insights/reporting | “Control tower” model: marketplace listing health + inventory + order visibility + profitability. |
| **Linnworks** | Order, inventory, warehouse, listings, shipping, forecasting, reporting, automation | Structure product by operational workflow: Listing → Inventory → Order → Fulfillment → Shipping → Reporting → Automation. |
| **Sellbrite** | Listing, inventory sync, shipping, FBA/multi-warehouse, API | SMB promise: list everywhere, sync inventory, ship orders, prevent overselling. |
| **Sellercloud** | Catalog, inventory, WMS, order, rule engine, purchasing, shipping, reporting, accounting, API | Full ecommerce ERP module map. Rule engine is core, not optional. |
| **Zentail** | Marketplace listing automation, catalog command center, orders, inventory forecasting, pricing, analytics | Marketplace compliance automation is valuable: category/schema changes, missing attributes, rejected listings. |
| **Shopify Marketplace Connect** | Connect Shopify catalog to marketplaces, sync listings/orders/inventory/prices | Sellers want marketplace ops inside their existing system of record. Onword should integrate with existing workflows, not force migration. |
| **ShipStation** | Shipping, carrier rates, labels, tracking, returns, automation/API | Shipping is often a specialized action layer. For Korea, courier/tracking automation is a core module. |
| **Extensiv** | Order visibility, warehouse routing, inventory, fulfillment complexity tiers | Segment customers by operational maturity: marketplace-only → in-house warehouse → multi-warehouse/3PL. |
| **Cin7** | Inventory, accounting integrations, financial intelligence, warehouse, forecasting, manufacturing/BOM | ERP depth expands into inventory planning, purchasing, supplier, BOM/manufacturing. |
| **Brightpearl** | Retail operating system, automation engine, inventory planning, retail analytics | Sell “operations automation,” not “BI dashboard.” |
| **NetSuite-like ERP** | Accounting, order processing, inventory, production, supply chain, warehouse, returns | Long-term target: one source of truth across finance, inventory, orders, customer, supplier, channel. |

---

## 3. Key Functions We Need To Implement To Become A Selling Tool Company

### Priority Legend

- **MVP**: needed for the first useful selling operations dashboard.
- **Phase 2**: needed to become a serious selling tool, not just analytics.
- **Phase 3**: AI-native/ERP depth and moat-building.

## 3.1 Connector / Data Collection Layer

| Priority | Function | Why It Matters | Notes |
|---|---|---|---|
| MVP | Channel account connection | Without authentication/permission, no data. | Support API keys/OAuth/HMAC/JWT/vendor code/IP allowlisting. |
| MVP | Order collection | Core source of sales operations. | Poll every 1–5 minutes where allowed; use reconciliation windows. |
| MVP | Product/listing collection | Needed to map sales to SKU/listing health. | Pull product IDs, names, options, SKUs, sale status, category. |
| MVP | Inventory collection | Needed for stockout/oversell alerts. | Many channels expose partial stock; central stock may need seller ERP/OMS input. |
| MVP | Claim/return/cancel collection | Needed for daily exception queue and profit accuracy. | Normalize status/reason/date. |
| MVP | CS/Q&A/review collection where available | Customer service is a daily workflow, not optional. | Product Q&A and messages differ by platform. |
| MVP | Raw payload storage | Debugging and schema evolution. | Store exact original JSON/XML/CSV rows. |
| Phase 2 | Settlement/fee collection | Needed for profit and reconciliation. | Harder because channel settlement structures vary. |
| Phase 2 | Existing OMS import | Fastest adoption path. | Import Sabangnet/PlayAuto/Shoplinker exports/API if available. |
| Phase 2 | Webhook support | Reduces polling load. | Where marketplace supports webhooks. |
| Phase 3 | Connector health monitoring | Required at scale. | Alert on API failures, auth expiry, schema drift. |

## 3.2 Unified Data Structure / Normalization Layer

| Priority | Function | Why It Matters |
|---|---|---|
| MVP | Canonical IDs | Must link channel records to internal UDS entities. |
| MVP | Order-item-level normalization | One order can contain multiple product lines; dashboard must operate at item level. |
| MVP | Status normalization | Channel statuses differ; manager needs one status language. |
| MVP | Product/SKU alias mapping | Same product appears differently across channels. |
| MVP | Channel listing mapping | Same SKU can have different listing IDs, titles, prices, and statuses per channel. |
| MVP | Amount normalization | Gross/net/discount/shipping/refund/settlement must be comparable. |
| MVP | Date/time normalization | Order, pay, ship, delivery, claim dates need timezone and standard semantics. |
| MVP | PII handling | Buyer/receiver info may be masked; must handle missing/partial PII. |
| Phase 2 | Financial event normalization | Fees, payouts, refunds, ad spend, settlement events. |
| Phase 2 | Inventory ledger | Available/on-hand/committed/incoming/reserved/safety stock. |
| Phase 3 | Entity resolution with confidence | Auto-match SKUs/products/customers across noisy data. |

## 3.3 Unified Dashboard / Command Center

Store managers need an **exception-driven operating cockpit**.

### MVP Dashboard Sections

| Section | Must Show | Must Enable |
|---|---|---|
| Executive Summary | Today sales, orders, unshipped, overdue, low stock, open claims, CS overdue, estimated profit | Drill into queues |
| Order Queue | New/paid/awaiting shipment/fulfilled/cancelled/refunded orders by channel | Filter, export, assign, inspect |
| Fulfillment Queue | Due-to-ship, overdue, missing tracking, partial shipment, warehouse issue | Create task, upload tracking, handoff to WMS/OMS |
| Inventory Health | Low stock, out-of-stock, oversell risk, days remaining, stock mismatch | Reorder, pause listing, adjust stock |
| Claim/Return Queue | Open cancellation/return/exchange/refund, due dates, reasons | Approve, escalate, inspect root cause |
| Product/Listing Health | Listing errors, missing attributes, rejected listings, price/stock mismatch | Fix product data, resubmit, bulk edit |
| Settlement/Profit | Gross/net sales, fees, refund, shipping cost, estimated margin, settlement mismatch | Reconcile, investigate anomalies |
| CS Queue | Open inquiries, unanswered product Q&A, overdue replies, negative reviews | Reply, template, assign, link to order |
| Channel Performance | Sales/profit/return/SLA/listing errors by channel | Allocate inventory, adjust price, prioritize channel |

## 3.4 Action Layer

A dashboard that cannot act will become a reporting toy. Selling tools win because they let operators do work.

| Priority | Action | Notes |
|---|---|---|
| MVP | Create operational task | Low-risk; can work before write APIs. |
| MVP | Export action list | CSV/Excel for warehouse/CS/manager. |
| MVP | CS reply draft | AI can draft, human approves. |
| MVP | Product/listing fix recommendation | Identify missing/invalid attributes. |
| MVP | Inventory alert and reorder suggestion | Start read-only + task creation. |
| MVP | Settlement discrepancy task | Flag mismatch; human verifies. |
| Phase 2 | Tracking/invoice upload | Needs channel write permission. |
| Phase 2 | Stock sync/pause listing | High value, higher risk. Use approval workflows. |
| Phase 2 | Bulk product update/resubmission | Needs marketplace-specific schema compliance. |
| Phase 2 | Claim/return action | Approve/reject/refund through APIs where supported. |
| Phase 2 | Rule-based automation | If low stock → set channel stock buffer / pause listing. |
| Phase 3 | Agentic workflow execution | AI executes multi-step operational tasks with audit trail. |

## 3.5 Automation / Rules Engine

Mature selling tools converge on rules/automation.

Example rules:

```text
IF available_stock < safety_stock THEN create reorder task.
IF ship_by_at < now + 4h AND tracking_number is null THEN mark fulfillment as urgent.
IF channel_listing_error exists THEN assign catalog task to product manager.
IF settlement_expected - settlement_received > threshold THEN create finance exception.
IF claim_reason contains damaged/defective spike for SKU THEN create product quality investigation.
IF channel inventory mismatch > threshold THEN trigger stock sync check.
```

Required objects:

- `automation_rules`
- `automation_runs`
- `operational_tasks`
- `exceptions`
- `audit_logs`
- `approval_requests`

---

## 4. Recommended Product Roadmap For Onword

## MVP: Read-Only AI Command Center + Task Layer

Goal: useful without immediately competing with Sabangnet/PlayAuto write workflows.

Must include:

1. Connect 5 priority channels/API/export sources.
2. Build UDS order-item normalized database.
3. Show unified order/product/inventory/claim/settlement/CS cockpit.
4. Generate daily manager briefing.
5. Create operational tasks and recommendations.
6. Export queues for warehouse/CS/manager.
7. Store raw payloads for debugging.

MVP modules:

- Channel connector manager
- UDS normalized database
- Order and order-item dashboard
- Fulfillment exception queue
- Inventory risk dashboard
- Claims/returns/refunds queue
- Product/listing health dashboard
- Basic settlement/profit view
- CS inbox/Q&A summary if available
- AI briefing + recommendation engine
- Task/exception workflow

## Phase 2: Write Actions + Workflow Automation

Goal: become a true selling tool, not just a BI layer.

Add:

- Tracking/invoice upload
- Stock sync and channel stock buffers
- Product/listing bulk updates
- Claim/return actions
- CS reply send/approval
- Rule engine
- WMS/3PL/courier integrations
- Settlement reconciliation workflow
- Existing OMS connectors/importers
- Role permissions and audit logs

## Phase 3: AI-Native Commerce ERP

Goal: moat beyond legacy OMS.

Add:

- Demand forecasting
- Reorder/purchase order automation
- Supplier scorecards
- Product lifecycle management
- Contribution-margin-aware pricing/ad recommendations
- Automated root-cause analysis
- Channel compliance monitor
- Agentic operations copilot
- Accounting/tax integrations
- Warehouse labor/productivity analytics

---

## 5. Minimum Data Model To Support Selling Tool Functions

Core canonical tables:

- `channels`
- `channel_accounts`
- `raw_channel_payloads`
- `channel_sync_state`
- `products`
- `product_variants`
- `channel_listings`
- `orders`
- `order_items`
- `shipments`
- `shipment_items`
- `inventory_levels`
- `inventory_movements`
- `claims`
- `returns`
- `refunds`
- `settlement_batches`
- `settlement_lines`
- `financial_events`
- `customers`
- `receivers`
- `cs_threads`
- `cs_messages`
- `product_questions`
- `reviews`
- `operational_tasks`
- `exceptions`
- `automation_rules`
- `automation_runs`
- `audit_logs`

Dashboard aggregate tables:

- `dashboard_daily_sales`
- `dashboard_channel_performance_daily`
- `dashboard_sku_performance_daily`
- `dashboard_inventory_health`
- `dashboard_exception_counts`
- `dashboard_settlement_reconciliation`

Design principles:

1. Keep raw data forever or at least long enough to replay normalization.
2. Use append-only history for status, inventory, financial events, and actions.
3. Normalize at order-item level.
4. Track external channel IDs as first-class fields.
5. Treat exceptions/tasks as persisted workflow objects, not temporary UI states.
6. Separate canonical product from channel listing.
7. Allow incomplete/masked PII.
8. Keep channel write actions behind approval and audit logs.

---

## 6. Key Functions Checklist

| Module | Function | Priority | Build Notes |
|---|---|---|---|
| Connectors | API credentials/account setup | MVP | Per-channel auth patterns differ: OAuth, HMAC, JWT, API key, vendor code, IP allowlist. |
| Connectors | Scheduled polling and reconciliation | MVP | Need near-real-time + nightly backfill. |
| Connectors | Raw payload capture | MVP | Required for debugging, audits, schema changes. |
| Orders | Unified order inbox | MVP | Channel/status filters and item-level rows. |
| Orders | Order timeline/status history | MVP | Store changes, not just latest state. |
| Order Items | Product/order-line normalization | MVP | One row per purchased item/product order. |
| Fulfillment | Unshipped/overdue queue | MVP | Highest daily operational value. |
| Fulfillment | Tracking/invoice status | MVP | Read first, write later. |
| Inventory | Low-stock/out-of-stock alerts | MVP | Manager action trigger. |
| Inventory | Multi-location stock states | Phase 2 | Needed for WMS maturity. |
| Product | Channel listing health | MVP | Missing attributes, rejected listings, price/stock mismatch. |
| Product | Bulk product update | Phase 2 | Marketplace schema-specific and risky. |
| Claims | Cancel/return/exchange/refund queue | MVP | Daily exception workflow. |
| Settlement | Estimated profit and settlement mismatch | MVP | Start with approximate profit; improve with settlement APIs. |
| CS | Unified inquiry/Q&A queue | MVP | Especially valuable with product/order context. |
| CS | AI reply drafts | MVP | Low-risk human approval flow. |
| Automation | Operational task system | MVP | Foundation for actionability. |
| Automation | Rules engine | Phase 2 | Differentiates from passive dashboard. |
| AI | Daily manager briefing | MVP | Strong Onword-native wedge. |
| AI | Root-cause analysis | Phase 3 | Combine CS, returns, SKU, supplier, channel, settlement. |
| Finance | Fee/COGS/ad-spend joins | Phase 2 | Needed for real margin/profit. |
| ERP | Purchasing/replenishment | Phase 2 | Reorder recommendations and supplier workflows. |
| Audit | Permissions and action logs | Phase 2 | Required before write actions. |

---

## 7. Competitive Positioning Recommendation

### Bad positioning

```text
“We are another Sabangnet/PlayAuto.”
```

This is weak because incumbents have channel coverage, workflow depth, and years of edge-case handling.

### Better positioning

```text
“AI command center for multichannel commerce operations.”
```

Meaning:

- It sits above existing channels and optionally existing OMS tools.
- It unifies data into UDS.
- It identifies urgent operational/financial/customer problems.
- It recommends actions.
- It gradually executes approved actions.

### Best wedge for Barudak-like sellers

1. **Read from all channels.**
2. **Normalize into UDS.**
3. **Daily manager briefing + exception queues.**
4. **Settlement/profit reconciliation.**
5. **Stockout/overstock and fulfillment risk prediction.**
6. **AI CS and claim response support.**
7. **Write-back automations later.**

This avoids the hardest initial problem: replacing the seller's current OMS/warehouse operations from day one.

---

## 8. Source URLs

### Korean tools

- Sabangnet: https://www.sabangnet.co.kr/
- Sabangnet support malls: https://www.sabangnet.co.kr/service-intro/support-malls
- PlayAuto: https://www.plto.com/
- PlayAuto pricing: https://www.plto.com/introduction/Charge/?tabActive=0
- PlayAuto supported shops: https://www.plto.com/introduction/ShopList/?tabActive=0
- Shoplinker: https://www.shoplinker.co.kr/
- Shoplinker pricing: https://www.shoplinker.co.kr/price/price_info
- Shoplinker supported malls: https://www.shoplinker.co.kr/service/supported_mall
- Sellmate: https://sellmate.io/
- Sellmate pricing: https://sellmate.io/price
- Sellpia: https://www.sellpia.com/
- Sellpia pricing: https://www.sellpia.com/pricing.html
- Sellpia sales/support channels: https://www.sellpia.com/sales.html
- EasyAdmin: https://www.ezadmin.co.kr/index.html
- EasyAdmin supported malls: https://www.ezadmin.co.kr/sub_01_02.html
- EasyAdmin add-ons/services: https://www.ezadmin.co.kr/sub_02_03.html
- Cafe24 Market Plus: https://www.cafe24.com/commerce/channel/market.html
- ESM PLUS: https://www.esmplus.com/
- Naver SmartStore Center: https://sell.smartstore.naver.com/
- Coupang Wing: https://wing.coupang.com/
- Coupang Marketplace: https://marketplace.coupang.com/

### Global platforms

- Rithum Marketplace Listings: https://www.rithum.com/products/brands/marketplace-listings/
- Rithum Inventory Management: https://www.rithum.com/products/brands/inventory-management/
- Rithum Order Management: https://www.rithum.com/products/brands/order-management/
- Rithum Commerce Insights: https://www.rithum.com/products/brands/commerce-insights-reporting/
- Linnworks features: https://www.linnworks.com/features/
- Sellbrite: https://www.sellbrite.com/how-sellbrite-works/
- Sellbrite API: https://developer.sellbrite.com/
- Sellercloud features: https://sellercloud.com/features/
- Sellercloud API: https://sellercloud.com/features/web-service-api/
- Zentail: https://www.zentail.com/
- Shopify Marketplace Connect: https://apps.shopify.com/marketplace-connect
- ShipStation fulfillment: https://www.shipstation.com/fulfillment/
- ShipStation API: https://www.shipstation.com/fulfillment/api/
- Extensiv order management: https://www.extensiv.com/brands/order-management
- Cin7 features: https://www.cin7.com/features/
- Brightpearl: https://www.brightpearl.com/
- NetSuite ERP: https://www.netsuite.com.sg/portal/sg/products/erp.shtml
- NetSuite Returns Management: https://www.netsuite.com/portal/products/erp/order-management/returns-management.shtml

### Dashboard/API pattern references

- Shopify Admin GraphQL docs: https://shopify.dev/docs/api/admin-graphql
- Amazon Selling Partner API docs: https://developer-docs.amazon.com/sp-api/
- Google Merchant Center Help: https://support.google.com/merchants/
- Meta Marketing API Insights: https://developers.facebook.com/docs/marketing-api/insights/

---

## 9. Caveats

1. Some pages were bot-protected or dynamic, especially Coupang Wing and some Cafe24 pages. Where direct official content was blocked, official URLs plus accessible snippets/public pages were used.
2. Channel counts are marketing/support-table counts, not verified API capability counts. A channel can support order collection but not product registration, CS, settlement, or claim actions.
3. Pricing changes frequently; use captured pricing as directional, not contractual.
4. The decisive moat is not “having a dashboard.” It is combining data normalization, operational exceptions, and safe action execution across channels.
