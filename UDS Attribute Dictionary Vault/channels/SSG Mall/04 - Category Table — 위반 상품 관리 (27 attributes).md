---
title: Category Table — 위반 상품 관리 (27 attributes)
channel: SSG Mall
type: notion-table-migration
source_notion_page_id: 369559dfde8580d38e38d7a0019a37aa
source_table_id: 369559df-de85-81a0-96e6-f94d4871e2d2
rows_including_header: 28
csv_backup: ../../_csv/SSG Mall/04 - Category Table — 위반 상품 관리 (27 attributes).csv
---

# Category Table — 위반 상품 관리 (27 attributes)

- Channel: [[SSG Mall Index|SSG Mall]]
- Rows including header: **28**
- CSV backup: `../../_csv/SSG Mall/04 - Category Table — 위반 상품 관리 (27 attributes).csv`

| UDS 속성명 | SSG 필드명 | API 카테고리 | 사용 API 문서 수 | 공통/반복 | UDS 필요도 | 설명 |
| --- | --- | --- | --- | --- | --- | --- |
| API 인증키 | Authorization | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | Authorization: Vendor API Authentication Key \| Authorization: 샘플코드에서 확인된 필드 \| Authorization: 샘플코드에서 확인된 필드 |
| Action Sales Status Applicatio | itemQualEndDts | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualEndDts: Action Sales Status Application Period End date and time |
| Ending Date for Seaching Regis | searchEndDate | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | searchEndDate: Ending Date for Seaching Registration Date(YYYYMMDD) ※ To set the start date and end date, both values must be entered. |
| Explanation Contents | explCntt | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | explCntt: Explanation Contents |
| Item Quality Inflow Type | itemQualInfloTypeNm | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualInfloTypeNm: Item Quality Inflow Type |
| Item Quality Inflow Type Code  | itemQualInfloTypeCd | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualInfloTypeCd: Item Quality Inflow Type Code 11 : Management of Risk Item Blocking 12 : Management of Item Report 13 : IPR Center Report 14 : Management of Item Information Violations 20 : Management of OCR Item Information Quality 30 : OCR Abnormal Images 31 : OCR Abnormal Images (Item Detail Description) 40 : Expiration of Item Information Edit 50 : SIRENS Text Search |
| Item Quality Process Result | itemQualProcRstNm | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualProcRstNm: Item Quality Process Result |
| Item Quality Process Result Co | itemQualProcRstCd | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualProcRstCd: Item Quality Process Result Code 90 : RM Report Received 05 : RM Confirmation Requested 20 : RM Confirmation Rejected 10 : RM Confirmation Completed \| itemQualProcRstCd: Item Quality Process Result Code 90 : RM Report Received 05 : RM Confirmation Requested 20 : RM Confirmation Rejected 10 : RM Confirmation Completed |
| Sell Status | sellStatNm | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | sellStatNm: Sell Status |
| Sell Status Code (commCd:I004) | sellStatCd | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | sellStatCd: Sell Status Code (commCd:I004) 05 : Additional Information Required 10 : Pending Approval 20 : For Sale 80 : Temporary Suspension of Sales 85 : Sale Prohibition 90 : Permanent Suspension of Sales \| sellStatCd: Sell Status Code (commCd:I004) 05 : Additional Information Required 10 : Pending Approval 20 : For Sale 80 : Temporary Suspension of Sales 85 : Sale Prohibition 90 : Permanent Suspension of Sales |
| Starting Date for Seaching Reg | searchStartDate | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | searchStartDate: Starting Date for Seaching Registration Date(YYYYMMDD) ※ To set the start date and end date, both values must be entered. |
| Violation Contents | itemQualViolRsnNm | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualViolRsnNm: Violation Contents |
| Violation Detail Contents | itemQualViolCntt | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualViolCntt: Violation Detail Contents |
| Violation Registration Date | itemQualRegDt | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemQualRegDt: Violation Registration Date |
| object | item | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | item: object |
| rmItems | rmItems | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS |  |
| updateRiskManagement 일자 | updateRiskManagement | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS |  |
| 결과 | result | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS |  |
| 결과 메시지 | resultMessage | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | resultMessage: Result Message \| resultMessage: Result Message |
| 결과 설명 | resultDesc | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | resultDesc: Error Message \| resultDesc: Error Message |
| 결과코드 | resultCode | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | resultCode: Result Code (00 indicates a normal status, all other codes represent errors) \| resultCode: Result Code (00 indicates a normal status, all other codes represent errors) |
| 상품 ID | itemId | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemId: Item Identification ※ If this value is set, other parameters are ignored. \| itemId: Item Identification \| itemId: Item Identification |
| 상품명 | itemNm | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | itemNm: Item Name |
| 샘플코드에서 확인된 필드 | accept | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | accept: 샘플코드에서 확인된 필드 \| accept: 샘플코드에서 확인된 필드 \| accept: 샘플코드에서 확인된 필드 |
| 응답 형식 | Accept | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | Accept: application/xml application/json \| Accept: application/xml application/json |
| 페이지 번호 | page | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | page: Page |
| 페이지 크기 | pageSize | 위반 상품 관리 | 1 | 단일 | ✅ 핵심 UDS | pageSize: Number of Prints Per Page |
