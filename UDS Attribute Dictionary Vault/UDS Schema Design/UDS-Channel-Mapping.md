# UDS Channel Mapping

이 파일은 `UDS-Channel-Mapping.csv`의 설명판입니다. 행은 채널, 열은 UDS 한국어 속성입니다. 셀에는 로컬 추출 CSV에서 확인된 원천 필드명을 넣었고, 확인되지 않은 항목은 비워 두었습니다.

## Source dictionaries inspected
- Coupang: `_csv/Coupang/01 - Universal Total Table — 전체 Coupang 고유 UDS 속성.csv` (`Coupang 필드명`)
- Cafe24: `_csv/Cafe24/01 - Universal Total Table — 전체 Cafe24 고유 UDS 속성.csv` (`Cafe24 필드명`)
- Naver Smart Store: `_csv/Naver Smart Store/01 - Universal Total Table — 전체 Naver Smart Store 고유 UDS 속성.csv` (`Naver 필드명`)
- Gmarket/Auction: `_csv/Gmarket Auction/01 - Universal Total Table — 전체 Gmarket-Auction 고유 UDS 속성.csv` (`Gmarket/Auction 필드명`)
- SSG Mall: `_csv/SSG Mall/01 - Universal Total Table — SSG (1163 attributes).csv` (`SSG 필드명`)

## Mapping table

### 주문

| channel | 채널 | 채널 주문 ID | 주문일시 | 결제일시 | 주문 상태 | 결제 수단 | 통화 | 주문 금액 | 할인 금액 | 결제 금액 | 판매자 ID | 원본 수집 시각 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang |  | orderId | orderedAt / orderDate | paidAt | STATUS | paymentId |  |  |  |  | vendorId |  |
| Cafe24 |  | order_id | order_date / ordered_date | pay_date, payment_date | order_status, order_status_additional_info, process_status, status, status_additional_info, status_name_id, status_type / payment_status, status | change_payment_method, code, display, payment_display_type, payment_method, payment_method_code, payment_method_url, payment_methods | commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | order_price_amount / commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | discount_amount, keep_auto_calculation, order_sale_price / country_shipping_fee, free_shipping_price, include_regional_shipping_rate, include_shipping_fee, permission_delivery_fee_inquiry, prepaid_shipping_fee, ship_benefits, shipping_fee, shipping_fee_criteria, shipping_fee_detail, shipping_fee_discount_amount, shipping_fee_information, shipping_fee_sale, shipping_fee_setting, shipping_fee_setting_detail, shipping_fee_type, shipping_rates | change_payment_amount, change_payment_amount_reason, paid_amount, payment_amount / commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | mall_id / shop_no |  |
| Naver Smart Store |  | orderId |  | paymentDate | productOrderStatus / productOrderStatuses | paymentMethod |  | totalAmount / payAmount |  | payAmount | merchantId |  |
| Gmarket/Auction |  | ContrNo, Data>ContrNo, Data>OrderNo, OrderNo, data>OrderNo, data>RequestOrders>OrderNo, orderNo / Data>PackNo, data>PayNo | OrderDate / Data>OrderDate | PayDate | OrderStatus | isPrepayment |  | OrderAmount / BuyerPayAmt | multiplePurchaseDiscountAmount | BuyerPayAmt | SellerId / siteSellerId |  |
| SSG Mall |  | orordNo / bfOrderId / allnOrdNo | ordCmplDts / ordCnclDts | paymtDt / paymtCmplDt | ordItemStat / ordItemStatCd / ordItemStatNm |  |  | ordAmt | dcAmt |  | venId / settlVenId |  |

### 주문상품

