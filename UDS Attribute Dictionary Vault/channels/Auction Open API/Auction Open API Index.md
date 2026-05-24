---
title: Auction Open API
channel: Auction Open API
source: api-doc-extraction
extracted_at: 2026-05-24T22:02:43
---

# Auction Open API

- Source type: legacy Auction SOAP/XML Open API.
- Primary API docs/WSDLs:
  - `http://api.auction.co.kr/APIv1/AuctionService.asmx?WSDL`
  - `http://api.auction.co.kr/APIv1/ShoppingService.asmx?WSDL`
  - `http://api.auction.co.kr/APIv1/SecurityService.asmx?WSDL`
- [[01 - Universal Total Table — 전체 Auction Open API 고유 UDS 속성|Universal Total Table — 전체 Auction Open API 고유 UDS 속성]] — 1610 rows including header; CSV: `_csv/Auction Open API/01 - Universal Total Table — 전체 Auction Open API 고유 UDS 속성.csv`
- [[Source Page Text]]

## Extraction stats

- WSDL services scanned: 3
- Operations discovered: 220
- Operation pages fetched: 220
- Raw field names extracted: 2924
- Semantic UDS attributes: 1609
- ✅ 핵심 UDS: 1219
- 🟡 후보: 104
- ⚪ 선택 / 낮음: 286

## Area counts

- 기타 API: 1253
- 상품 API: 761
- 주문/배송 API: 367
- 클레임 API: 164
- 정산 API: 106
- CS API: 70
- 인증 API: 47

## Interpretation

- This is **not** a replacement for the newer `Gmarket Auction` ESM dictionary already in this vault. It is a supplementary Auction-only legacy Open API source.
- Use the ESM dictionary as the primary modern connector reference; use this table to catch Auction SOAP fields/operations that still matter or reveal older business concepts.
