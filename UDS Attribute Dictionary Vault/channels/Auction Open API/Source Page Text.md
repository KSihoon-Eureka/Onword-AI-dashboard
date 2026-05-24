---
title: Auction Open API Source Page Text
channel: Auction Open API
type: source-summary
---

# Auction Open API Source Page Text

Legacy Auction Open API docs inspected for UDS extraction. Main docs discovered in previous thread and re-used here.

## Source URLs

- https://developer.auction.co.kr/Information.aspx?menu=sub1
- https://developer.auction.co.kr/Information.aspx?menu=sub2
- https://developer.auction.co.kr/APITools/ReferenceSearchList.aspx
- http://api.auction.co.kr/APIv1/AuctionService.asmx?WSDL
- http://api.auction.co.kr/APIv1/ShoppingService.asmx?WSDL
- http://api.auction.co.kr/APIv1/SecurityService.asmx?WSDL

## Extraction notes

- WSDL services scanned: 3
- Operations discovered: 220
- Operation pages fetched: 220
- Operation page fetch failures: 0
- Raw field names extracted: 2924
- Semantic UDS attributes: 1609

## Services

- AuctionService: `http://api.auction.co.kr/APIv1/AuctionService.asmx?WSDL` — 678,398 bytes
- ShoppingService: `http://api.auction.co.kr/APIv1/ShoppingService.asmx?WSDL` — 344,427 bytes
- SecurityService: `http://api.auction.co.kr/APIv1/SecurityService.asmx?WSDL` — 9,942 bytes

## Caveat

This source is older SOAP/XML Auction Open API. For modern Gmarket/Auction integration, treat ESM Trading API as primary and this as a legacy/supplementary Auction-specific attribute source.