| channel | 채널 주문상품 ID | 상품 ID | 옵션 ID | 상품명 | 옵션명 | 판매자 SKU | 수량 | 판매 단가 | 품목 총액 | 품목 할인액 | 품목 상태 | 발주확인일시 | 구매확정일시 | 세금 포함 여부 | 과세 금액 | 상품 유형 | 클레임 가능 여부 | 행 해시 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang | vendorItemId / shipmentBoxId | sellerProductId / productId | vendorItemId / sellerSkuCode | productName / itemName, sellerProductName / displayProductName |  | externalVendorSkuCode / sellerSkuCode / externalSkuId | quantity | originalPrice / PRICE |  |  | STATUS |  | finalSettlementDate | taxType |  |  |  |  |
| Cafe24 | order_item_code | product_no | variant_code / option_id | product_name | option_value / option_id | custom_product_code / variant_code | quantity | product_price / price | order_price_amount | discount_amount, keep_auto_calculation, order_sale_price | order_status, order_status_additional_info, process_status, status, status_additional_info, status_name_id, status_type / payment_status, status |  | purchaseconfirmation_date | include_tax | tax_amount |  | cancel_request |  |
| Naver Smart Store | productOrderId | channelProductNo / originProductNo | optionId | productName / channelProductName | productOrderOption | sellerManagementCode | productQuantity | unitPriceValue / salePrice | totalAmount / purchaseAmount |  | productOrderStatus |  | paymentConfirmDate | taxType | taxationSalesAmount | productOrderType | claimType |  |
| Gmarket/Auction | SkuId | data>GoodsNo / siteDetail>gmkt>SiteGoodsNo | SkuId / ItemOptionCode | Data>GoodsName, GoodsName, data>GoodsName, data>RequestOrders>GoodsName, goodsName, items>goodsName | ItemOptionValue / Data>Data>SkuName | Data>Data>SkuManageCode / itemAddtionalInfo>inventoryCode | OrderQty / ItemOptionOrderCnt / PcsQty | itemAddtionalInfo>eCoupon>price | OrderAmount / ContrAmount | multiplePurchaseDiscountAmount | OrderStatus / ClaimStatus | OrderConfirmDate |  |  |  | goodsType | ClaimCancelType |  |
| SSG Mall | ordItemSeq / ordLotNo | ItemId / goodsMngCd | uitemId / addOrdOptnSeq | itemNm | addOptnNm / addOptnVal / addOrdOptnNm | goodsMngCd / mdlNm | ordQty / dircQty / procItemQty | fstSellprc | ordAmt | dcAmt / splVenBdnDcAmt | ordItemStatCd / ordItemStatNm / itemStatTypeCd | ordCnfDts | purchDcsnYn | ctvatInclYn |  | itemSellTypeCd / ordTypeCd06Yn | retExchPsblYn |  |

### 배송

| channel | 배송 ID | 택배사 코드 | 택배사명 | 운송장 번호 | 배송 상태 | 배송비 | 배송 메시지 | 출고 예정일 | 출고일시 | 배송완료일시 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang | shipmentBoxId | deliveryCompanyCode | deliveryCompanyName | invoiceNumber | STATUS | deliveryCharge / deliveryFee | receiver / parcelPrintMessage | estimatedShippingDate |  | deliveredDate |
| Cafe24 | shipping_code | shipping_company_code | shipping_company_name / exchange_address1, exchange_address2, exchange_country_code, return_invoice_no, return_shipping_company_name | tracking_no / exchange_address1, exchange_address2, exchange_country_code, return_invoice_no, return_shipping_company_name | shipping_status | country_shipping_fee, free_shipping_price, include_regional_shipping_rate, include_shipping_fee, permission_delivery_fee_inquiry, prepaid_shipping_fee, ship_benefits, shipping_fee, shipping_fee_criteria, shipping_fee_detail, shipping_fee_discount_amount, shipping_fee_information, shipping_fee_sale, shipping_fee_setting, shipping_fee_setting_detail, shipping_fee_type, shipping_rates / individual_fee_calculation_type, individual_shipping_fee | shipping_message | expected_delivery_date, shipments_start_date, shipped_date | expected_delivery_date, shipments_start_date, shipped_date | delivered_date |
| Naver Smart Store | deliveryBundleGroupId | collectDeliveryCompany, deliveryCompanyCode, reDeliveryCompany / logisticsCompanyId | logisticsCompanyName | trackingNumber / collectTrackingNumber |  | deliveryFee |  |  | dispatchDate |  |
| Gmarket/Auction | DeliveryGroupNo / Data>PackNo, data>PayNo | DeliveryCompanyCode | DeliveryCompName | invoiceNo / Data>Data>OrderDetail>InvoiceNo | Data>ShippingCmplDate, data>TransCompleteDate | DeliveryExpense / AddShippingFee |  | DeliveryDueDate / DeliveryDueTime | InvoiceIssueDate / Data>Data>OrderDetail>InvoiceIssueDate | Data>ShippingCmplDate, data>TransCompleteDate |
| SSG Mall | shppNo / bfShppNo / boxNo | delicoNm | delicoNm / delicoVenNm | wblNo / delicoTrscNo | lastShppProgStatDtlCd / lastShppProgStatDtlNm |  | shppMsgId / mdBuyerMsgs | whinExpcDt |  | deliveryEnd / deliveryEnds |

