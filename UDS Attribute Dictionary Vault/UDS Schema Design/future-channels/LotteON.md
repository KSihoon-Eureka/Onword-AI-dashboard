# LotteON Future Channel API Note

## Status

LotteON OpenAPI is a credible future API connector candidate.

## Known details

- OpenAPI host commonly referenced as `https://openapi.lotteon.com`.
- Delivery/order-search API identified: `POST /v1/openapi/delivery/v1/SellerDeliveryOrdersSearch`.
- Korean API name: 출고/회수지시(주문정보) 조회.
- Access requirements: seller API key and likely server IP registration or seller-tool onboarding; key validity may be time-limited.

## Connector implications

- Good candidate for actionable order/fulfillment polling.
- Historical backfill and settlement coverage require separate endpoint confirmation.
- Extract a LotteON field dictionary before adding to UDS mapping.
