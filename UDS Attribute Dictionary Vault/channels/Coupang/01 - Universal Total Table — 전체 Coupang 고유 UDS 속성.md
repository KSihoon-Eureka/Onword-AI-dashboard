---
title: Universal Total Table — 전체 Coupang 고유 UDS 속성
channel: Coupang
type: notion-table-migration
source_notion_page_id: 369559dfde8580268fb8d1216cd0e1f0
source_table_id: 369559df-de85-81d8-90f4-c971b0229899
rows_including_header: 652
csv_backup: ../../_csv/Coupang/01 - Universal Total Table — 전체 Coupang 고유 UDS 속성.csv
---

# Universal Total Table — 전체 Coupang 고유 UDS 속성

- Channel: [[Coupang Index|Coupang]]
- Rows including header: **652**
- CSV backup: `../../_csv/Coupang/01 - Universal Total Table — 전체 Coupang 고유 UDS 속성.csv`

| UDS 속성명 | Coupang 필드명 | API 카테고리 | 사용 API 문서 수 | 공통/반복 | 설명 |
| --- | --- | --- | --- | --- | --- |
| 10원 | PRICE | 쿠폰 / 캐시백 APIs | 2 |  | 10원 단위 금액 |
| 19세이상 | ADULT_ONLY | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 19세이상 구입 가능 상품 |
| 4자 | z | 물류센터 APIs | 5 |  | 4자 |
| Attribute | Attribute | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Description |
| CJ대한통운 | CJGLS | 물류센터 APIs | 1 |  | CJ대한통운 |
| CODE | CODE | CS APIs, 물류센터 APIs, 반품 APIs, 쿠폰 / 캐시백 APIs | 12 | 공통 | MEANING |
| COUPANG | COUPANG | 반품 APIs | 2 |  | COUPANG |
| CS_CENTER | CS_CENTER | 교환 APIs | 1 |  | CS |
| CS_CONFIRM | CS_CONFIRM | 반품 APIs | 2 |  | CS_CONFIRM |
| CS_LOSS_CONFIRM | CS_LOSS_CONFIRM | 반품 APIs | 2 |  | CS_LOSS_CONFIRM |
| CUSTOMER | CUSTOMER | 반품 APIs | 2 |  | CUSTOMER |
| GENERAL | GENERAL | 반품 APIs | 2 |  | GENERAL |
| HTML | HTML | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | HTML |
| Item | Item | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Description |
| Key | Key | 로켓그로스 APIs, 상품 APIs | 4 | 공통 |  |
| MANDATORY | MANDATORY | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 필수 |
| None | None | 배송 / 환불 APIs | 1 |  | None |
| OK | OK | 쿠폰 / 캐시백 APIs | 3 |  | OK |
| OPTIONAL | OPTIONAL | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 선택 |
| Pagination | Pagination | 쿠폰 / 캐시백 APIs | 13 |  | Array |
| RETURN | RETURN | 반품 APIs | 1 |  |  |
| ReceiptMap | ReceiptMap | 배송 / 환불 APIs | 1 |  | Object |
| STATUS | STATUS | 배송 / 환불 APIs | 2 |  | MEANING |
| UNDEFINED | UNDEFINED | 반품 APIs | 2 |  | UNDEFINED |
| VENDOR | VENDOR | 반품 APIs | 2 |  | VENDOR |
| VENDOR_CONFIRM | VENDOR_CONFIRM | 반품 APIs | 2 |  | VENDOR_CONFIRM |
| Value | Value | 반품 APIs | 2 |  | Value |
| WMS | WMS | 반품 APIs | 2 |  | WMS |
| ableSplitShipping | ableSplitShipping | 배송 / 환불 APIs | 4 |  | Boolean |
| action | action | 쿠폰 / 캐시백 APIs | 1 |  | expire |
| additionalInformation | additionalInformation | 로켓그로스 APIs | 1 |  |  |
| additionalInformationForRocketGrowth | additionalInformationForRocketGrowth | 로켓그로스 APIs | 2 |  |  |
| addressType | addressType | 물류센터 APIs | 4 |  | String |
| adultOnly | adultOnly | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| allowedOfferConditions | allowedOfferConditions | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | Array |
| amountInStock | amountInStock | 상품 APIs | 1 |  | Number |
| answeredAt | answeredAt | CS APIs | 1 |  | String |
| attributeTypeName | attributeTypeName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| attributeTypename | attributeTypename | 로켓그로스 APIs, 상품 APIs | 2 | 공통 |  |
| attributeValueName | attributeValueName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| attributeValuename | attributeValuename | 로켓그로스 APIs, 상품 APIs | 2 | 공통 |  |
| attributes | attributes | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 6 | 공통 | Array |
| autoCategorizationPredictionResultType | autoCategorizationPredictionResultType | 카테고리 APIs | 1 |  | String |
| barcode | barcode | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| body | body | 쿠폰 / 캐시백 APIs | 2 |  |  |
| brand | brand | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | String |
| bundleInfo | bundleInfo | 상품 APIs | 1 |  | Map<String,String> |
| bundleType | bundleType | 상품 APIs | 2 |  | String |
| buyerEmail | buyerEmail | CS APIs | 1 |  | String |
| buyerPhone | buyerPhone | CS APIs | 1 |  | String |
| cancelCountSum | cancelCountSum | 반품 APIs | 2 |  | Number |
| cancelId | cancelId | 반품 APIs | 2 |  | Number |
| cancelReason | cancelReason | 교환 APIs, 반품 APIs | 3 | 공통 | String |
| cancelReasonCategory1 | cancelReasonCategory1 | 반품 APIs | 2 |  | String |
| cancelReasonCategory2 | cancelReasonCategory2 | 반품 APIs | 2 |  | String |
| categoryId | categoryId | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Number |
| cdnPath | cdnPath | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| certificationAttachments | certificationAttachments | 로켓그로스 APIs, 상품 APIs | 4 | 공통 |  |
| certificationCode | certificationCode | 로켓그로스 APIs, 상품 APIs | 4 | 공통 |  |
| certificationType | certificationType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 |  |
| certifications | certifications | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 6 | 공통 | Array |
| child | child | 로켓그로스 APIs, 카테고리 APIs | 3 | 공통 | String |
| collectCompleteDate | collectCompleteDate | 교환 APIs | 1 |  | String |
| collectInformationsDto | collectInformationsDto | 교환 APIs | 1 |  | Object |
| collectStatus | collectStatus | 교환 APIs | 1 |  | String |
| comment | comment | 상품 APIs, 카테고리 APIs | 2 | 공통 | String |
| companyContactNumber | companyContactNumber | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 8 | 공통 | String |
| completeConfirmDate | completeConfirmDate | 반품 APIs | 2 |  | String |
| completeConfirmType | completeConfirmType | 반품 APIs | 2 |  | String |
| consumerCashFee02kg | consumerCashFee02kg | 물류센터 APIs | 2 |  | Number |
| consumerCashFee05kg | consumerCashFee05kg | 물류센터 APIs | 4 |  | Number |
| consumerCashFee10kg | consumerCashFee10kg | 물류센터 APIs | 4 |  | Number |
| consumerCashFee20kg | consumerCashFee20kg | 물류센터 APIs | 4 |  | Number |
| content | content | CS APIs, 로켓그로스 APIs, 상품 APIs, 쿠폰 / 캐시백 APIs | 20 | 공통 | Object |
| contentDetails | contentDetails | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| contents | contents | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | List |
| contentsType | contentsType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| contractCustomerNumber | contractCustomerNumber | 물류센터 APIs | 1 |  | String |
| contractNumber | contractNumber | 물류센터 APIs | 1 |  | String |
| countPerPage | countPerPage | 물류센터 APIs | 1 |  | Number |
| countryCode | countryCode | 물류센터 APIs | 2 |  | String |
| couponFailedVendorItemIdResponses | couponFailedVendorItemIdResponses | 쿠폰 / 캐시백 APIs | 1 |  | Array |
| couponId | couponId | 쿠폰 / 캐시백 APIs | 3 |  | Integer |
| createAt | createAt | 물류센터 APIs | 2 |  | String |
| createDate | createDate | 물류센터 APIs | 1 |  | Object |
| createdBy | createdBy | 상품 APIs | 1 |  | String |
| createdByType | createdByType | 교환 APIs | 1 |  | String |
| createdByTypeLabel | createdByTypeLabel | 교환 APIs | 1 |  | String |
| csPartnerCounselingStatus | csPartnerCounselingStatus | CS APIs | 1 |  | String |
| currentPage | currentPage | 물류센터 APIs | 1 |  | Number |
| dateFrom | dateFrom | 반품 APIs | 1 |  | 조회 시작일 (yyyy-MM-dd) |
| dateTo | dateTo | 반품 APIs | 1 |  | 조회 종료일 (yyyy-MM-dd) |
| deliverCode | deliverCode | 물류센터 APIs | 3 |  | String |
| deliverName | deliverName | 물류센터 APIs | 3 |  | String |
| deliveredDate | deliveredDate | 배송 / 환불 APIs | 4 |  | String |
| deliveryCharge | deliveryCharge | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| deliveryChargeOnReturn | deliveryChargeOnReturn | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| deliveryChargeType | deliveryChargeType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| deliveryCode | deliveryCode | 물류센터 APIs | 2 |  | String |
| deliveryCompanyCode | deliveryCompanyCode | 로켓그로스 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs | 7 | 공통 | String |
| deliveryCompanyName | deliveryCompanyName | 배송 / 환불 APIs | 4 |  | String |
| deliveryFee | deliveryFee | 정산 APIs | 1 |  | Object |
| deliveryInvoiceGroupDtos | deliveryInvoiceGroupDtos | 교환 APIs | 1 |  | Array |
| deliveryInvoiceModifiable | deliveryInvoiceModifiable | 교환 APIs | 1 |  | Boolean |
| deliveryMethod | deliveryMethod | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| deliveryStatus | deliveryStatus | 교환 APIs | 1 |  | String |
| description | description | 쿠폰 / 캐시백 APIs | 2 |  | String |
| disabled | disabled | 쿠폰 / 캐시백 APIs | 1 |  | boolean |
| disabledAt | disabledAt | 쿠폰 / 캐시백 APIs | 1 |  | String |
| discount | discount | 쿠폰 / 캐시백 APIs | 2 |  | Number |
| displayCategoryCode | displayCategoryCode | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 9 | 공통 | String |
| displayProductName | displayProductName | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | String |
| documentPath | documentPath | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| emptyBarcode | emptyBarcode | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Boolean |
| emptyBarcodeReason | emptyBarcodeReason | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| enclosePrice | enclosePrice | 반품 APIs | 2 |  | Object |
| endAt | endAt | 쿠폰 / 캐시백 APIs | 1 |  | String |
| errorMessage | errorMessage | 물류센터 APIs | 2 |  | String |
| estimatedShippingDate | estimatedShippingDate | 배송 / 환불 APIs | 2 |  | String |
| exchangeAddressDtoV1 | exchangeAddressDtoV1 | 교환 APIs | 1 |  | Object |
| exchangeAmount | exchangeAmount | 교환 APIs | 1 |  | String |
| exchangeId | exchangeId | 교환 APIs | 1 |  | Number |
| exchangeItemDtoV1s | exchangeItemDtoV1s | 교환 APIs | 1 |  | Array |
| exchangeStatus | exchangeStatus | 교환 APIs | 1 |  | String |
| exchangeStatusLabel | exchangeStatusLabel | 교환 APIs | 1 |  | String |
| exposed | exposed | 상품 APIs | 1 |  |  |
| externalSkuId | externalSkuId | 로켓그로스 APIs | 1 |  | String |
| externalVendorSku | externalVendorSku | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| extraInfoMessage | extraInfoMessage | 로켓그로스 APIs, 상품 APIs | 3 | 공통 | String |
| extraProperties | extraProperties | 로켓그로스 APIs, 배송 / 환불 APIs, 상품 APIs | 8 | 공통 | Object |
| failVendorItemIds | failVendorItemIds | 쿠폰 / 캐시백 APIs | 1 |  | Array |
| failed | failed | 쿠폰 / 캐시백 APIs | 1 |  | Number |
| failedItemIds | failedItemIds | 배송 / 환불 APIs | 1 |  | Array |
| false | false | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 3 | 공통 | false |
| faultByType | faultByType | 반품 APIs | 2 |  | String |
| faultType | faultType | 교환 APIs | 1 |  | String |
| faultTypeLabel | faultTypeLabel | 교환 APIs | 1 |  | String |
| finalSettlementDate | finalSettlementDate | 정산 APIs | 1 |  | String |
| freeShipOverAmount | freeShipOverAmount | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| generalProductName | generalProductName | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | String |
| global | global | 물류센터 APIs | 1 |  | 기본값: false 국내(domestic) or 해외(overseas) CODE Mean false 국내(domestic) true 해외(overseas) |
| goodsflowStatus | goodsflowStatus | 물류센터 APIs | 2 |  | String |
| imageOrder | imageOrder | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| imageType | imageType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| images | images | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | List |
| inTrasitDateTime | inTrasitDateTime | 배송 / 환불 APIs | 4 |  | String |
| inquiryAt | inquiryAt | CS APIs | 1 |  | String |
| inquiryStatus | inquiryStatus | CS APIs | 1 |  | String |
| inventoryDetails | inventoryDetails | 로켓그로스 APIs | 1 |  |  |
| invoiceNumber | invoiceNumber | 반품 APIs, 배송 / 환불 APIs | 7 | 공통 | String |
| invoiceNumberId | invoiceNumberId | 반품 APIs | 1 |  | Number |
| isAllowSingleItem | isAllowSingleItem | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | Boolean |
| isCod | isCod | 배송 / 환불 APIs | 4 |  | Boolean |
| isExpirationDateRequiredForRocketGrowth | isExpirationDateRequiredForRocketGrowth | 로켓그로스 APIs | 1 |  | Boolean |
| itemIndex | itemIndex | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | ItemIndex = 0 as element index position of items List |
| itemName | itemName | CS APIs, 로켓그로스 APIs, 상품 APIs | 5 | 공통 | String |
| items | items | 로켓그로스 APIs, 상품 APIs, 정산 APIs | 4 | 공통 | Array |
| jeju | jeju | 물류센터 APIs | 2 |  | Number |
| legalAgreement | legalAgreement | 로켓그로스 APIs | 2 |  | String |
| managedCode | managedCode | 쿠폰 / 캐시백 APIs | 1 |  | String |
| manufacture | manufacture | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | String |
| marketplaceItemData | marketplaceItemData | 로켓그로스 APIs | 2 |  |  |
| marketplaceShippingAndReturnInfo | marketplaceShippingAndReturnInfo | 로켓그로스 APIs | 1 |  |  |
| maxAmount | maxAmount | 쿠폰 / 캐시백 APIs | 2 |  | 최대적립금액 최소값은 0 FIXED 혹은 FIXED_WITH_QUANTITY 선택 시 파라미터 입력 불필요 |
| maxDiscountPrice | maxDiscountPrice | 쿠폰 / 캐시백 APIs | 1 |  | 최대할인금액 최소 10원 이상 |
| maximumBuyCount | maximumBuyCount | 로켓그로스 APIs, 상품 APIs | 3 | 공통 | Number |
| maximumBuyForPerson | maximumBuyForPerson | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| maximumBuyForPersonPeriod | maximumBuyForPersonPeriod | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| maximumDiscountPrice | maximumDiscountPrice | 쿠폰 / 캐시백 APIs | 2 |  | Number |
| maximumPerDaily | maximumPerDaily | 쿠폰 / 캐시백 APIs | 2 |  | Number |
| minimumPrice | minimumPrice | 쿠폰 / 캐시백 APIs | 2 |  | Number |
| modelNo | modelNo | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| modifiedAt | modifiedAt | 교환 APIs, 반품 APIs | 3 | 공통 | String |
| modifiedByType | modifiedByType | 교환 APIs | 1 |  | String |
| modifiedByTypeLabel | modifiedByTypeLabel | 교환 APIs | 1 |  | String |
| notJeju | notJeju | 물류센터 APIs | 2 |  | Number |
| noticeCategories | noticeCategories | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | Array |
| noticeCategoryDetailName | noticeCategoryDetailName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| noticeCategoryName | noticeCategoryName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| notices | notices | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | List |
| offerCondition | offerCondition | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| offerDescription | offerDescription | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| onSale | onSale | 상품 APIs | 1 |  | Boolean |
| orderDate | orderDate | CS APIs | 1 |  | String |
| orderDeliveryStatusCode | orderDeliveryStatusCode | 교환 APIs | 1 |  | String |
| orderDeliveryStatusLabel | orderDeliveryStatusLabel | 교환 APIs | 1 |  | String |
| orderItems | orderItems | 로켓그로스 APIs, 배송 / 환불 APIs | 6 | 공통 | Array |
| orderedAt | orderedAt | 배송 / 환불 APIs | 4 |  | String |
| originalPrice | originalPrice | 상품 APIs | 2 |  | Number |
| outboundShippingPlaceCode | outboundShippingPlaceCode | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 5 | 공통 | Number |
| outboundShippingTimeDay | outboundShippingTimeDay | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| overseaShippingInfoDto | overseaShippingInfoDto | 배송 / 환불 APIs | 4 |  | Object |
| overseasPurchased | overseasPurchased | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| pagination | pagination | CS APIs | 2 |  | Object |
| paidAt | paidAt | 로켓그로스 APIs, 배송 / 환불 APIs | 6 | 공통 | String |
| parallelImported | parallelImported | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| parcelPrintMessage | parcelPrintMessage | 배송 / 환불 APIs | 4 |  | String |
| paymentId | paymentId | 반품 APIs | 2 |  | Number |
| pccNeeded | pccNeeded | 로켓그로스 APIs, 상품 APIs | 5 | 공통 | Boolean |
| permittedCount | permittedCount | 상품 APIs | 1 |  | Number |
| phoneNumber2 | phoneNumber2 | 물류센터 APIs | 4 |  | String |
| placeAddresses | placeAddresses | 물류센터 APIs | 3 |  | Array |
| preRefund | preRefund | 반품 APIs | 2 |  | Boolean |
| preSplitShipped | preSplitShipped | 배송 / 환불 APIs | 2 |  | Boolean |
| predictedCategoryId | predictedCategoryId | 카테고리 APIs | 1 |  | String |
| predictedCategoryName | predictedCategoryName | 카테고리 APIs | 1 |  | String |
| priceData | priceData | 로켓그로스 APIs | 2 |  | O |
| productGroup | productGroup | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | String |
| publishedDate | publishedDate | 쿠폰 / 캐시백 APIs | 1 |  |  |
| reason | reason | 교환 APIs, 쿠폰 / 캐시백 APIs | 2 | 공통 | String |
| reasonCode | reasonCode | 교환 APIs, 반품 APIs | 3 | 공통 | String |
| reasonCodeText | reasonCodeText | 교환 APIs, 반품 APIs | 3 | 공통 | String |
| reasonEtcDetail | reasonEtcDetail | 교환 APIs | 1 |  | String |
| receiptCategory | receiptCategory | CS APIs | 1 |  | String |
| receiptId | receiptId | 반품 APIs | 3 |  | Number |
| receiptStatus | receiptStatus | 반품 APIs | 2 |  | String |
| receiptType | receiptType | 반품 APIs | 2 |  | String |
| recognitionDate | recognitionDate | 정산 APIs | 1 |  | String |
| refer | refer | 배송 / 환불 APIs | 4 |  | String |
| referType | referType | 교환 APIs | 1 |  | String |
| referTypeLabel | referTypeLabel | 교환 APIs | 1 |  | String |
| refundDeliveryDuty | refundDeliveryDuty | 반품 APIs | 2 |  | String |
| regNumber | regNumber | 반품 APIs | 1 |  | String |
| registeredCount | registeredCount | 상품 APIs | 1 |  | Number |
| rejectable | rejectable | 교환 APIs | 1 |  | Boolean |
| releaseStopStatus | releaseStopStatus | 반품 APIs | 2 |  | String |
| remoteArea | remoteArea | 배송 / 환불 APIs | 4 |  | Boolean |
| remoteAreaDeliverable | remoteAreaDeliverable | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| remoteInfoId | remoteInfoId | 물류센터 APIs | 1 |  | Number |
| remoteInfos | remoteInfos | 물류센터 APIs | 1 |  | Array |
| remotePrice | remotePrice | 배송 / 환불 APIs | 4 |  | Object |
| replies | replies | CS APIs | 1 |  | Array |
| requestTransactionId | requestTransactionId | 쿠폰 / 캐시백 APIs | 1 |  | String |
| requested | requested | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Boolean |
| requestedId | requestedId | 쿠폰 / 캐시백 APIs | 1 |  | String |
| requesterAddress | requesterAddress | 반품 APIs | 2 |  | String |
| requesterAddressDetail | requesterAddressDetail | 반품 APIs | 2 |  | String |
| requesterName | requesterName | 반품 APIs | 2 |  | String |
| requesterPhoneNumber | requesterPhoneNumber | 반품 APIs | 2 |  | String |
| requesterRealPhoneNumber | requesterRealPhoneNumber | 반품 APIs | 2 |  | String |
| requesterZipCode | requesterZipCode | 반품 APIs | 2 |  | String |
| requiredDocumentNames | requiredDocumentNames | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | Array |
| requiredDocuments | requiredDocuments | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | List |
| responseCode | responseCode | 배송 / 환불 APIs | 3 |  | Number |
| responseKey | responseKey | 배송 / 환불 APIs | 1 |  | Number |
| responseList | responseList | 배송 / 환불 APIs | 3 |  | Array |
| responseMessage | responseMessage | 배송 / 환불 APIs | 3 |  | String |
| restricted | restricted | 상품 APIs | 1 |  | Boolean |
| resultCode | resultCode | 교환 APIs, 물류센터 APIs, 배송 / 환불 APIs | 8 | 공통 | String |
| resultMessage | resultMessage | 교환 APIs, 물류센터 APIs, 배송 / 환불 APIs | 8 | 공통 | String |
| returnAddress | returnAddress | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 8 | 공통 | String |
| returnAddressDetail | returnAddressDetail | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 8 | 공통 | String |
| returnCenterCode | returnCenterCode | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 6 | 공통 | String |
| returnCharge | returnCharge | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| returnChargeName | returnChargeName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| returnDeliveryDtos | returnDeliveryDtos | 교환 APIs, 반품 APIs | 3 | 공통 | Object |
| returnDeliveryId | returnDeliveryId | 반품 APIs | 3 |  | Number |
| returnDeliveryType | returnDeliveryType | 반품 APIs | 2 |  | String |
| returnExchangeDeliveryType | returnExchangeDeliveryType | 반품 APIs | 1 |  | String |
| returnFee02kg | returnFee02kg | 물류센터 APIs | 2 |  | Number |
| returnFee05kg | returnFee05kg | 물류센터 APIs | 4 |  | Number |
| returnFee10kg | returnFee10kg | 물류센터 APIs | 4 |  | Number |
| returnFee20kg | returnFee20kg | 물류센터 APIs | 4 |  | Number |
| returnItems | returnItems | 반품 APIs | 2 |  | Array |
| returnShippingCharge | returnShippingCharge | 반품 APIs | 2 |  | Object |
| returnZipCode | returnZipCode | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 8 | 공통 | String |
| rfmInboundName | rfmInboundName | 로켓그로스 APIs | 2 |  | String |
| rocketGrowthItemData | rocketGrowthItemData | 로켓그로스 APIs | 2 |  |  |
| ruleId | ruleId | 쿠폰 / 캐시백 APIs | 1 |  | Number |
| saleDate | saleDate | 정산 APIs | 1 |  | String |
| saleEndedAt | saleEndedAt | CS APIs, 로켓그로스 APIs, 상품 APIs | 7 | 공통 | String |
| salePrice | salePrice | 상품 APIs | 3 |  | Number |
| saleStartedAt | saleStartedAt | CS APIs, 로켓그로스 APIs, 상품 APIs | 7 | 공통 | String |
| saleType | saleType | 정산 APIs | 1 |  | String |
| salesCountMap | salesCountMap | 로켓그로스 APIs | 1 |  |  |
| sameDayShipping | sameDayShipping | 상품 APIs | 2 |  | Object |
| searchTags | searchTags | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | List |
| sellerItemId | sellerItemId | 상품 APIs | 1 |  | Number |
| sellerProductItemId | sellerProductItemId | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Number |
| settlementDate | settlementDate | 정산 APIs | 1 |  | String |
| shipmentType | shipmentType | 배송 / 환불 APIs | 4 |  | String |
| shippingPlaceName | shippingPlaceName | 물류센터 APIs | 3 |  | String |
| shippingPrice | shippingPrice | 배송 / 환불 APIs | 4 |  | Object |
| skuInfo | skuInfo | 로켓그로스 APIs | 2 |  |  |
| splitShipping | splitShipping | 배송 / 환불 APIs | 6 |  | Boolean |
| startAt | startAt | 쿠폰 / 캐시백 APIs | 1 |  | String |
| statusName | statusName | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | String |
| succeeded | succeeded | 쿠폰 / 캐시백 APIs | 1 |  | Number |
| success | success | 쿠폰 / 캐시백 APIs | 13 |  | Boolean |
| successVendorItemIds | successVendorItemIds | 쿠폰 / 캐시백 APIs | 1 |  | Array |
| successable | successable | 교환 APIs | 1 |  | Boolean |
| targetMonth | targetMonth | 쿠폰 / 캐시백 APIs | 1 |  | 조회하고자 하는 예산월 yyyy-MM targetMonth를 입력하지 않으면 현재 월에 해당하는 예산이 조회됨. |
| taxType | taxType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| templateName | templateName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| title | title | 쿠폰 / 캐시백 APIs | 2 |  | String |
| total | total | 쿠폰 / 캐시백 APIs | 1 |  | Number |
| totalElements | totalElements | 물류센터 APIs | 1 |  | Number |
| totalPages | totalPages | 물류센터 APIs | 1 |  | Number |
| true | true | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 3 | 공통 | true |
| type | type | 쿠폰 / 캐시백 APIs | 3 |  | couponItemId |
| typeOfDiscount | typeOfDiscount | 쿠폰 / 캐시백 APIs | 2 |  | String |
| unionDeliveryType | unionDeliveryType | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| unitCount | unitCount | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | Number |
| usable | usable | 물류센터 APIs | 4 |  | Boolean |
| userId | userId | 쿠폰 / 캐시백 APIs | 2 |  | String |
| value | value | 쿠폰 / 캐시백 APIs | 1 |  | Number |
| valueType | valueType | 쿠폰 / 캐시백 APIs | 1 |  | String |
| vendorCashFee02kg | vendorCashFee02kg | 물류센터 APIs | 2 |  | Number |
| vendorCashFee05kg | vendorCashFee05kg | 물류센터 APIs | 4 |  | Number |
| vendorCashFee10kg | vendorCashFee10kg | 물류센터 APIs | 4 |  | Number |
| vendorCashFee20kg | vendorCashFee20kg | 물류센터 APIs | 4 |  | Number |
| vendorCreditFee02kg | vendorCreditFee02kg | 물류센터 APIs | 2 |  | Number |
| vendorCreditFee05kg | vendorCreditFee05kg | 물류센터 APIs | 4 |  | Number |
| vendorCreditFee10kg | vendorCreditFee10kg | 물류센터 APIs | 4 |  | Number |
| vendorCreditFee20kg | vendorCreditFee20kg | 물류센터 APIs | 4 |  | Number |
| vendorDocumentPath | vendorDocumentPath | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | String |
| vendorItemIds | vendorItemIds | 반품 APIs, 쿠폰 / 캐시백 APIs | 3 | 공통 | Array |
| vendorPath | vendorPath | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | O |
| vendorUserId | vendorUserId | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | String |
| x | x | 물류센터 APIs | 5 |  | 2~4자 |
| y | y | 물류센터 APIs | 5 |  | 3~4자 |
| 가격 | forceSalePriceUpdate, price | 상품 APIs | 1 |  | 가격 변경 비율 제한 여부 false(default 값) or true (가격 변경 비율 제한 없음) 입력 실수 방지를 위해 기존 가격 대비 변경할 수 있는 가격 비율 제한함. forceSalePriceUpdate=true 를 추가해서 가격변경 요청 시 처리 가능함. |
| 값 | NONE | 교환 APIs | 1 |  | 값 없음 |
| 개인통관부호) | pccNeeded | 상품 APIs | 1 |  | PCC(개인통관부호) 필수/비필수 여부 해외구매대행 상품인 경우, 상품 PCC(개인통관번호) - 기본값 : 비필수(false) true 고객이 PCC 입력 후 구매 가능 (PCC는 발주서에 포함 됨) false 고객이 PCC를 입력하지 않고 상품 구매 가능 |
| 거절원인코드 | exchangeRejectCode | 교환 APIs | 1 |  | 거절원인코드 노트: 교환거절코드는"SOLDOUT" 또는 "WITHDRAW"만 입력할 수 있습니다 SOLDOUT : 교환할수있지만 아이템이 매진되였습니다. WITHDRAW :교환요청이 철회되였습니다 (고객님이 요청함) |
| 검색 | paidDateFrom, paidDateTo | 로켓그로스 APIs | 1 |  | 검색 종료일시 yyyymmdd 형태로 조회하기 원하는 종료 날짜 기입 ex) 20240709 최대 30일까지 조회 가능합니다. |
| 검색옵션 | NONE | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 검색옵션 |
| 결과 메시지 | message | CS APIs, 교환 APIs, 로켓그로스 APIs, 물류센터 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 89 | 공통 | 성공 혹은 실패에 따른 결과 메시지 200: OK 206: Partial successfully 400: Bad request , will show corresponding bad request message 500: Internal error |
| 결과를 | requestTransactionId, requestedId | 쿠폰 / 캐시백 APIs | 2 |  | 결과를 조회할 ID |
| 결과없음 | NONE | 배송 / 환불 APIs | 2 |  | 결과없음 |
| 결과코드 | code | CS APIs, 교환 APIs, 로켓그로스 APIs, 물류센터 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 89 | 공통 | Http request status code Example: 200, 400, 500 |
| 결재완료 | ACCEPT | 교환 APIs | 1 |  | 결재완료 |
| 결제완료 | ACCEPT | 배송 / 환불 APIs | 5 |  | 결제완료 |
| 고객 | CUS, CUSTOMER | 교환 APIs, 반품 APIs | 3 | 공통 | 고객 |
| 고객과실 | CUSTOMER | 교환 APIs | 1 |  | 고객과실 |
| 고객이 | false, true | 로켓그로스 APIs, 상품 APIs | 5 | 공통 | 고객이 PCC 입력 후 구매 가능 (PCC는 발주서에 포함 됨) |
| 과세 | TAX | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 과세 (기본값) |
| 교환 | exchangeId | 교환 APIs | 3 |  | 교환 접수번호 *교환 요청 목록 조회 API를 이용해서 확인할 수 있습니다. |
| 교환배송 | EXCHANGE_DELIVERY | 교환 APIs | 1 |  | 교환배송 |
| 교환배송철회 | Withdraw | 교환 APIs | 1 |  | 교환배송철회 |
| 교환재고없음 | CHANGE_SEND_FAIL | 교환 APIs | 1 |  | 교환재고없음(미발송) |
| 교환정보 | CHANGE_SEND_COMPLETE | 교환 APIs | 1 |  | 교환정보 전송완료 |
| 교환확정 | CHANGE_SEND_READY | 교환 APIs | 1 |  | 교환확정 |
| 교환확정홀드 | CHANGE_SEND_HOLD | 교환 APIs | 1 |  | 교환확정홀드(교환확정에서 철회될 경우 변경되는 코드) |
| 교환회수철회 | Withdraw | 교환 APIs | 1 |  | 교환회수철회 |
| 구매대행 | AGENT_BUY, NOT_OVERSEAS_PURCHASED, OVERSEAS_PURCHASED | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 구매대행 아님 (기본값) |
| 구매옵션 | EXPOSED | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 구매옵션 |
| 구비 | requiredDocuments | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 구비 서류 필수인 경우 입력 구비서류는 5MB이하의 파일 입력 가능 (PDF, HWP, DOC, DOCX, TXT, PNG, JPG, JPEG) |
| 국내 | false, global | 물류센터 APIs | 2 |  | 국내 혹은 해외 CODE Mean false 국내(domestic) true 해외(overseas) |
| 굿스플로 | goodsflowInfoDto | 물류센터 APIs | 1 |  | 굿스플로 택배 연동 정보 |
| 권한이 | PERMISSION_DENIED | 배송 / 환불 APIs | 2 |  | 권한이 없습니다. |
| 기본배송비 | deliveryCharge | 상품 APIs | 3 |  | 기본배송비 유료배송 또는 조건부 무료배송 시, 편도 배송비 금액 입력 |
| 기준출고일 | outboundShippingTimeDay | 상품 APIs | 1 |  | 기준출고일(일) 주문일(D-Day) 이후 배송을 위한 출고예정일자를 '일' 단위로 입력. (당일출고를 하는 경우 '1'을 입력하세요.다음날(D+1) 출고일 경우 '1' 입력하시기 바랍니다.) |
| 기타 | ETC | 교환 APIs | 1 |  | 기타 |
| 날짜 | DATE | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 날짜 |
| 내부직원 | COUPANG | 교환 APIs | 1 |  | 내부직원 |
| 노출상품명 | displayProductName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 노출상품명 실제 쿠팡 판매페이지에서 노출되는 상품명. [ brand ]+[ generalProductName ]과 동일하게 입력할 것을 권장, 미입력 상태로도 등록 가능 미입력 시 [ brand ]+[ generalProductName ]이 노출되거나, [ sellerProductName ]이 노출될 수 있음 최대 길이 : 100 자 |
| 노출카테고리코드 | displayCategoryCode | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 8 | 공통 | 노출카테고리코드 카테고리 목록 조회 API 또는 카테고리 정보 excel 을 다운받아 노출카테고리코드 확인 가능 ※ 미입력 시, 카테고리 자동매칭 서비스에 의해 자동으로 카테고리가 등록될 수 있습니다. 자세한 사항은 여기 를 확인하세요. |
| 다운로드 | couponId, expireCouponList | 쿠폰 / 캐시백 APIs | 2 |  | 다운로드 쿠폰ID (쿠폰 생성 시 Response로 확인) |
| 다음 | nextPageIndex, pageIndex, token | 반품 APIs, 정산 APIs | 2 | 공통 | 다음 페이지 조회를 위한 token값 다음 페이지를 호출하기 위한 토큰값 (첫 페이지 조회 시에는'token='까지만 입력) |
| 다음 페이지 토큰 | nextToken | 교환 APIs, 로켓그로스 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs | 10 | 공통 | 결과 문자열 목록은 다음 결과 페이지를 가져오는 데 사용됩니다. nextToken이 반환되면 nextToken 값이 다음 요청으로 전달됩니다. nextToken이 반환되지 않으면 더 이상 반환할 내용이 없습니다. |
| 다음페이지에 | hasNext | 정산 APIs | 1 |  | 다음페이지에 데이터 존재 여부 |
| 답변 | content | CS APIs | 2 |  | 답변 내용 최소 2 ~ 최대 1,000자까지 입력 가능 줄넘김을 위해서는 \n를 사용하시기 바랍니다. |
| 답변 상태 | answeredType | CS APIs | 1 |  | 답변 상태 Name Status ALL 전체보기 ANSWERED 답변완료 NOANSWER 미답변 |
| 답변완료 | ANSWER, ANSWERED | CS APIs | 2 |  | 답변완료 |
| 대기 | WAIT | 교환 APIs | 1 |  | 대기 |
| 대기중 | STANDBY | 쿠폰 / 캐시백 APIs | 6 |  | 대기중 |
| 도로명 | ROADNAME | 물류센터 APIs | 6 |  | 도로명 |
| 도서산간 | N, Y, remoteAreaDeliverable, remoteInfos | 로켓그로스 APIs, 물류센터 APIs, 상품 APIs | 10 | 공통 | 도서산간 배송여부 Parameter Name Status Y 도서산간 배송 N 도서산간 배송안함 |
| 동일한 | vendorItemIds | 쿠폰 / 캐시백 APIs | 1 |  | 동일한 캐시백 룰을 적용하려는 옵션 ID 목록 최대 적립할 수 있는 옵션 ID 개수는 50개 필수값 |
| 등록상품 ID | sellerProductId | 로켓그로스 APIs, 상품 APIs | 13 | 공통 | 등록상품ID 상품 생성 완료 시, 출력 된 등록상품 아이디 (data) |
| 등록상품명 | itemName, sellerProductName | 로켓그로스 APIs, 상품 APIs | 10 | 공통 | 등록상품명 발주서에 사용되는 상품명 최대 길이 : 100 자 |
| 로젠택배 | KGB | 물류센터 APIs | 1 |  | 로젠택배 |
| 로켓와우회원한정 | true | 쿠폰 / 캐시백 APIs | 1 |  | 로켓와우회원한정 |
| 롯데택배 | HYUNDAI | 물류센터 APIs | 1 |  | 롯데택배 |
| 리퍼 | REFURBISHED | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 6 | 공통 | 리퍼 |
| 마켓플레이스 | marketplaceShippingAndReturnInfo | 로켓그로스 APIs | 1 |  | 마켓플레이스 아이템을 생성하려면 배송 및 반품 정보가 필요합니다. 로켓그로스의 경우 쿠팡이 배송 및 반품을 담당하므로 본 내용은 로켓그로스 등록상품 생성 시에는 유효하지 않을 수 있습니다. |
| 매출인식 | recognitionDateFrom, recognitionDateTo | 정산 APIs | 1 |  | 매출인식 시작일 최대 31일 이내로 입력 형식 : YYYY-MM-dd |
| 매출인식시작일 | revenueRecognitionDateFrom | 정산 APIs | 1 |  | 매출인식시작일 |
| 매출인식월 | revenueRecognitionYearMonth | 정산 APIs | 1 |  | 매출인식월 형식 : YYYY-MM |
| 매출인식종료일 | revenueRecognitionDateTo | 정산 APIs | 1 |  | 매출인식종료일 |
| 무료배송 | FREE | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 무료배송 |
| 무료배송을 | freeShipOverAmount | 상품 APIs | 3 |  | 무료배송을 위한 조건 금액 ● 예시 : 10,000원 이상 조건부 무료배송을 설정하기 원할 경우 [deliveryChargeType]을 'CONDITIONAL_FREE'로 설정 후, [freeShipOverAmount]에 10000을 입력 ※ 100원 이상 단위로 입력 가능 ※ 무료배송인 경우, 0 입력 |
| 묶음 | NOT_UNION_DELIVERY, UNION_DELIVERY, unionDeliveryType | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 묶음 배송여부 Parameter Name Status UNION_DELIVERY 묶음 배송 가능 NOT_UNION_DELIVERY 묶음 배송 불가능 ※ 묶음 배송 조건 출고지 정보 필수 입력 (출고지 정보가 같은 상품만 묶음 배송 가능) 착불배송 불가 설정 불가 |
| 문의 | partnerCounselingStatus | CS APIs | 1 |  | 문의 상태 Name Status NONE 전체 ANSWER 답변완료 NO_ANSWER 미답변 : 판매자의 답변이 필요한 상태 TRANSFER 미확인 : 쿠팡이 상담완료한 업체이관 건으로 판매자의 확인이 필요한 상태, 답변은 필요없음 |
| 문의 ID | inquiryId | CS APIs | 4 |  | Inquiry ID 판매자가 어느 질문을 확인해야할 지를 입력합니다. 먼저 쿠팡 고객센터 문의조회 API를 사용하여 미확인 상태(TRANSFER)인 inquiry 값을 확인합니다. |
| 문의 조회시작일 | inquiryStartAt | CS APIs | 2 |  | 조회시작일, 형식: yyyy-MM-dd 1. vendorItemId가 null인 경우, 반드시 이 파라미터를 입력하여 조회합니다. 해당 조회시작일과 종료일 기간의 모든 상담리스트를 조회할 수 있습니다.(inquiryEndAt - inquiryStartAt = 7d) 2. vendorItemId 값 입력이 있을 경우 이 파라미터는 입력하지 않아도 조회가 가능합니다. a. 조회시작일과 조회종료일이 null인 경우, 해당 vendorItemId의 모든 상담리스트를 조회할수있습니다. b. 조회시작일과 조회종료일 값이 있을 경우 해당 기간의 모든 상담리스트를 조회할수있습니다. |
| 문의 조회종료일 | inquiryEndAt | CS APIs | 2 |  | 조회종료일, 형식: yyyy-MM-dd |
| 문자열 | STRING | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 문자열 |
| 물류과실 | WMS | 교환 APIs | 1 |  | 물류과실 |
| 미답변 | NOANSWER, NO_ANSWER | CS APIs | 2 |  | 미답변 : 판매자의 답변이 필요한 상태 |
| 미출고 | N, NOT_RELEASED | 교환 APIs, 반품 APIs | 3 | 공통 | 미출고 |
| 미확인 | TRANSFER | CS APIs | 1 |  | 미확인 : 쿠팡이 상담완료한 업체이관 건으로 판매자의 확인이 필요한 상태, 답변은 필요없음 |
| 반품 | REFUND, receiptId, returnExchangeDeliveryType | 반품 APIs, 정산 APIs | 2 | 공통 | 반품 또는 교환 접수ID 반품요청 목록조회, 교환요청 목록조회 API를 통해 확인가능 receiptId는 반드시 number 타입이어야 합니다. |
| 반품배송비 | returnCharge | 상품 APIs | 3 |  | 반품배송비 반품회수시 편도 배송비 *초도반품배송비와 비교 시, 100~150%까지만 입력 가능 |
| 반품완료 | CC, RETURNS_COMPLETED | 반품 APIs | 2 |  | 반품완료 |
| 반품요청 | searchType | 반품 APIs | 1 |  | 반품요청 목록 조회를 분단위로 조회 시에는 "searchType=timeFrame"파라메터를 전송하여야 합니다. |
| 반품접수 | RETURNS_UNCHECKED, UC, cancelCount | 반품 APIs | 3 |  | 반품접수 수량 |
| 반품접수번호 | receiptId | 반품 APIs | 2 |  | 반품접수번호 (취소번호는 지원되지 않습니다) ReceiptId는 반품요청 목록 조회API를 통해 확인가능합니다. ReceiptId는 반드시 number타입이어야 합니다. |
| 반품주문 | RETURN, cancelType | 반품 APIs | 1 |  | code description RETURN 반품주문조회 (default) CANCEL 취소주문조회 default 값은 RETURN 이며, 취소주문을 조회할 경우에는 status 파라메터를 제거해야 합니다. |
| 반품지 | placeAddresses, returnCenterCode, returnCenterCodes, shippingPlaceName | 물류센터 APIs | 3 |  | 반품지 센터코드 일괄 조회가능한 returnCenterCodes의 최대 개수는 100. 예) 1000554021,1000554704 |
| 반품지담당자명 | returnChargeName | 상품 APIs | 1 |  | 반품지담당자명 쿠팡 Wing 또는 반품지 생성 API를 통해 반품지 등록 후 확인 |
| 반품지명 | returnChargeName | 상품 APIs | 2 |  | 반품지명 쿠팡 Wing 또는 반품지 조회 API를 통해 반품지 등록 후 확인 '반품지 조회 시, shippingPlaceName로 노출되는 값 입력' |
| 반품지센터코드 | returnCenterCode | 상품 APIs | 3 |  | 반품지센터코드 반품지 생성 후, 추출 된 반품지 센터코드를 입력 ● 반품지 생성은 Wing 또는 반품지 생성 API를 통해 가능 ● 반품지 생성이 불가능한 경우, "NO_RETURN_CENTERCODE"를 입력하여 직접 반품지 정보 등록 가능 ※ 반품자동연동 서비스(굿스플로우)는 계약한 택배사가 있어야만 이용이 가능하며, 반품지 센터코드 입력 필수 ※ 해외 배송 상품은 반드시 국내 반품지 주소지와 계약된 택배사 코드를 입력하여 반품지 센터 코드를 생성해주시기바랍니다. *해외 배송 상품 반품지 가이드(Click) |
| 반품지연락처 | companyContactNumber | 상품 APIs | 3 |  | 반품지연락처 쿠팡 Wing 또는 반품지 조회 API를 통해 반품지 등록 후 확인 |
| 반품지우편번호 | returnZipCode | 상품 APIs | 3 |  | 반품지우편번호 쿠팡 Wing 또는 반품지 생성 API를 통해 반품지 등록 후 확인 |
| 반품지주소 | returnAddress | 상품 APIs | 3 |  | 반품지주소 쿠팡 Wing 또는 반품지 생성 API를 통해 반품지 등록 후 확인 |
| 반품지주소상세 | returnAddressDetail | 상품 APIs | 3 |  | 반품지주소상세 쿠팡 Wing 또는 반품지 생성 API를 통해 반품지 등록 후 확인 |
| 발행 | wowExclusive | 쿠폰 / 캐시백 APIs | 1 |  | 발행 대상 쿠폰을 사용할 수 있는 대상 false 전체고객 (기본값) true 로켓와우회원한정 일반 다운로드 쿠폰은 false로 생성해주시기 바랍니다. true는 로켓와우 회원을 대상으로 골드박스 등 기획전에 선정된 상품에 대해 적용하는 값이며, 상품에 적용 시 사전 승인이 필요합니다. |
| 발행중지 | PAUSED | 쿠폰 / 캐시백 APIs | 6 |  | 발행중지 |
| 배송 | marketplaceShippingAndReturnInfo | 로켓그로스 APIs | 1 |  | 배송 및 반품 정보는 마켓플레이스 아이템에 대해서만 수정할 수 있습니다 . |
| 배송방법 | deliveryMethod | 상품 APIs | 3 |  | 배송방법 Parameter Name Status SEQUENCIAL 일반배송 (순차배송) COLD_FRESH 신선냉동 MAKE_ORDER 주문제작 AGENT_BUY 구매대행 VENDOR_DIRECT 설치배송 또는 판매자 직접 전달 “INSTRUCTURE”와 “MAKE_ORDER_DIRECT”는 “VENDOR_DIRECT”로 통합되었습니다. |
| 배송번호 | shipmentBoxId | 교환 APIs, 배송 / 환불 APIs | 9 | 공통 | 배송번호 재배송을 위한 배송번호 입고확인 처리 후 교환요청목록 조회 시 deliveryInvoiceGroupDtos 정보 아래에, 새로 생성된 shipmentBoxId를 입력해야합니다. |
| 배송비종류 | deliveryChargeType | 상품 APIs | 3 |  | 배송비종류 Parameter Name Status FREE 무료배송 NOT_FREE 유료배송 CHARGE_RECEIVED 착불배송 CONDITIONAL_FREE 조건부 무료배송 ● 무료배송 설정 시 초도반품배송비(편도)[deliveryChargeOnReturn]와, 반품배송비(편도)[returnCharge] 금액 설정 ● 유료배송 설정 시 기본배송비[deliveryCharge]와 반품배송비(편도) 금액 설정 ● 조건부 무료배송 설정 시 기본배송비와 반품배송비(편도) 금액 설정 ● 착불배송 설정 시 착불배송 가능 카테고리는 따로 정리되어 있으며, 판매자 안내를 위해 판매자콜센터에 공유가 되었습니다. ※ [CONDITIONAL_FREE] 사용 시, 원하는 조건부 무료배송 금액을 별도로 설정할 수 있습니다. |
| 배송실패 | Fail | 교환 APIs | 1 |  | 배송실패 |
| 배송연동 | BeforeDirection, CompleteDirection | 교환 APIs | 1 |  | 배송연동 전 |
| 배송연동실패 | DirectionFail | 교환 APIs | 1 |  | 배송연동실패 |
| 배송완료 | CompleteDelivery, FINAL_DELIVERY | 교환 APIs, 배송 / 환불 APIs | 6 | 공통 | 배송완료 |
| 배송중 | DELIVERING, Delivering | 교환 APIs, 배송 / 환불 APIs | 6 | 공통 | 배송중 |
| 배송지시 | DEPARTURE, orderSheetInvoiceApplyDtos | 교환 APIs, 배송 / 환불 APIs | 8 | 공통 | 배송지시 상태로 변경할 대상 정보 목록 |
| 배송진행상태가 | INVALID_STATUS | 배송 / 환불 APIs | 2 |  | 배송진행상태가 유효하지 않습니다. |
| 배송추적 | TRACKING | 교환 APIs | 1 |  | 배송추적 |
| 번들상품 | bundleInfo | 상품 APIs | 2 |  | 번들상품 |
| 벤더 | VENDOR | 교환 APIs | 1 |  | 벤더 |
| 병행수입 | NOT_PARALLEL_IMPORTED, PARALLEL_IMPORTED | 로켓그로스 APIs, 상품 APIs | 5 | 공통 | 병행수입 아님 (기본값) |
| 보류 | RESERVE, pendingReleasedAmount | 교환 APIs, 정산 APIs | 2 | 공통 | 보류(해제)금액 보류가 해제 되면서 이번 지급에 포함될 금액 |
| 부모이관글 | parentAnswerId | CS APIs | 1 |  | 부모이관글 ID(answerId) 쿠팡 고객센터 문의 조회API에서 조회한 answerId 를 입력해야 됩니다. |
| 부분승인완료 | PARTIAL_APPROVED | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 부분승인완료 |
| 부분실패 | PARTIAL_ERROR | 배송 / 환불 APIs | 2 |  | 부분실패 |
| 분리배송 | IS_SEPARATE_MUST_BE_TRUE_WHEN_SEPARATE_DELIVERY | 배송 / 환불 APIs | 2 |  | 분리배송 접수 후 일반배송으로 처리 할 수 없습니다. 분리배송 여부를 Y로 수정하시기 바랍니다. |
| 불가 | REJECT | 교환 APIs | 1 |  | 불가 |
| 브랜드 | brand | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 5 | 공통 | 브랜드 브랜드명은 한글/영어 표준이름 입력 띄어쓰기 및 특수문자 없이 입력 |
| 비과세 | FREE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 비과세 |
| 비정상반품완료 | RETURN_COLLECT_NOT_OK | 교환 APIs | 1 |  | 비정상반품완료(수량불일치 등) |
| 사용 | DISABLED, usable | 로켓그로스 APIs, 물류센터 APIs, 카테고리 APIs | 5 | 공통 | 사용 가능 여부 사용하지 않는 반품지를 사용안함처리 할 수 있습니다. 단 해당 반품지를 사용하고 있는 상품 정보도 함께 수정해주셔야 합니다. 사용가능 true 사용안함 false |
| 사용가능 | ENABLE, true | 교환 APIs, 물류센터 APIs | 2 | 공통 | 사용가능 |
| 사용가능여부 | usable | 물류센터 APIs | 1 |  | 사용가능여부 true 사용가능 false 사용불가 기본값 : true |
| 사용불가 | DISABLE, false | 교환 APIs, 물류센터 APIs | 2 | 공통 | 사용불가 |
| 사용자 | userId | 물류센터 APIs, 쿠폰 / 캐시백 APIs | 5 | 공통 | 사용자 아이디(쿠팡 WING 로그인 계정) |
| 사용종료 | EXPIRED | 쿠폰 / 캐시백 APIs | 6 |  | 사용종료 |
| 사용중 | APPLIED | 쿠폰 / 캐시백 APIs | 6 |  | 사용중 |
| 상담사 | COUNSELOR | 교환 APIs | 1 |  | 상담사 |
| 상세 메시지 | details | 로켓그로스 APIs, 배송 / 환불 APIs, 상품 APIs | 3 | 공통 | 에러 및 경고 상황에 대해 상세 설명되어 있습니다. |
| 상태 | status | 교환 APIs, 로켓그로스 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 16 | 공통 | 발주서 상태 Parameter Name Status ACCEPT 결제완료 INSTRUCT 상품준비중 DEPARTURE 배송지시 DELIVERING 배송중 FINAL_DELIVERY 배송완료 NONE_TRACKING 업체 직접 배송(배송 연동 미적용), 추적불가 |
| 상품 | couponItems | 쿠폰 / 캐시백 APIs | 1 |  | 상품 쿠폰적용을 위한 데이터 |
| 상품 ID | productId | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Number |
| 상품군 | productGroup | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 상품군 상품의 종류를 나타내는 명칭으로 노출카테고리의 최하위명을 참고하여 입력 가능. 제품명[ generalProductName ]과 중복될 경우, 입력 불필요 |
| 상품등록 | ettorItems | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | 상품등록 실패가 될 수 있는 상품이 나열되어져 있습니다. Item Type Description itemIndex Integer ItemIndex = 0 as element index position of items List itemName String 등록상품명 attributes List <Attribute> Attribute Type Description attributeTypename String attributeValuename String message String 유효하지 않은 데이터 타입, 단위 |
| 상품명 | productName | 카테고리 APIs | 1 |  | 상품명 |
| 상품삭제 | DELETED | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 상품삭제 |
| 상품속성정보 | attributes | 카테고리 APIs | 1 |  | 상품속성정보 (예 : 사이즈, 색상, 소재 등) |
| 상품에 | productDescription | 카테고리 APIs | 1 |  | 상품에 대한 상세설명 |
| 상품이 | NOT_ALLOW_SEPARATE_WHEN_ONE_VENDOR_ITEM | 배송 / 환불 APIs | 2 |  | 상품이 한가지인 경우 분리배송 할 수 없습니다. |
| 상품정보 검증이 필요한 상품 (노출제한) MOTA | ViolationTypeSearchField | 상품 APIs | 1 |  | NO_VA_V2: 상품정보 검증이 필요한 상품 (노출제한) MOTA_V2: 누락된 필수 구매옵션을 입력해야하는 상품 (노출제한) ATTR: 옵션 수정이 필요한 상품 (노출낮음) |
| 상품준비중 | INSTRUCT, shipmentBoxIds | 교환 APIs, 배송 / 환불 APIs | 7 | 공통 | 상품준비중 상태로 변경할 묶음배송번호 목록 최대 50개 까지만 요청 요망 |
| 새 | NEW | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 6 | 공통 | 새 상품 |
| 생성 시작일시 | createdAtFrom | 교환 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs | 5 | 공통 | 검색 시작일시（ ISO-8601 표준을 준수해야 합니다.） yyyy-mm-ddT00:00%2B09:00 형태로 조회하기 원하는 시작 날짜 및 시각 기입 ex) 2025-07-29T01:23%2B09:00 |
| 생성 종료일시 | createdAtTo | 교환 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs | 5 | 공통 | 검색 종료일시（ ISO-8601 표준을 준수해야 합니다.） yyyy-mm-ddT00:00 형태로 조회하기 원하는 종료 날짜 및 시각 기입 ex) 2025-07-29T15:50%2B09:00 해당 일자 내 24시간이내로 조회 가능합니다. |
| 생성일시 | createdAt | 교환 APIs, 로켓그로스 APIs, 반품 APIs, 상품 APIs | 10 | 공통 | 상품등록일시 "yyyy-MM-dd" 형식 예)2015-12-17과 같이 입력하면, 2015-12-17T00:00:00 ~ 2015-12-17T23:59:59 와 같이 조회됨 |
| 서버 응답 메세지와 동일한 값) | httpStatusMessage | 쿠폰 / 캐시백 APIs | 13 |  | HTTP Status Message (서버 응답 메세지와 동일한 값) |
| 서버 응답 코드와 동일한 값) | httpStatus | 쿠폰 / 캐시백 APIs | 13 |  | HTTP Status Code(서버 응답 코드와 동일한 값) |
| 서비스 | READY | 로켓그로스 APIs, 카테고리 APIs | 3 | 공통 | 서비스 준비중 |
| 서비스중 | ACTIVE | 로켓그로스 APIs, 카테고리 APIs | 3 | 공통 | 서비스중 |
| 설명 | ViolationTypeAndOr | 상품 APIs | 1 |  | 설명: "ViolationTypeSearchField" 필드에 2개 이상의 파라미터를 입력하는 경우 필수입니다. 값: AND OR |
| 설치배송 | VENDOR_DIRECT | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 설치배송 또는 판매자 직접 전달 |
| 성공 | DONE, OK, SUCCESS | 배송 / 환불 APIs, 쿠폰 / 캐시백 APIs | 3 | 공통 | 성공 |
| 셀러 | storeFeeDiscount | 정산 APIs | 1 |  | 셀러 스토어 이용료 할인 금액 |
| 속성 | INPUT, SELECT | 카테고리 APIs | 1 |  | 속성 값은 dataType 값과 단위를 조합하여 직접 입력한 값으로 정의할 수 있습니다. |
| 송장번호 | invoiceNumber | 배송 / 환불 APIs | 1 |  | 송장번호 |
| 송장번호가 | INVALID_INVOICE_NUMBER | 배송 / 환불 APIs | 2 |  | 송장번호가 유효하지 않습니다. |
| 수량 | quantity | 상품 APIs | 1 |  | 재고수량 |
| 수정하려는 | outboundShippingPlaceCode | 물류센터 APIs | 1 |  | 수정하려는 출고지 코드 |
| 수취인 | receiver | 배송 / 환불 APIs | 4 |  | Object |
| 숫자 | NUMBER | 로켓그로스 APIs, 카테고리 APIs | 2 | 공통 | 숫자 |
| 승인대기중 | APPROVING | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 승인대기중 |
| 승인반려 | DENIED | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 승인반려 |
| 승인완료 | APPROVED | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 승인완료 |
| 시작일 | startAt | 쿠폰 / 캐시백 APIs | 1 |  | 시작일 yyyy-MM-ddTHH:mm:ss 현재 시간보다 최소 2시간 이후로 적용 가능 (현시간 오후 2시 일 경우, startAt은 오후 4시 이후로 설정 가능) |
| 신선냉동 | COLD_FRESH | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 신선냉동 |
| 실사용자ID | confirmBy, replyBy | CS APIs | 2 |  | 실사용자ID(쿠팡 Wing ID) 업체(Vendor)에 소속된 사용자ID |
| 실사용자아이디 | vendorUserId | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 실사용자아이디(쿠팡 WING 아이디) 업체(Vendor)에 소속된 사용자아이디 |
| 실패 | FAIL, FAILED | 배송 / 환불 APIs, 쿠폰 / 캐시백 APIs | 3 | 공통 | 실패 |
| 심사중 | IN_REVIEW | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 심사중 |
| 아이템 | DETACHED | 쿠폰 / 캐시백 APIs | 3 |  | 아이템 파기 |
| 알수없는 | UNDEFINED_ERROR_OCCUR | 배송 / 환불 APIs | 2 |  | 알수없는 오류 |
| 업체 | COM, NONE_TRACKING, VENDOR | 교환 APIs, 반품 APIs, 배송 / 환불 APIs | 8 | 공통 | 업체 직접 배송(배송 연동 미적용), 추적불가 |
| 업체과실 | VENDOR | 교환 APIs | 1 |  | 업체과실 |
| 업체상품옵션목록 | items | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 업체상품옵션목록 최대 200개 옵션 등록 가능 |
| 업체의 | contractId, userId | 배송 / 환불 APIs, 쿠폰 / 캐시백 APIs | 5 | 공통 | 업체의 계약서 아이디 (자유계약의 경우 -1 입력) |
| 업체전달완료 | CompleteCollect | 교환 APIs | 1 |  | 업체전달완료 |
| 업체직송 | VendorDirect | 교환 APIs | 1 |  | 업체직송 |
| 업체직송은 | NOT_ALLOW_VENDOR_DIRECT | 배송 / 환불 APIs | 2 |  | 업체직송은 분리배송 할 수 없습니다. |
| 없음 | NONE | CS APIs | 2 |  | 없음 |
| 에러 | errorMessage | 쿠폰 / 캐시백 APIs | 2 |  | 에러 상세내용 |
| 에러발생 | errorCode | 쿠폰 / 캐시백 APIs | 2 |  | 에러발생 시 분류 |
| 예금주 | bankAccountHolder | 정산 APIs | 1 |  | 예금주 |
| 오류 | ERROR | 교환 APIs | 1 |  | 오류 |
| 옵션 ID | vendorItemId | CS APIs, 로켓그로스 APIs, 배송 / 환불 APIs, 상품 APIs, 쿠폰 / 캐시백 APIs | 18 | 공통 | 옵션 ID 1. 조회시작일과 조회종료일이 null인 경우, 이 파라미터를 사용해야만 해당 vendorItemId 아래의 모든 상담리스트를 조회할 수 있습니다. 2. 조회시작일과 조회종료일 값이 있을 경우 이 파라미터는 입력할 필요 없습니다. |
| 완료 | SUCCESS | 교환 APIs | 1 |  | 완료 |
| 요청됨 | REQUESTED | 쿠폰 / 캐시백 APIs | 1 |  | 요청됨 |
| 우체국 | EPOST | 물류센터 APIs | 1 |  | 우체국 |
| 운송장번호 | invoiceNumber | 교환 APIs, 반품 APIs, 배송 / 환불 APIs | 3 | 공통 | 운송장번호 |
| 월 | MONTHLY | 정산 APIs | 1 |  | 월 정산 내역 |
| 웹 | WEB_MOBILE, WEB_PC | 교환 APIs | 1 |  | 웹 모바일 |
| 유료배송 | NOT_FREE | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 유료배송 |
| 유효시작일 | startAt | 쿠폰 / 캐시백 APIs | 1 |  | 유효시작일 유효시작일은 다음날 00시부터 작동하도록 설정 가능 ex: 8월4일 15시에 쿠폰을 생성한다면 8월5일00시 부터 쿠폰이 적용되도록 생성 |
| 유효종료일 | endAt | 쿠폰 / 캐시백 APIs | 1 |  | 유효종료일 |
| 유효하지 않은 데이터 타입 | attributes | 로켓그로스 APIs, 상품 APIs | 2 | 공통 | Attribute Type Description attributeTypename String attributeValuename String message String 유효하지 않은 데이터 타입, 단위 |
| 은행명 | bankName | 정산 APIs | 1 |  | 은행명 |
| 을 제외한 나머지 Status 에서 서버 내 상세한 실패 | errorMessage | 쿠폰 / 캐시백 APIs | 1 |  | HTTP Status 200을 제외한 나머지 Status 에서 서버 내 상세한 실패 이유 메세지가 담깁니다. |
| 을 제외한 나머지 Status에서 서버 내 상세한 실패 | errorMessage | 쿠폰 / 캐시백 APIs | 12 |  | HTTP Status 200을 제외한 나머지 Status에서 서버 내 상세한 실패 이유 메세지가 담깁니다. |
| 응답 데이터 | data | CS APIs, 교환 APIs, 로켓그로스 APIs, 물류센터 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 79 | 공통 | 캐시백 룰 성공 적용시 옵션목록으로 반환됨;실패시 실패원인 메세지 반환. |
| 응답자 | replyBy | CS APIs | 1 |  | 응답자 셀러포탈(WING) 아이디 |
| 이관취소 | CANCEL | CS APIs | 2 |  | 이관취소 |
| 이름 | name | 로켓그로스 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 4 | 공통 | 프로모션명(최대 45자) |
| 이면 발주서 목록 | searchType | 배송 / 환불 APIs | 2 |  | search type for order sheets results searchType=timeFrame이면 발주서 목록 조회(분단위 전체)로 수행되며, 그 외에는 발주서 목록 조회(일단위 페이징)로 수행됩니다. |
| 이미 | DUPLICATE_INVOICE_NUMBER, NOT_ALLOW_INVOICE_NUMBER_RE_UPLOAD, NOT_FOUND_INVOICE_NUMBER, RELEASED | 교환 APIs, 배송 / 환불 APIs | 3 | 공통 | 이미 저장된 송장번호가 있어, 송장번호 등록이 불가능합니다. (동일송장번호 업로드 조건 : 주문자/수취인정보 동일) |
| 이미지 | IMAGE, IMAGE_NO_SPACE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 이미지(공백없음) |
| 이미지-이미지 | IMAGE_IMAGE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 이미지-이미지 |
| 이미지-텍스트 | IMAGE_TEXT | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 이미지-텍스트 |
| 이미출고 | RELEASED | 교환 APIs | 1 |  | 이미출고 |
| 이미출고됨 | A | 반품 APIs | 2 |  | 이미출고됨 |
| 이미회수 | ALREADY_RETURN | 교환 APIs | 1 |  | 이미회수 |
| 일반 | GENERAL | 교환 APIs | 1 |  | 일반 |
| 일반배송 | DELIVERY, NOT_ALLOW_SEPARATE_AFTER_NORMAL_DELIVERY, SEQUENCIAL | 교환 APIs, 로켓그로스 APIs, 배송 / 환불 APIs, 상품 APIs | 9 | 공통 | 일반배송 접수 후 분리배송을 다시 할 수 없습니다. |
| 일양택배 | ILYANG | 물류센터 APIs | 1 |  | 일양택배 |
| 임시저장 | SAVED | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 임시저장 |
| 입고완료 | VENDOR_WAREHOUSE_CONFIRM | 반품 APIs | 2 |  | 입고완료 |
| 자동승인요청여부 | requested | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 자동승인요청여부 상품 등록 시, 자동으로 판매승인요청을 진행할지 여부 선택 ● false : 작성 내용만 저장하고 판매요청 전 상태 (판매를 원할 시에는 상품 승인요청 API 또는 wing에서 판매요청을 진행 해야 함) ● true : 저장 및 자동으로 판매 승인 요청 |
| 적립액 | value | 쿠폰 / 캐시백 APIs | 1 |  | 적립액 최소값은 1 |
| 적용할 | couponId | 쿠폰 / 캐시백 APIs | 1 |  | 적용할 쿠폰ID |
| 전담택배비 | dedicatedDeliveryAmount | 정산 APIs | 1 |  | 전담택배비 사용안함 |
| 전송완료 | RETURN_SEND_COMPLETE | 교환 APIs | 1 |  | 전송완료 |
| 전연령 | EVERYONE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 전연령 구입 가능 상품 (기본값) |
| 전주채권 | debtOfLastWeek | 정산 APIs | 1 |  | 전주채권 전주에 발생한 손실 관련 차감액 |
| 전체 | NONE | CS APIs | 1 |  | 전체 |
| 전체고객 | false | 쿠폰 / 캐시백 APIs | 1 |  | 전체고객 (기본값) |
| 전체보기 | ALL | CS APIs | 1 |  | 전체보기 |
| 접수 | RECEIPT, RETURN_SEND_READY, receiptId | 교환 APIs, 배송 / 환불 APIs | 3 | 공통 | 접수 ID |
| 정렬값 | sort | 쿠폰 / 캐시백 APIs | 2 |  | 정렬값 (asc, desc) 기본값 ascending |
| 정률할인 | RATE | 쿠폰 / 캐시백 APIs | 2 |  | 정률할인 |
| 정보가 제공되지 않습니다 | TRUE | 로켓그로스 APIs | 1 |  | SKU 정보가 제공되지 않습니다. |
| 정보없음 | NoneData | 교환 APIs | 1 |  | 정보없음 |
| 정산 | settlementDate | 정산 APIs | 1 |  | 정산(예정)일 |
| 정산대금 | bankAccount | 정산 APIs | 1 |  | 정산대금 입금 계좌번호 **뒤 4자리 마스킹 처리 |
| 정산대상액 | settlementTargetAmount | 정산 APIs | 1 |  | 정산대상액 =총판매액-판매수수료 |
| 정산유형 | settlementType | 정산 APIs | 1 |  | 정산유형 Parameter Name Status MONTHLY 월 정산 내역 WEEKLY 주 정산 내역 ADDITIONAL 추가 지급 RESERVE 최종액 지급 |
| 정산차감 | deductionAmount | 정산 APIs | 1 |  | 정산차감 |
| 정상 | SEQUENCIAL | 로켓그로스 APIs | 2 |  | 정상 배송 ( 순차배송 ) |
| 정상반품완료 | RETURN_COLLECT_OK | 교환 APIs | 1 |  | 정상반품완료 |
| 정수 | RATE | 쿠폰 / 캐시백 APIs | 2 |  | 1~99 정수입력 |
| 정액할인 | PRICE | 쿠폰 / 캐시백 APIs | 2 |  | 정액할인 |
| 제목 | TITLE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 제목 |
| 제조사 | manufacture | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 제조사 정확한 제조사 정보를 기입할 수 없는 경우, [brand] 항목과 동일한 정보 입력 |
| 제품명 | generalProductName | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 제품명 구매옵션[ Attribute exposed ] 정보(사이즈, 색상 등) 를 포함하지 않는 상품명. 모델명 추가 기입 가능 |
| 조건부 | CONDITIONAL_FREE | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 조건부 무료배송 |
| 존재하지 | NOT_FOUND_SHIPMENT_BOX | 배송 / 환불 APIs | 2 |  | 존재하지 않는 송장번호입니다. |
| 종료일 | endAt | 쿠폰 / 캐시백 APIs | 1 |  | 종료일 yyyy-MM-ddTHH:mm:ss |
| 주 | WEEKLY | 정산 APIs | 1 |  | 주 정산 내역 |
| 주문 | SALE | 정산 APIs | 1 |  | 주문 건 |
| 주문번호 | orderId | CS APIs, 교환 APIs, 로켓그로스 APIs, 반품 APIs, 배송 / 환불 APIs, 정산 APIs, 쿠폰 / 캐시백 APIs | 18 | 공통 | 주문번호 status 파라메터를 제외하고 조회할 경우에는 orderId가 파라메터에 포함되어야 합니다. searchType=timeFrame일 경우 지원하지 않는 파라메터입니다. |
| 주문상품 | bigCancelCode, middleCancelCode | 배송 / 환불 APIs | 1 |  | 주문상품 취소 사유 중 중분류 사유 코드 CCTTER // 재고 연동 오류 : 재고 문제로 취소가 발생하는 경우 CCPNER // 제휴사이트 오류 : 주소 문제로 고객 배송지 생성 불가시 취소 되는 오류 CCPRER // 가격등재오류 : 양사간 상품 가격오류 발생시 취소 되는 오류 상품준비중 상태의 상품 취소(출고중지완료) 시에는 입력값과 상관없이 사유 카테고리가 각각 "배송불만", "품절"로 고정됩니다. 취소 상세 사유는 "파트너 API 강제 취소"로 기록됩니다. |
| 주문자 | orderer | 배송 / 환불 APIs | 4 |  | Object |
| 주문제작 | MAKE_ORDER, extraInfoMessage | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 주문제작 안내 메시지 배송 방법을 '주문제작'으로 선택했을 경우, 고객에게 안내할 메시지를 입력 |
| 중고 | USED_BEST, USED_GOOD, USED_NORMAL | 로켓그로스 APIs, 상품 APIs, 카테고리 APIs | 6 | 공통 | 중고(최상) |
| 지급 | DONE, SUBJECT | 정산 APIs | 1 |  | 지급 완료 |
| 지급액 | settlementAmount | 정산 APIs | 1 |  | 지급액 유형 정책 주정산 정산대상액의 70% 월정산 정산대상액의 100% |
| 지번 | JIBUN | 물류센터 APIs | 6 |  | 지번 |
| 직권처리 | DISPUTE_PROCESS | CS APIs | 2 |  | 직권처리 |
| 진행 | PROGRESS | 교환 APIs | 1 |  | 진행 |
| 착불배송 | CHARGE_RECEIVED | 로켓그로스 APIs, 상품 APIs | 8 | 공통 | 착불배송 |
| 철회 | CANCEL, cancelIds | 교환 APIs, 반품 APIs | 2 | 공통 | 철회 이력을 조회할 취소(반품)접수번호 목록 한 번에 최대 50개까지 cancelIds 조회가 가능합니다. cancelIds는 number 타입이어야 합니다. |
| 초도반품배송비 | deliveryChargeOnReturn | 상품 APIs | 3 |  | 초도반품배송비 무료배송인 경우 반품시 소비자가 지불하는 배송비 |
| 총판매액 | totalSale | 정산 APIs | 1 |  | 총판매액 =판매액+판매배송료-(취소액+취소배송료+할인쿠폰) |
| 최종액 | RESERVE, lastAmount | 정산 APIs | 1 |  | 최종액 ( 유보성격의 금액 ) 주정산 30% 유보금액 |
| 최종지급액 | finalAmount | 정산 APIs | 1 |  | 최종지급액 or 지급예정액 (최종적으로 셀러에게 입금될 금액) =지급액+보류(해제)금액 -(전담택배비+판매자서비스이용료+정산차감+전주채권+쿠런티이용료+쿠런티보상금+판매자할인쿠폰+스토어이용료할인금액) |
| 추가 | ADDITIONAL | 정산 APIs | 1 |  | 추가 지급 |
| 추가출고배송 | FORCED_DELIVERY | 교환 APIs | 1 |  | 추가출고배송 |
| 출고 | cancelCount | 배송 / 환불 APIs | 1 |  | 출고 수량 |
| 출고됨 | Y | 반품 APIs | 2 |  | 출고됨 |
| 출고시 | CANCEL_REQUEST_WHEN_DEPARTURE | 교환 APIs | 1 |  | 출고시 철회요청 |
| 출고예정일은 | PSD_NOT_ALLOW_TO_CHANGE | 배송 / 환불 APIs | 2 |  | 출고예정일은 최초 등록 이후 변경 할 수 없습니다. |
| 출고중지 | ORDER_DELIVERY_PARTIAL_STOP_REQUESTED, STOPPED | 교환 APIs, 배송 / 환불 APIs | 3 | 공통 | 출고중지 요청건입니다. |
| 출고중지됨 | S | 반품 APIs | 2 |  | 출고중지됨 |
| 출고중지요청 | RELEASE_STOP_UNCHECKED, RU | 반품 APIs | 2 |  | 출고중지요청 |
| 출고지 | content, outboundShippingPlaceCode, placeAddresses, placeCodes, shippingPlaceName | 물류센터 APIs | 3 |  | 출고지 코드 출고지 생성 시, Response 메시지로 노출되는 값 outboundShippingPlaceCode와 동일 |
| 출고지명 | placeNames | 물류센터 APIs | 1 |  | 출고지명 shippingPlaceName과 동일 |
| 출고지주소코드 | outboundShippingPlaceCode | 상품 APIs | 3 |  | 출고지주소코드 묶음 배송 선택할 경우 필수, 출고지 조회 API를 통해 조회 가능 해외구매대행(AGENT_BUY) 선택시 해외주소지만 입력가능함 |
| 취소 | receiptId | 반품 APIs | 1 |  | 취소(반품)접수번호 ReceiptId는 반품요청 목록 조회API를 통해 확인가능합니다. ReceiptId는 반드시 number타입이어야 합니다. |
| 취소대기상태의 | ORDER_DELIVERY_CANCELED_HOLDING_FOR_CANCEL | 배송 / 환불 APIs | 2 |  | 취소대기상태의 주문건입니다. |
| 취소된 | ORDER_DELIVERY_CANCELED | 배송 / 환불 APIs | 2 |  | 취소된 주문건입니다. or 출고 준비중 상태인경우-> 출고중지 요청건입니다. |
| 취소주문 | CANCEL | 반품 APIs | 1 |  | 취소주문조회 |
| 취소할 | receiptCounts, vendorItemIds | 배송 / 환불 APIs | 1 |  | 취소할 상품의 옵션 ID(vendorItemId) 배열 receiptCounts 와 쌍으로 입력 |
| 카테고리 | locale | 로켓그로스 APIs | 1 |  | 카테고리 이름의 언어 . 사용 가능한 언어는 en , zh -CN, kr 입니다 . locale 을 제공하지 않으면 기본적으로 카테고리 이름은 KR 로 표시됩니다 . |
| 카테고리의 | registrationType | 로켓그로스 APIs | 1 |  | 카테고리의 BusinessType . 등록 유형을 제공하지 않으면 기본적으로 모든 카테고리를 보여줍니다 . 입력할 수 있는 값은 RFM 과 CGF 입니다 . 로켓그로스 운영 카테고리의 경우 'RFM'을 입력하여 조회합니다. |
| 캐시백 | valueType | 쿠폰 / 캐시백 APIs | 1 |  | 캐시백 유형 FIXED_WITH_QUANTITY(수량별 정액할인), FIXED(정액할인) |
| 캐시백 관련 계약완료 후 제공받은 룰 아이디를 | ruleId | 쿠폰 / 캐시백 APIs | 3 |  | Rule ID 캐시백 관련 계약완료 후 제공받은 룰 아이디를 입력 |
| 쿠런티보상금 | couranteeCustomerReward | 정산 APIs | 1 |  | 쿠런티보상금 |
| 쿠런티이용료 | couranteeFee | 정산 APIs | 1 |  | 쿠런티이용료 |
| 쿠팡 | COU | 반품 APIs | 2 |  | 쿠팡 |
| 쿠팡과실 | COUPANG | 교환 APIs | 1 |  | 쿠팡과실 |
| 쿠팡확인요청 | PR, REQUEST_COUPANG_CHECK | 반품 APIs | 2 |  | 쿠팡확인요청 |
| 쿠폰 | appliedOptionCount, couponId, couponPolicies, couponType, policies, publishedDate, title, usageAmount | 쿠폰 / 캐시백 APIs | 3 |  | 쿠폰 세부정책 각 쿠폰은 최대 3개의 세부정책을 생성할 수 있습니다. 한 쿠폰에 서로다른 타입의 정책 생성불가 (ex: PRICE / PRICE => 가능, PRICE / RATE => 불가능 |
| 쿠폰ID | couponId | 쿠폰 / 캐시백 APIs | 4 |  | 쿠폰ID 쿠폰 아이템 생성 / 쿠폰삭제 & 조회 등에 사용 |
| 쿠폰상태 | couponStatus | 쿠폰 / 캐시백 APIs | 2 |  | 쿠폰상태 생성시에는 'STANDBY'로 노출 |
| 쿠폰생성 | COUPON_PUBLISH, lastModifiedBy, lastModifiedDate | 쿠폰 / 캐시백 APIs | 2 |  | 쿠폰생성(최종수정) 계정 |
| 쿠폰아이템 | COUPON_ITEM_EXPIRE | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰아이템 파기 |
| 쿠폰아이템ID | couponItemId | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰아이템ID |
| 쿠폰아이템생성 | COUPON_ITEM_PUBLISH | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰아이템생성 |
| 쿠폰유형 | couponType | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰유형(다운로드쿠폰은 'DOWNLOAD' 사용) |
| 쿠폰을 | vendorItems | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰을 적용할 옵션ID 한 번에 적용할 옵션ID 수는 10,000개를 초과할 수 없음 |
| 쿠폰적용 | endDate, startDate | 쿠폰 / 캐시백 APIs | 2 |  | 쿠폰적용 시작일 'YYYY-MM-DD HH:MM:SS' |
| 쿠폰파기 | COUPON_EXPIRE | 쿠폰 / 캐시백 APIs | 1 |  | 쿠폰파기 |
| 택배사 | deliveryCompanyCode, goodsDeliveryCode, goodsflowInfoOpenApiDto, regNumber | 교환 APIs, 물류센터 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs | 7 | 공통 | 택배사 회수번호 (회수번호 발행 시 입력) |
| 텍스트 | TEXT | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 텍스트 |
| 텍스트-이미지 | TEXT_IMAGE | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 텍스트-이미지 |
| 텍스트-텍스트 | TEXT_TEXT | 로켓그로스 APIs, 상품 APIs | 6 | 공통 | 텍스트-텍스트 |
| 파기할 | couponId | 쿠폰 / 캐시백 APIs | 1 |  | 파기할 쿠폰ID |
| 파라미터 사용 시 | O | 로켓그로스 APIs | 1 |  | "rocketGrowth" 파라미터 사용 시, 로켓그로스 상품 또는 마켓플레이스 및 로켓그로스 아이템이 모두 존재하는 Hybrid 상품 목록이 조회됩니다. 파라미터 미사용 시, 기존 형식에 따라 마켓플레이스 상품 또는 마켓플레이스 및 로켓그로스 아이템이 모두 존재하는 Hybrid 상품이 조회됩니다. |
| 판매수수료 | serviceFee | 정산 APIs | 1 |  | 판매수수료 =판매수수료+우대수수료 환급액 |
| 판매시작일시 | saleStartedAt | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 판매시작일시 " yyyy-MM-dd'T'HH:mm:ss " 형식 |
| 판매자 | downloadableCoupon, sellerDiscountCoupon | 정산 APIs | 1 |  | 판매자 할인쿠폰 (즉시할인쿠폰) |
| 판매자 ID | vendorId | CS APIs, 교환 APIs, 로켓그로스 APIs, 물류센터 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs, 카테고리 APIs, 쿠폰 / 캐시백 APIs | 67 | 공통 | 판매자 ID 쿠팡에서 업체에게 발급한 고유 코드. WING 로그인 후 확인 가능 예) A00012345 |
| 판매자 상품코드 | externalVendorSkuCode | 상품 APIs | 1 |  | 판매자 상품코드 (업체상품코드) |
| 판매자상품코드 | sellerSkuCode | 카테고리 APIs | 1 |  | 판매자상품코드(업체상품코드) |
| 판매자서비스이용료 | sellerServiceFee | 정산 APIs | 1 |  | 판매자서비스이용료(서버이용료) |
| 판매자확인 | DISPUTE_PROCESS_COMPLETE | CS APIs | 2 |  | 판매자확인 |
| 판매종료일시 | saleEndedAt | 로켓그로스 APIs, 상품 APIs | 4 | 공통 | 판매종료일시 " yyyy-MM-dd'T'HH:mm:ss " 형식, *2099 년 까지 길게 선택 가능 |
| 페이지 | size | 쿠폰 / 캐시백 APIs | 2 |  | 페이지 당 건수 |
| 페이지 번호 | page | 쿠폰 / 캐시백 APIs | 2 |  | 페이지. 기본값 0 다음 페이지를 호출하기 위한 키값. 첫 페이지 호출시에는 넣지 않거나 '0' 입력. 두 번째 페이지를 보려면 '1'을 입력합니다, 등등 |
| 페이지 크기 | pageSize | CS APIs, 물류센터 APIs | 4 | 공통 | 페이지당 최대 호출 수 Default=10, Max=50 ※ 입력하지 않을 경우, 디폴트 값인 10으로 처리 됩니다. |
| 페이지당 | sizePerPage | 반품 APIs | 1 |  | 페이지당 최대 조회 요청 값 기본값 : 10, 최대값 : 100 |
| 페이지당 건수 | maxPerPage | 교환 APIs, 로켓그로스 APIs, 반품 APIs, 배송 / 환불 APIs, 상품 APIs, 정산 APIs | 7 | 공통 | 페이지당 최대 조회 요청 값 default = 50 searchType=timeFrame일 경우 지원하지 않는 파라메터입니다. cancelType=CANCEL일 경우 요청한 maxPerPage보다 적은 수의 결과가 출력될 수 있습니다. |
| 페이징 | pagination | 물류센터 APIs | 1 |  | 페이징 |
| 폐기 | DEPOSE | 교환 APIs | 1 |  | 폐기 |
| 한진택배 | HANJIN | 물류센터 APIs | 1 |  | 한진택배 |
| 할인률 | discount | 쿠폰 / 캐시백 APIs | 1 |  | 할인률 |
| 할인방식 | type | 쿠폰 / 캐시백 APIs | 1 |  | 할인방식 RATE(정률할인), FIXED_WITH_QUANTITY(수량별 정액할인), PRICE(정액할인) |
| 할인율기준가 | originalPrice | 상품 APIs | 1 |  | 할인율기준가 0원 부터 최소 10원 단위로 입력 가능합니다. (1원 단위 입력 불가) |
| 합포장건 | NOT_FOUND_VENDOR_ITEM | 배송 / 환불 APIs | 2 |  | 합포장건 중 누락된 상품이 있습니다. |
| 해외 | OVERSEA, true | 물류센터 APIs | 3 |  | 해외(overseas) |
| 현재 페이지 번호 | pageNum | CS APIs, 물류센터 APIs | 4 | 공통 | 조회 페이지 Min = 1, Max: 리턴되는 totalPages 값 ※ 목록을 조회하실 경우, 반드시 입력해주세요 |
| 호출 | requestResultStatus | 쿠폰 / 캐시백 APIs | 2 |  | 호출 결과 SUCCESS / FAIL |
| 호출응답 | transactionStatusResponse | 쿠폰 / 캐시백 APIs | 1 |  | 호출응답 상세 |
| 회수 | NoCollect | 교환 APIs | 1 |  | 회수 불필요 |
| 회수실패 | COLLECT_FAIL, Fail | 교환 APIs | 1 |  | 회수실패 |
| 회수안함 | NO_RETURN | 교환 APIs | 1 |  | 회수안함 |
| 회수연동 | BeforeDirection, CompleteDirection | 교환 APIs | 1 |  | 회수연동 전 |
| 회수연동실패 | DirectionFail | 교환 APIs | 1 |  | 회수연동실패 |
| 회수중 | Delivering | 교환 APIs | 1 |  | 회수중 |
| 회수진행 | RETURN | 교환 APIs | 1 |  | 회수진행 |