### 클레임

| channel | 클레임 ID | 클레임 유형 | 클레임 상태 | 클레임 사유 코드 | 클레임 사유 | 클레임 수량 | 클레임 접수일시 | 환불 금액 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang | cancelId | RETURN, cancelType / RETURN | STATUS | cancelReasonCategory1 / cancelReasonCategory2 | cancelReason | RETURNS_UNCHECKED, UC, cancelCount |  | exchangeAmount |
| Cafe24 | claim_code | claim_quantity, claim_reason_type, claim_status, claim_type, refund_bank_account_required, refund_benefit_setting, refund_processing_setting / claim_reason_type, reason, reason_type | claim_quantity, claim_reason_type, claim_status, claim_type, refund_bank_account_required, refund_benefit_setting, refund_processing_setting | claim_reason_type, reason | claim_reason / exchange_request_count, reason | claim_quantity, claim_reason_type, claim_status, claim_type, refund_bank_account_required, refund_benefit_setting, refund_processing_setting | claim_due_date | refund_amount, refund_amounts |
| Naver Smart Store |  | claimType | claimStatus / claimStatuses | cancelReason, returnReason | cancelDetailedReason | returnQuantity |  | refundAmount |
| Gmarket/Auction | ClaimSeqNo | ClaimCancelType | ClaimStatus | ClaimReason | ClaimDetailReason / CancelComment |  | ClaimDate / CancelDate |  |
| SSG Mall | ordProcDemndStatCd | ntTaskTypeCd / itemrChngDemndDivCd | claimResult / chngDemndProcStatCd / chngDemndProcStatNm | clmRsnCd | clmRsnCntt / clmRsnNm | clmQty / cnclItemQty | clmDemndDts | rlordAmt |

### 상품

| channel | 마스터 상품 ID | 채널 상품 ID | 상품명 | 브랜드명 | 카테고리 ID | 카테고리명 | 판매상태 | 등록/수정일시 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang |  | sellerProductId / productId | productName / itemName, sellerProductName / displayProductName | brand | categoryId |  | STATUS | modifiedAt |
| Cafe24 |  | product_no | product_name | brand_code, brand_name, use_brand | categories, category_no, use_category | category_name | selling / change_payment_method, code, display, payment_display_type, payment_method, payment_method_code, payment_method_url, payment_methods | updated_date |
| Naver Smart Store |  | channelProductNo / originProductNo | productName / channelProductName | brandName | leafCategoryId | wholeCategoryName | statusType / productStatusTypes | modificationYmdt, modifiedDate |
| Gmarket/Auction |  | data>GoodsNo / siteDetail>gmkt>SiteGoodsNo | Data>GoodsName, GoodsName, data>GoodsName, data>RequestOrders>GoodsName, goodsName, items>goodsName | BrandName | CategoryCode |  | GoodsStatus | updateDate |
| SSG Mall |  | ItemId | itemNm | brandNm | dispCtgId | dispCtgNm | sellStatCd / itemStatTypeCd | modifyDate |

### 재고

| channel | 재고 스냅샷 ID | 가용 재고 수량 | 안전 재고 수량 | 재고 관리 여부 | 스냅샷 시각 |
| --- | --- | --- | --- | --- | --- |
| Coupang |  | amountInStock |  | inventoryDetails |  |
| Cafe24 |  | quantity / stock_quantity_max, stock_quantity_min | safety_inventory, stock_safety_max, stock_safety_min | inventories, inventory_control_type, use_inventory |  |
| Naver Smart Store |  | stockQuantity / todayStockQuantity |  | useStockManagement |  |
| Gmarket/Auction |  | BsStockQty / itemBasicInfo>Stock>Gmkt | HoldStockQty | itemAddtionalInfo>inventoryCode |  |
| SSG Mall |  | usablInvQty / baseInvQty | rstctInvQty | invMngYn |  |

