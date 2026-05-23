---
title: Category Table — 백화점 배송 (121 attributes)
channel: SSG Mall
type: notion-table-migration
source_notion_page_id: 369559dfde8580d38e38d7a0019a37aa
source_table_id: 369559df-de85-8113-86ab-f1f5f7a0e0c0
rows_including_header: 122
csv_backup: ../../_csv/SSG Mall/11 - Category Table — 백화점 배송 (121 attributes).csv
---

# Category Table — 백화점 배송 (121 attributes)

- Channel: [[SSG Mall Index|SSG Mall]]
- Rows including header: **122**
- CSV backup: `../../_csv/SSG Mall/11 - Category Table — 백화점 배송 (121 attributes).csv`

| UDS 속성명 | SSG 필드명 | API 카테고리 | 사용 API 문서 수 | 공통/반복 | UDS 필요도 | 설명 |
| --- | --- | --- | --- | --- | --- | --- |
| API 인증키 | Authorization | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | Authorization: 업체 인증키 Vendor API Authentication Key \| Authorization: 샘플코드에서 확인된 필드 \| Authorization: 샘플코드에서 확인된 필드 |
| Integer | dircItemQty / norRetProcQty / ordCnfdocNo / refusRetProcQty / shppDgr / whinDelayNts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDgr: Integer \| ordCnfdocNo: Integer \| whinDelayNts: Integer |
| Lot 위치 Lot Position | ordLotPst | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordLotPst: Lot 위치 Lot Position |
| LotNo Lot Number | ordLotNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordLotNo: LotNo Lot Number |
| POS 전송여부 Sent POS Y/N | posTrmsYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | posTrmsYn: POS 전송여부 Sent POS Y/N |
| POS 전송여부 Y Yes N No POS Sent Y | posSendYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | posSendYn: POS 전송여부 Y Yes N No POS Sent Y/N Y Yes N No |
| POS 전송처리자 Sent POS Processor | posTrmsRegpeId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | posTrmsRegpeId: POS 전송처리자 Sent POS Processor |
| PP회수확인일 PP Recollect Confirmed | ppRcovCnfDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ppRcovCnfDt: PP회수확인일 PP Recollect Confirmed Date \| ppRcovCnfDt: PP회수확인일 PP Recollect Confirmed Date |
| PP회수확인처리자 PP Recollect Confirm Processor | ppRcovCnfNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ppRcovCnfNm: PP회수확인처리자 PP Recollect Confirm Processor \| ppRcovCnfNm: PP회수확인처리자 PP Recollect Confirm Processor |
| Y | ordCnfdocNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordCnfdocNo: Y |
| eShop 주문여부 Y/N eShop Order Yes | fitOrdYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | fitOrdYn: eShop 주문여부 Y/N eShop Order Yes Or No Y/N \| fitOrdYn: eShop 주문여부 Y/N eShop Order Yes Or No Y/N |
| eShop 주문여부 eShop Order Yes or  | fitOrdYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | fitOrdYn: eShop 주문여부 eShop Order Yes or No \| fitOrdYn: eShop 주문여부 eShop Order Yes or No |
| pickgTarget | pickgTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| pickgTargets | pickgTargets | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| rcovCompleteTarget | rcovCompleteTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| rcovCompleteTargets | rcovCompleteTargets | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| rcovDirectionTarget | rcovDirectionTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| rcovDirectionTargets | rcovDirectionTargets | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| requestOrderSubjectManage | requestOrderSubjectManage | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| requestPickgTarget | requestPickgTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| requestRcovCompleteTarget | requestRcovCompleteTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| requestRcovDirectionTarget | requestRcovDirectionTarget | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS |  |
| vvip Y/N vvip Y/N | vvipYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | vvipYn: vvip Y/N vvip Y/N |
| 결과 | result | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | result: 샘플코드에서 확인된 필드 \| result: 샘플코드에서 확인된 필드 \| result: 샘플코드에서 확인된 필드 |
| 결과 메시지 | resultMessage | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | resultMessage: 결과 값 Result Message \| resultMessage: 샘플코드에서 확인된 필드 \| resultMessage: 결과 값 Result Message |
| 결과 설명 | resultDesc | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | resultDesc: 오류 메시지 Error Message \| resultDesc: 샘플코드에서 확인된 필드 \| resultDesc: 오류 메시지 Error Message |
| 결과코드 | resultCode | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | resultCode: 결과 코드 Result Code \| resultCode: 샘플코드에서 확인된 필드 \| resultCode: 결과 코드 Result Code |
| 결품등록여부 shortage item regist Y/ | shortgRegYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shortgRegYn: 결품등록여부 shortage item regist Y/N |
| 고객반품메모 Claim Reason Content | clmRsnCntt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | clmRsnCntt: 고객반품메모 Claim Reason Content \| clmRsnCntt: 고객반품메모 Claim Reason Content |
| 고객반품사유 Claim Reason Name | clmRsnNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | clmRsnNm: 고객반품사유 Claim Reason Name \| clmRsnNm: 고객반품사유 Claim Reason Name |
| 국내/외 구분 Y/N Domestic Or Intern | frgShppYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | frgShppYn: 국내/외 구분 Y/N Domestic Or International Yes Or No Domestic : N International : Y |
| 귀책사유주체 Return Request Reason Main | retImptMainNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retImptMainNm: 귀책사유주체 Return Request Reason Main |
| 단품 ID | uitemId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | uitemId: 단품ID Unit Item Identification \| uitemId: 샘플코드에서 확인된 필드 \| uitemId: 단품번호 Unit Item Number |
| 단품명 | uitemNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | uitemNm: 단품명 Unit Item Name \| uitemNm: 샘플코드에서 확인된 필드 \| uitemNm: 속성 Unit Item Name |
| 물류회수확인일 Logistics Recollect Co | logisRcovCnfDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | logisRcovCnfDt: 물류회수확인일 Logistics Recollect Confirmed Date \| logisRcovCnfDt: 물류회수확인일 Logistics Recollect Confirmed Date |
| 물류회수확인처리자 Logistics Recollect Confirm Pr | logisRcovCnfNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | logisRcovCnfNm: 물류회수확인처리자 Logistics Recollect Confirm Processor \| logisRcovCnfNm: 물류회수확인처리자 Logistics Recollect Confirm Processor |
| 미피킹 등록여부 Y Yes N No Registed Shortage It | shortgRegYns | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shortgRegYns: 미피킹 등록여부 Y Yes N No Registed Shortage Item Y/N Y Yes N No |
| 반품거부등록자 Return Refusal Registrant | retProcUserNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retProcUserNm: 반품거부등록자 Return Refusal Registrant |
| 반품거부메모 Return Denied Memo | retProcMemoCntt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retProcMemoCntt: 반품거부메모 Return Denied Memo |
| 반품거부사유 01 기간경과 02 사용상품 03 상품불량 04 구성품누락  | retRefusRsnCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retRefusRsnCds: 반품거부사유 01 기간경과 02 사용상품 03 상품불량 04 구성품누락 05 사은품누락 06 상품상이 07 상품수량상이 08 상품훼손/파손 09 케이스(BOX)파손 10 상담원과실 12 불량판정서 미동봉 11 기타 Return Denied Reason Overlap permitted. Must use ',' for division. 01 Period Elapsed 02 Use Item 03 Faulty Item 04 Main Item Omitted 05 Free Gift Omitted 06 Item Incorrect 07 Item Quantity Incorrect 08 Item Damage 09 Case(Box) Damage 10 Consultant's Mistake 12 Bad Judgment Unpackaged 11 Other |
| 반품거부사유 Return Denied Reason | retRefusRsnNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retRefusRsnNm: 반품거부사유 Return Denied Reason |
| 반품상태 10 반품완료 20 반품거부 30 반품거부CS처리중 40 반품거 | retProcStats | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retProcStats: 반품상태 10 반품완료 20 반품거부 30 반품거부CS처리중 40 반품거부CS처리완료 50 반품확인 60 회수철회 Return Process Status 10 Return Completed 20 Return Denied 30 Return Denied CS Processing 40 Return Denied CD Processing Completed 50 Return Confirmed 60 Return Revoked |
| 반품처리상태 Return Process Status | retProcStatNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | retProcStatNm: 반품처리상태 Return Process Status |
| 배송구분 21 반품회수 22 교환회수 23 AS회수 Release Typ | shppDivDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDivDtlCds: 배송구분 21 반품회수 22 교환회수 23 AS회수 Release Type 21 Return 22 Exchange 23 AS \| shppDivDtlCds: 배송구분 21 반품회수 22 교환회수 23 AS회수 Release Type 21 Return 22 Exchange 23 AS |
| 배송구분 Release Type Name | shppDivDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDivDtlNm: 배송구분 Release Type Name \| shppDivDtlNm: 배송구분 Release Type Name |
| 배송구분상세코드 11 일반출고 12 부분출고 13 기출하 14 재배송 1 | shppDivDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDivDtlCds: 배송구분상세코드 11 일반출고 12 부분출고 13 기출하 14 재배송 15 교환출고 16 AS출고 Release Type 11 General Release 12 Partial Release 13 Already Release 14 Re-shipping 15 Exchange Release 16 AS Release |
| 배송번호 | shppNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppNo: 배송번호 Shipping Number \| shppNo: 샘플코드에서 확인된 필드 \| shppNo: 배송번호 Shipping Number |
| 배송비부담주체 Shipping Cost Payee Main | shppcstBdnMainNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppcstBdnMainNm: 배송비부담주체 Shipping Cost Payee Main |
| 배송사 메모 | memoCntt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | memoCntt: 배송업무메모 Shipping Company Memo \| memoCntt: 배송업무메모 Shipping Company Memo |
| 배송상태 10 정상 20 취소 Shipping Status Code 10 | shppStatCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppStatCds: 배송상태 10 정상 20 취소 Shipping Status Code 10 Normal 20 Cancel \| shppStatCds: 배송상태 10 정상 20 취소 Shipping Status Code 10 Normal 20 Cancel |
| 배송상태 코드 | shppStatCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppStatCd: 샘플코드에서 확인된 필드 |
| 배송상태명 Shipping Status Name | shppStatNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppStatNm: 배송상태명 Shipping Status Name |
| 배송상태코드 10 정상 30 대기 Shipping Status Code  | shppStatCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppStatCds: 배송상태코드 10 정상 30 대기 Shipping Status Code 10 Normal 30 On Hold |
| 배송순번 | shppSeq | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppSeq: Integer \| shppSeq: 샘플코드에서 확인된 필드 \| shppSeq: Y |
| 배송예약일 | shppRsvtDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppRsvtDt: 출고예정일 Process Date at Picking Direction \| shppRsvtDt: 샘플코드에서 확인된 필드 |
| 배송유형 10 자사배송 20 택배배송 30 매장방문 70 퀵/당일배송 8 | shppTypeCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeCds: 배송유형 10 자사배송 20 택배배송 30 매장방문 70 퀵/당일배송 80 글로벌배송 Shipping Type Code 10 In-House Shipping 20 3rd party Logistics 30 In-Store Visit 70 Express Delivery Service 80 International Shipping \| shppTypeCds: 배송유형 10 자사배송 20 택배배송 30 매장방문 70 퀵/당일배송 80 글로벌배송 Shipping Type Code 10 In-House Shipping 20 3rd party Logistics 30 In-Store Visit 70 Express Delivery Service 80 International Shipping |
| 배송유형 Shipping Type Detail Name | shppTypeDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeDtlNm: 배송유형 Shipping Type Detail Name \| shppTypeDtlNm: 배송유형 Shipping Type Detail Name |
| 배송유형 상세코드 | shppTypeDtlCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeDtlCd: 샘플코드에서 확인된 필드 |
| 배송유형 코드 | shppTypeCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeCd: 샘플코드에서 확인된 필드 |
| 배송유형명 Shipping Type Name | shppTypeNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeNm: 배송유형명 Shipping Type Name |
| 배송유형상세 11 일반자사배송 21 지정택배배송 32 매장픽업 71 퀵배 | shppTypeDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeDtlCds: 배송유형상세 11 일반자사배송 21 지정택배배송 32 매장픽업 71 퀵배송 81 글로벌지정택배배송 34 픽업데스크픽업 Detail Shipping Type Code 11 In-House Shipping 21 3rd party Logistics 32 Store Pick-Up 71 Express Delivery Service 81 International Shipping 34 Desk Pick-Up |
| 배송유형상세명 Shipping Type Detail Name | shppTypeDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeDtlNm: 배송유형상세명 Shipping Type Detail Name |
| 배송유형코드 10 자사배송 20 택배배송 30 매장방문 70 퀵/당일배송 | shppTypeCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppTypeCds: 배송유형코드 10 자사배송 20 택배배송 30 매장방문 70 퀵/당일배송 80 글로벌배송 Shipping Type Number 10 In-House Shipping 20 3rd party Logistics 30 In-Store Visit 70 Express Delivery Service 80 International Shipping |
| 배송주체 13 센터입고브랜드 Shipping Main Code 13 Lo | shppMainCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppMainCds: 배송주체 13 센터입고브랜드 Shipping Main Code 13 Logistics center \| shppMainCds: 배송주체 13 센터입고브랜드 Shipping Main Code 13 Logistics center |
| 배송주체 Shipping Main Code Name | shppMainNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppMainNm: 배송주체 Shipping Main Code Name |
| 배송차수 1 1차수 2 2차수 3 3차수 4 4차수 Shipping Re | shppDrgs | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDrgs: 배송차수 1 1차수 2 2차수 3 3차수 4 4차수 Shipping Release Number 1 First Release 2 Second Release 3 Third Release 4 Fourth Release |
| 빠른조회값, 빠른조회일 경우 필수 값 If quick search, th | commValue | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | commValue: 빠른조회값, 빠른조회일 경우 필수 값 If quick search, then mandatory value. \| commValue: 빠른조회값, 빠른조회일 경우 필수 값 If quick search, then mandatory value. |
| 빠른조회타입, 빠른조회일 경우 필수 값 01 주문번호 02 배송번호 03 | commType | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | commType: 빠른조회타입, 빠른조회일 경우 필수 값 01 주문번호 02 배송번호 03 주문확인서번호 04 운송장번호 If general search, then mandatory value. 01 Order Number 02 Shipping Number 03 Order Confirmation Number 04 Waybill Number |
| 빠른조회타입, 빠른조회일 경우 필수 값 01 주문확인서번호 02 주문번호 | commType | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | commType: 빠른조회타입, 빠른조회일 경우 필수 값 01 주문확인서번호 02 주문번호 03 배송번호 04 운송장번호 If general search, then mandatory value. 01 Order Confirmation Number 02 Order Number 03 Shipping Number 04 Waybill Number |
| 사은품 Free Gifts | frebie / frebieNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | frebie: 사은품 Free Gifts \| frebieNm: 사은품 Free Gifts |
| 상세배송구분 Release Type Name | shppDivDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDivDtlNm: 상세배송구분 Release Type Name |
| 상세배송상태 11 배송지시 21 피킹지시 22 피킹완료 31 패킹완료 4 | lastShppProgStatDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | lastShppProgStatDtlCds: 상세배송상태 11 배송지시 21 피킹지시 22 피킹완료 31 패킹완료 41 출고대기 42 출고보류 43 출고완료 51 배송완료 52 배송거절 Detail Shipping Process Status 11 Shipping Instructed 21 Picking Instructed 22 Picking Completed 31 Packing Completed 41 Release On Hold 42 Release Delayed 43 Release Completed 51 Shipping Completed 52 Shipping Rejected |
| 상세배송진행상태 61 회수지시 62 물류회수확인 63 회수확인 66 회수 | shppProgStatDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppProgStatDtlCds: 상세배송진행상태 61 회수지시 62 물류회수확인 63 회수확인 66 회수철회 Recollect Status 61 Recollect Instructed 62 Recollect Confirmed(Logistics center) 63 Recollect Confirmed(Picking&Packing center) 66 Recollect Revoked |
| 상품 ID | itemId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | itemId: 상품번호 Item Number \| itemId: 샘플코드에서 확인된 필드 \| itemId: 상품번호 Item Number |
| 상품명 | itemNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | itemNm: 상품명 Item Name \| itemNm: 샘플코드에서 확인된 필드 \| itemNm: 상품명 Item Name |
| 샘플코드에서 확인된 필드 | accept / allnTypeNm / clmRsnCntt / clmRsnNm / delicoVenNm / dircItemQty / dptsFloNm / evntStrtDts / fitOrdYn / frgShppNm / frgShppYn / giftOrdYn / lastShppProgStatDtlCd / lastShppProgStatDtlNm / logisRcovCnfDt / logisRcovCnfNm / lrnkSplVenNm / norRetProcQty / ordCnfdocNo / ordListPrintYn / ordLotNo / ordLotPst / pickgTarget / pickgTargets / posTrmsRegpeId / posTrmsYn / ppRcovCnfDt / ppRcovCnfNm / rcovCompleteTarget / rcovCompleteTargets / rcovDircDt / rcovDirectionTarget / rcovDirectionTargets / rcovMthdNm / refundYn / requestPickgCmpl / requestPickgTarget / requestRcovCompleteTarget / requestRcovDirectionTarget / resellPsblYn / retProcStatNm / salestrNm / salestrNo / shppDgr / shppDivDtlNm / shppMainCd / shppMainCds / shppMainNm / shppStatNm / shppTypeCds / shppTypeDtlNm / shppTypeNm / shppcstBdnMainNm / trsfYn / whinDelayNts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | accept: 샘플코드에서 확인된 필드 \| requestPickgTarget: 샘플코드에서 확인된 필드 \| accept: 샘플코드에서 확인된 필드 |
| 선물포장메세지 Gift Message | giftPackMemoCntt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | giftPackMemoCntt: 선물포장메세지 Gift Message |
| 선물하기 주문여부 Y/N Gift Order Y/N | giftOrdYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | giftOrdYn: 선물하기 주문여부 Y/N Gift Order Y/N |
| 선물하기 주문여부 Y/N Y Yes N No Gift  | giftOrdYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | giftOrdYn: 선물하기 주문여부 Y/N Y Yes N No Gift Order Y/N Y Yes N No |
| 수거지시(집하)일 Collect Completed Da | colctCmplDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | colctCmplDt: 수거지시(집하)일 Collect Completed Date |
| 수령자명 | rcptpeNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcptpeNm: 수취인 Recipient \| rcptpeNm: 샘플코드에서 확인된 필드 \| rcptpeNm: 수취인 Recipient |
| 영업점 변경여부 Change Sales store Y/ | trsfYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | trsfYn: 영업점 변경여부 Change Sales store Y/N |
| 운송장번호 | wblNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | wblNo: 운송장번호 Waybill Number \| wblNo: 운송장번호 Waybill Number \| wblNo: 샘플코드에서 확인된 필드 |
| 원주문번호 | orordNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | orordNo: 주문번호 Order Number \| orordNo: 샘플코드에서 확인된 필드 \| orordNo: 주문번호 Order Number |
| 응답 형식 | Accept | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | Accept: application/xml application/json application/xml application/json \| Accept: application/xml application/json application/xml application/json \| Accept: application/xml application/json application/xml application/json |
| 재판매가능 구분 Resell Possibility Di | resellPsblYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | resellPsblYn: 재판매가능 구분 Resell Possibility Division |
| 점포코드 1002 본점 1003 타임스퀘어점리빙관 10 | salestrNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | salestrNo: 점포코드 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 Department Code 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 \| salestrNo: 점포코드 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 Department Code 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 |
| 점포코드 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 100 | salestrNos | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | salestrNos: 점포코드 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 Department Code 1002 본점 1003 타임스퀘어점리빙관 1004 강남점 1005 인천점 1006 사우스시티 1007 의정부점 1008 광주신세계 1009 센텀시티점 1010 마산점 1011 아라리오점 1013 타임스퀘어점패션관 1024 대전신세계 1020 시코르강남역점 1022 팩토리스토어 고양점 1017 김해점 1018 하남점 1021 팩토리스토어 강남점 1023 온라인점 1019 대구신세계 |
| 제휴구분 Alliance Type Name | allnTypeNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | allnTypeNm: 제휴구분 Alliance Type Name \| allnTypeNm: 제휴구분 Alliance Type Name \| allnTypeNm: 제휴구분 Alliance Type Name |
| 조회 시작일 | perdStrDts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | perdStrDts: 기간시작일, 일반조회일 경우 필수 값. 기간은 15일 이내 If general search, then mandatory value. Period is within 15 days \| perdStrDts: 샘플코드에서 확인된 필드 \| perdStrDts: 샘플코드에서 확인된 필드 |
| 조회 종료일 | perdEndDts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | perdEndDts: 기간종료일, 일반조회일 경우 필수 값. 기간은 15일 이내 If general search, then mandatory value. Period is within 15 days \| perdEndDts: 샘플코드에서 확인된 필드 \| perdEndDts: 샘플코드에서 확인된 필드 |
| 조회기간 유형 | perdType | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | perdType: 기간타입, 일반조회일 경우 필수 값 01 피킹지시일 If general search, then mandatory value. 01 Picking Direction Date \| perdType: 샘플코드에서 확인된 필드 \| perdType: 샘플코드에서 확인된 필드 |
| 주문 배송메모 | ordMemoCntt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordMemoCntt: 고객배송메모 Customer Shipping Memo \| ordMemoCntt: 샘플코드에서 확인된 필드 |
| 주문리스트출력여부 print order List Y/N | ordListPrintYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordListPrintYn: 주문리스트출력여부 print order List Y/N |
| 주문번호 | ordNo | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordNo: 주문번호 Order Number \| ordNo: 샘플코드에서 확인된 필드 |
| 주문자Id Customer Id | ordpeId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordpeId: 주문자Id Customer Id |
| 주문자명 | ordpeNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordpeNm: 주문자 Customer \| ordpeNm: 샘플코드에서 확인된 필드 \| ordpeNm: 주문자 Customer |
| 주문확인서출력시간 Print TimeStamp Orde | ordCnfdocPrtDts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordCnfdocPrtDts: 주문확인서출력시간 Print TimeStamp Order Confirmation Paper |
| 주문확인서출력처리자 Print Processor Ord | ordCnfdocPrtRegpeId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | ordCnfdocPrtRegpeId: 주문확인서출력처리자 Print Processor Order Confirmation Paper |
| 지점명 Sales store name | salestrNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | salestrNm: 지점명 Sales store name \| salestrNm: 지점명 Sales store name \| salestrNm: 지점명 Sales store name |
| 최종배송상세진행상태명 Final Shipping Detail Proces | lastShppProgStatDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | lastShppProgStatDtlNm: 최종배송상세진행상태명 Final Shipping Detail Process Status Name |
| 출고유형 상세코드 | shppDivDtlCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppDivDtlCd: 샘플코드에서 확인된 필드 |
| 출고주체 10 점포PP센터 20 구로통합물류센터 Release Wareh | whoutMainDivCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | whoutMainDivCds: 출고주체 10 점포PP센터 20 구로통합물류센터 Release Warehouse 10 Dept Release 20 Guro Warehouse |
| 층정보 01 지하5층 02 지하4층 03 지하3층 04 | dptsFloCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | dptsFloCd: 층정보 01 지하5층 02 지하4층 03 지하3층 04 지하2층 05 지하1층 06 지상1층 07 지상2층 27 지상3M층 08 지상3층 09 지상4층 10 지상5층 11 지상6층 12 지상7층 13 지상8층 14 지상9층 15 지상10층 16 지상11층 17 지상12층 18 B 지하2 19 B 지하1 20 B 지상1 21 B 지상2 22 B 지상3 23 B 지상4 24 B 지상5 25 B 지상6 26 B 지상7 Department Floor Code 01 지하5층 02 지하4층 03 지하3층 04 지하2층 05 지하1층 06 지상1층 07 지상2층 27 지상3M층 08 지상3층 09 지상4층 10 지상5층 11 지상6층 12 지상7층 13 지상8층 14 지상9층 15 지상10층 16 지상11층 17 지상12층 18 B 지하2 19 B 지하1 20 B 지상1 21 B 지상2 22 B 지상3 23 B 지상4 24 B 지상5 25 B 지상6 26 B 지상7 |
| 층정보 Sales store Floor | dptsFloNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | dptsFloNm: 층정보 Sales store Floor |
| 택배사 Shipping Company Name | delicoVenNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | delicoVenNm: 택배사 Shipping Company Name \| delicoVenNm: 택배사 Shipping Company Name |
| 판매가 | sellprc | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | sellprc: Integer \| sellprc: 샘플코드에서 확인된 필드 \| sellprc: Integer |
| 피킹완료일시 Process Date at Picking | pickgCmplDts | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | pickgCmplDts: 피킹완료일시 Process Date at Picking Complete |
| 피킹완료처리자 Processor Picking Comp | pickgCmplRegpeId | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | pickgCmplRegpeId: 피킹완료처리자 Processor Picking Complete |
| 피킹지시일 Process Date at Picking  | pickgDircDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | pickgDircDt: 피킹지시일 Process Date at Picking Direction |
| 하위업체명 Low Rand Vendor | lrnkSplVenNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | lrnkSplVenNm: 하위업체명 Low Rand Vendor \| lrnkSplVenNm: 하위업체명 Low Rand Vendor \| lrnkSplVenNm: 하위업체명 Low Rand Vendor |
| 환불여부 Refund Yes Or No | refundYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | refundYn: 환불여부 Refund Yes Or No |
| 환불여부 Y/N Refund Yes Or No Y/N | refundYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | refundYn: 환불여부 Y/N Refund Yes Or No Y/N \| refundYn: 환불여부 Y/N Refund Yes Or No Y/N |
| 환불처리여부 Refund Yes Or No | refundYn | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | refundYn: 환불처리여부 Refund Yes Or No |
| 회수상태 63 회수확인 64 회수완료 65 회수완료보류 66 회수철회 R | shppProgStatDtlCds | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | shppProgStatDtlCds: 회수상태 63 회수확인 64 회수완료 65 회수완료보류 66 회수철회 Recollect Status 63 Recollect Confirmed 64 Recollect Completed 65 Recollect Completed On Hold 66 Recollect Revoked |
| 회수상태 Recollect Status | lastShppProgStatDtlNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | lastShppProgStatDtlNm: 회수상태 Recollect Status \| lastShppProgStatDtlNm: 회수상태 Recollect Status |
| 회수신청방법 Recollect Request Method | rcovMthdNm | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcovMthdNm: 회수신청방법 Recollect Request Method \| rcovMthdNm: 회수신청방법 Recollect Request Method |
| 회수완료보류사유 Reasons for pending c | rcovHoldCd | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcovHoldCd: 회수완료보류사유 Reasons for pending collection completion |
| 회수완료보류일 Recollect Completion O | rcovCmplDeferDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcovCmplDeferDt: 회수완료보류일 Recollect Completion On Hold Date |
| 회수완료일 Recollect Completed Date | rcovCmplDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcovCmplDt: 회수완료일 Recollect Completed Date |
| 회수지시일 Recollect Instructed Dat | rcovDircDt | 백화점 배송 | 1 | 단일 | ✅ 핵심 UDS | rcovDircDt: 회수지시일 Recollect Instructed Date \| rcovDircDt: 회수지시일 Recollect Instructed Date |
