# CJ OnStyle Future Channel API Note

## Status

CJ OnStyle Standard API is a credible future API connector candidate.

## Known details

- Partner docs: `https://partners.cjonstyle.com/standardApi`
- Delivery/order endpoint identified: `POST https://ingress-api.cjoshopping.com/delivery/getDeliveryList`
- QA endpoint: `https://qa-ingress-api.cjoshopping.com/delivery/getDeliveryList`
- Auth headers include `vendorCode` and `authenticationKey`.
- IP allowlisting is typically required before production calls.
- Candidate unique key: `CJONSTYLE:{orderNo}:{orderItemSequence}:{orderDetailSequence}:{orderProcessingSequence}`.

## Connector implications

- Strong phase-2 candidate after credential/IP setup.
- Extract order, shipment, claim, settlement field dictionaries before joining MVP UDS mapping.