### 정산

| channel | 정산 ID | 정산 기준일 | 정산 상태 | 정산 대상 금액 | 수수료 금액 | 정산 지급 금액 |
| --- | --- | --- | --- | --- | --- | --- |
| Coupang | paymentId | settlementDate / finalSettlementDate | settlementType | settlementTargetAmount | deductionAmount | settlementAmount |
| Cafe24 | payment_no |  | settle_type / payment_settle_type | commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | change_payment_amount, change_payment_amount_reason, paid_amount, payment_amount |
| Naver Smart Store | merchantId | paymentConfirmDate | settleDecisionType | paySettleAmount | commissionSettleAmount | normalSettleAmount / quickSettleAmount |
| Gmarket/Auction | SettleType | SettleExpectDate | SettleType / SettleExceptName | TotalSettlementAmount / SettlementPrice | BasicServiceFee / SellerPcsFee | SettlementPrice / TotalTransferAmountForeign |
| SSG Mall | settlVenId |  | settlCycleCd |  | feeAmt | rlordAmt |

### 고객/수령자

| channel | 구매자 ID | 구매자명 | 구매자 연락처 | 수령자명 | 수령자 연락처 | 우편번호 | 주소 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Coupang | buyerEmail |  | buyerPhone | receiver |  |  |  |
| Cafe24 | buyer_address1, buyer_address2, buyer_zipcode, cellphone, email, names_furigana, phone, user_id, user_name / buyer | buyer_name, name / buyer_address1, buyer_address2, buyer_zipcode, cellphone, email, names_furigana, phone, user_id, user_name | buyer_phone / buyer_cellphone | name, name_en, name_furigana, receiver_name / cellphone, city_en, phone, receiver, receiver_address1, receiver_address2, receiver_zipcode, state_en, street_en, virtual_phone_no | receiver_phone / receiver_cellphone | cellphone, city_en, phone, receiver, receiver_address1, receiver_address2, receiver_zipcode, state_en, street_en, virtual_phone_no | cellphone, city_en, phone, receiver, receiver_address1, receiver_address2, receiver_zipcode, state_en, street_en, virtual_phone_no |
| Naver Smart Store | merchantId |  |  |  |  |  | baseAddress |
| Gmarket/Auction | BuyerId / data>BuyerID, data>RequestOrders>BuyerId | BuyerName, data>BuyerName, data>RequestOrders>BuyerName | BuyerMobileTel / BuyerTel | Data>RcverInfoNa, RcverInfoNa, data>ReceiverName, data>RequestOrders>ReceiverName | data>ResendInfo>ReceiverInfo>TelNo | data>ResendInfo>ReceiverInfo>ZipCode | data>ResendInfo>ReceiverInfo>Address / data>ResendInfo>ReceiverInfo>AddressFront |
| SSG Mall | ordCstId |  | frgTelno |  | frgShpplocTelno / frgShpplocHpno | frgZipcd / frgShpplocZipcd | bascAddr / dtlAddr / frgShpplocBascAddr |

### CS

| channel | 문의 ID | 문의 유형 | 문의 제목 | 문의 내용 | 답변 상태 |
| --- | --- | --- | --- | --- | --- |
| Coupang | inquiryId |  | title | content | answeredAt |
| Cafe24 | board_no | admin_name, board_category_no, board_exposure_setting, board_guide, board_list, board_name, board_type, linked_board, og_board, password_rules, permission_board_manage, use_additional_board, use_board, use_nick_name_icon, use_writer_name_icon | additional_items, additional_order_info_list, available_coupon_count_by_order, category_no, check_order_info, description, field_length, input_type, is_required, is_simple_join, max_input_length, option_values, order_coupons, order_form_input_type, order_info, order_item_delete, orderform_additional_enabled, orderform_property_id, quick_signup, shipping_info, subject, textarea_rows, width_percentage | content | reply_status |
| Naver Smart Store | questionId | questionType | title | question | answered |
| Gmarket/Auction |  | QnaType, SiteType, data>SiteType, siteId, siteType |  |  | answerStatus |
| SSG Mall | postngId | qna / noticeType | postngTitleNm | postngCntt / cnts |  |

