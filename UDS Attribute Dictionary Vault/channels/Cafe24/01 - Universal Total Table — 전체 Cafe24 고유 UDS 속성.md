---
title: Universal Total Table — 전체 Cafe24 고유 UDS 속성
channel: Cafe24
type: notion-table-migration
source_notion_page_id: 369559dfde8580d5b2c6e393b7aede0f
source_table_id: 369559df-de85-81ce-b760-c22704765d2b
rows_including_header: 1016
csv_backup: ../../_csv/Cafe24/01 - Universal Total Table — 전체 Cafe24 고유 UDS 속성.csv
---

# Universal Total Table — 전체 Cafe24 고유 UDS 속성

- Channel: [[Cafe24 Index|Cafe24]]
- Rows including header: **1016**
- CSV backup: `../../_csv/Cafe24/01 - Universal Total Table — 전체 Cafe24 고유 UDS 속성.csv`

| UDS 속성명 | Cafe24 필드명 | API 카테고리 | API 리소스 | 사용 문서 수 | UDS 필요도 | 설명 |
| --- | --- | --- | --- | --- | --- | --- |
| 가격 | price | Personal, Product | Customers wishlist, Products | 3 | ✅ 핵심 UDS | 상품 판매가 상품의 판매 가격. 쿠폰 및 혜택을 적용하기 전의 가격. 상품 등록시엔 모든 멀티 쇼핑몰에 동일한 가격으로 등록하며, 멀티쇼핑몰별로 다른 가격을 입력하고자 할 경우 상품 수정을 통해 가격을 다르게 입력할 수 있다. ※ 판매가 = [ 공급가 + (공급가 * 마진율) + 추가금액 ] |
| 가격에 | include_tax | Order | Cancellation, Exchange, Orders, Orders shippingfeecancellation, Refunds, Return | 6 | ✅ 핵심 UDS | 가격에 세금 포함 T: 세금포함 F: 세금제외 |
| 간편결제 | easypay_name | Order | Orders | 1 | ✅ 핵심 UDS | 간편결제 결제사 이름 |
| 개별배송비 | individual_fee_calculation_type, individual_shipping_fee | Order, Shipping | Orders items, Orders shippingfeecancellation, Shipping | 4 | ✅ 핵심 UDS | 개별배송비 계산 기준 P : 상품별 I : 품목별 |
| 개별배송여부 | shipping_fee_by_product | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 개별배송여부 상품에 배송비를 개별적으로 부과할 것인지 공통 배송비를 부과할 것인지에 대한 설정. 개별 배송비를 사용하지 않을 경우 공통 배송비를 사용함. shipping_calculation이 A(자동계산)일 경우 null로 반환. T : 사용함 F : 사용안함 |
| 결제 | commission, confirmation_url, currency_code, currency_name, exchange_rate, paid, payment_amount, payment_gateway_name, payment_proiority, shop_currency_code, shop_currency_format, shop_currency_symbol | Application, Customer, Order, Salesreport, Store | Appstore orders, Appstore payments, Currency, Customers paymentinformation, Financials dailysales, Financials monthlysales, Orders, Orders payments, Reservations, Shops | 12 | ✅ 핵심 UDS | 결제 화폐 코드 멀티쇼핑몰의 결제 화폐 코드 South Korean Won (KRW) United States Dollar (USD) Japanese Yen (JPY) Chinese Yuan (CNY) Taiwan Dollar (TWD) Euro (EUR) Brazilian Real (BRL) Vietnamese Dong (VND) |
| 결제 취소 실패 메시지 | payment_gateway_failure_message | Order | Orders payments | 1 | ✅ 핵심 UDS | PG 결제 취소 실패 메시지 |
| 결제국가 | locale_code | Application | Appstore payments | 1 | ✅ 핵심 UDS | 결제국가 |
| 결제금액 | change_payment_amount, change_payment_amount_reason, paid_amount, payment_amount | Application, Order | Appstore payments, Orders payments, Orders paymenttimeline | 4 | ✅ 핵심 UDS | 결제금액 변경 여부 입금전 상태에서만 결제금액 변경 가능 단, CS주문상태 또는 CS처리이력이 존재하는 경우에는 결제금액 변경 불가능함 ※ 결제수단별 입금전 주문상태 - 무통장입금 : 입금전 - 다이비키 : 상품준비중 ~ 배송완료 [다이비키 입금전] T : 사용함 F : 사용안함 |
| 결제방식별 | points_setting_by_payment | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 결제방식별 적립금 설정 여부 Youtube shopping 이용 시에는 미제공 B : 기본 적립금설정 사용 C : 결제방식에 따른 적립 |
| 결제번호 | payment_no | Order | Orders paymenttimeline, Payments, Unpaidorders | 5 | ✅ 핵심 UDS | 결제번호 |
| 결제상태 | payment_status, status | Application, Order | Appstore payments, Orders, Orders migrations, Payments, Reservations | 6 | ✅ 핵심 UDS | 결제상태 canceled의 경우 앱을 통해 추가된 PG사에서 결제를 취소할 경우에만 사용 가능 paid: 입금확인 unpaid: 입금전 canceled: 결제취소 |
| 결제수단 | change_payment_method, code, display, payment_display_type, payment_method, payment_method_code, payment_method_url, payment_methods | Application, Customer, Order, Salesreport, Store, Supply | Appstore payments, Customers paymentinformation, Financials dailysales, Financials monthlysales, Financials store, Orders, Orders calculation, Orders migrations, Orders payments, Orders paymenttimeline, Payment setting, Paymentgateway paymentmethods | 27 | ✅ 핵심 UDS | 결제수단 코드 주문자가 이용한 결제수단의 코드 cash : 무통장 card : 신용카드 cell : 휴대폰 tcash : 계좌이체 icash : 가상계좌 prepaid : 선불금 credit : 예치금 point : 적립금 pointfy : 통합포인트 cvs : 편의점 cod : 후불 coupon : 쿠폰 market_discount : 마켓할인 giftcard : 제휴상품권 pointcard : 제휴포인트 etc : 기타 |
| 결제수단명 | payment_method_name | Order, Store | Orders, Paymentgateway paymentmethods, Reservations | 4 | ✅ 핵심 UDS | 결제수단명 주문자가 이용한 결제수단의 이름 |
| 결제수단별 | payment_method_detail, payment_method_information | Order, Store | Financials paymentgateway, Orders paymenttimeline | 2 | ✅ 핵심 UDS | 결제수단별 정산 정보 ※ payment_method_information 하위 요소에 대한 값 정의 1) payment_method_information > period(정산 기간) D : 일별 W : 주별 M : 월별 |
| 결제안내 | payment_info_by_product | Product | Products | 1 | ✅ 핵심 UDS | 결제안내 개별설정 사용여부 T : 개별설정 F : 기본설정 사용 |
| 결제예정 | total_amount_due | Order | Orders calculation | 1 | ✅ 핵심 UDS | 결제예정 금액 |
| 결제완료 | settle_count | Salesreport | Reports productsales, Reports salesvolume | 2 | ✅ 핵심 UDS | 결제완료 수량 조회 기간동안 해당 품목이 결제 완료된 수량 |
| 결제유형 | payment_settle_type | Order | Orders paymenttimeline | 1 | ✅ 핵심 UDS | 결제유형 O : 최초결제 R : 추가결제 P : 환불 |
| 결제일 | payment_datetime | Order | Orders paymenttimeline | 1 | ✅ 핵심 UDS | 결제일 |
| 결제일시 | pay_date, payment_date | Application, Order | Appstore payments, Orders, Reservations | 3 | ✅ 핵심 UDS | 결제승인일 |
| 결제자명 | billing_name | Order | Orders | 1 | ✅ 핵심 UDS | 결제자명 입금자 이름. 주문자 혹은 수령자 이름과는 다를 수 있음. |
| 결제정보 | payment_info_id | Order | Orders items | 1 | ✅ 핵심 UDS | 결제정보 아이디 |
| 결제취소 | cancel_request | Order | Payments | 2 | ✅ 핵심 UDS | 결제취소 요청 정보 |
| 결제코드 | payment_code | Order | Orders completions | 2 | ✅ 핵심 UDS | 결제코드 |
| 결제타입 | settle_type | Order | Unpaidorders | 2 | ✅ 핵심 UDS | 결제타입 S: 기본결제 E: 추가결제 |
| 고객 | customer_notification, use_customer | Notification, Order | Automails, Orders buyer, Orders buyer history | 5 | ✅ 핵심 UDS | 고객 T : 사용함 F : 사용안함 |
| 고객상담 | use_customer_inquiry | Order | Orders memos | 2 | ✅ 핵심 UDS | 고객상담 동시등록 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 고객센터 | customer_service_email, customer_service_fax, customer_service_hours, customer_service_phone, customer_service_sms | Store | Store | 1 | ✅ 핵심 UDS | 고객센터 상담/주문 이메일 쇼핑몰 화면에 표시되는 고객센터 상담 이메일 주소. |
| 공급사배송비 | supplier_shipping_fee | Order | Orders shippingfeecancellation | 1 | ✅ 핵심 UDS | 공급사배송비 |
| 공통페이지 | common_page_meta_description, common_page_title | Store | Seo setting | 2 | ✅ 핵심 UDS | 공통페이지 description 태그 |
| 과세금액 | tax_amount | Order | Cashreceipt | 1 | ✅ 핵심 UDS | 과세금액 |
| 관심상품번호 | wishlist_no | Personal | Customers wishlist | 1 | ✅ 핵심 UDS | 관심상품번호 |
| 교환 | reshipping_detail | Order | Exchange | 1 | ✅ 핵심 UDS | 교환 재발송 정보 |
| 교환/반품안내 | exchange_info, exchange_info_by_product | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 교환/반품안내 상품의 교환/반품 방법에 대한 안내 문구. HTML을 사용하여 입력이 가능하다. |
| 교환배송비(왕복) | exchange_shipping_fee | Store | Orders setting | 2 | ✅ 핵심 UDS | 교환배송비(왕복) 설정 |
| 교환상세 | exchange | Order | Orders | 2 | ✅ 핵심 UDS | 교환상세 리소스 |
| 교환상품 | exchanged_items | Order | Exchange, Orders exchange | 2 | ✅ 핵심 UDS | 교환상품 |
| 교환상품정보 | exchange_items | Order | Exchangerequests | 1 | ✅ 핵심 UDS | 교환상품정보 |
| 교환신청 | exchange_request_count, reason | Order | Exchangerequests, Orders dashboard | 2 | ✅ 핵심 UDS | 교환신청 사유 |
| 교환신청번호 | exchange_request_no | Order | Exchangerequests | 1 | ✅ 핵심 UDS | 교환신청번호 |
| 교환신청일 | exchange_request_date | Order | Orders items | 1 | ✅ 핵심 UDS | 교환요청일 교환 요청일 |
| 교환완료 | exchane_product_count, exchange_product_count | Salesreport | Reports productsales, Reports salesvolume | 2 | ✅ 핵심 UDS | 교환완료 수량 조회 기간동안 해당 품목이 교환된 수량 |
| 교환완료일 | exchange_date | Order | Orders items | 1 | ✅ 핵심 UDS | 교환완료일 교환 완료일 |
| 교환접수 | exchange_received_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 교환접수 건수 |
| 교환처리 | claim_due_date | Order | Exchange | 1 | ✅ 핵심 UDS | 교환처리 예정일 |
| 교환처리중 | exchange_processing_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 교환처리중 건수 |
| 구매금액 | discount_information | Customer | Customergroups | 1 | ✅ 핵심 UDS | 구매금액 할인설정 |
| 구매수량 | related_purchase_quantity | Store | Subscription shipments setting | 2 | ✅ 핵심 UDS | 구매수량 관계 여부 T : 구매수량에 따라 F : 구매수량에 관계없이 |
| 국내/해외배송 | shipping_type | Shipping, Supply | Carriers, Shipping, Shipping suppliers | 5 | ✅ 핵심 UDS | 국내/해외배송 설정 EC 베트남, 필리핀 버전에서는 사용할 수 없음. A : 국내배송 C : 해외배송 B : 국내/해외배송 |
| 기타배송 | shipping_etc | Shipping, Supply | Shipping, Shipping suppliers | 4 | ✅ 핵심 UDS | 기타배송 배송방법(shipping_method)이 shipping_06(기타) 일 때 기타 배송 정보 |
| 답변상태 | reply_status | Community | Boards articles | 1 | ✅ 핵심 UDS | 답변상태 N : 답변 전 P : 처리중 C : 답변 완료 |
| 동일상품교환 | same_product | Order | Exchange, Orders exchange | 2 | ✅ 핵심 UDS | 동일상품교환 여부 T : 동일상품교환 F : 다른상품교환 |
| 마켓 | market_cancel_request, market_cancel_request_quantity, market_custom_variant_code, market_fail_reason, market_fail_reason_guide, market_fail_reason_type, market_seller_id, market_sync | Order, Product | Orders, Orders items, Products | 5 | ✅ 핵심 UDS | 마켓 취소요청 여부 T : 취소 요청된 마켓 주문 F : 취소 요청되지 않은 마켓 주문 |
| 마켓 ID | market_id | Order | Orders | 1 | ✅ 핵심 UDS | 마켓 구분값 가격 비교 사이트를 통하여 마켓 등에서 상품 구매 시 해당 사이트를 구분하기 위한 ID |
| 마켓 주문번호 | market_order_no | Order | Orders | 2 | ✅ 핵심 UDS | 마켓 주문 번호 ,(콤마)로 여러 건을 검색할 수 있다. |
| 마켓연동 | open_market_status | Order | Orders items | 1 | ✅ 핵심 UDS | 마켓연동 상태값 |
| 면세금액 | tax_free_amount | Order | Cashreceipt | 1 | ✅ 핵심 UDS | 면세금액 |
| 묶음배송 | bundled_shipping_type | Order | Orders items | 1 | ✅ 핵심 UDS | 묶음배송 타입 배송 대상 주문건의 묶음배송 유형 N : 단일 주문 일반 배송(Normal) C :복합 주문 결합 배송(Combination) |
| 반품 | exchange_address1, exchange_address2, exchange_country_code, return_invoice_no, return_shipping_company_name | Order, Supply | Exchange, Orders exchange, Orders return, Return, Suppliers | 10 | ✅ 핵심 UDS | 반품 주소 국가 코드 |
| 반품배송비 | return_ship_type, return_shipping_fee, return_shipping_fee_detail | Order | Cancellation, Exchange, Refunds, Return | 4 | ✅ 핵심 UDS | 반품배송비 DEFAULT 0.00 |
| 반품배송비(편도) | return_shipping_fee | Store | Orders setting | 2 | ✅ 핵심 UDS | 반품배송비(편도) 설정 |
| 반품사유 | claim_reason_type, reason | Order | Orders return, Return | 2 | ✅ 핵심 UDS | 반품사유 구분 A : 고객변심 B : 배송지연 C : 배송불가지역 L : 수출/통관 불가 D : 포장불량 E : 상품불만족 F : 상품정보상이 G : 서비스불만족 H : 품절 I : 기타 |
| 반품상세 | return | Order | Orders | 2 | ✅ 핵심 UDS | 반품상세 리소스 |
| 반품수거일 | return_collected_date | Order | Orders items | 1 | ✅ 핵심 UDS | 반품수거일 |
| 반품승인일시 | return_confirmed_date | Order | Orders, Orders items | 2 | ✅ 핵심 UDS | 반품승인일시 |
| 반품신청 | return_request_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 반품신청 건수 |
| 반품신청일 | return_request_date | Order | Orders items | 1 | ✅ 핵심 UDS | 반품요청일 반품 요청일 |
| 반품완료 | return_product_count | Salesreport | Reports productsales, Reports salesvolume | 2 | ✅ 핵심 UDS | 반품완료 수량 조회 기간동안 해당 품목이 반품된 수량 |
| 반품접수 | return_received_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 반품접수 건수 |
| 반품주소 | exchange_zipcode, return_address | Order, Shipping, Supply | Return, Shipping, Suppliers | 5 | ✅ 핵심 UDS | 반품주소 우편번호 |
| 반품처리 | claim_due_date | Order | Return | 1 | ✅ 핵심 UDS | 반품처리 예정일 |
| 반품처리중 | return_processing_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 반품처리중 건수 |
| 배송 | customer_pays_return_shipping, delivery_type, shipping_calculation, shipping_type, shipping_type_text, use | Order, Personal, Product, Salesreport, Store | Bundleproducts, Carts, Orders, Orders calculation, Orders setting, Products, Reports salesvolume, Shippingmanager, Subscription shipments | 11 | ✅ 핵심 UDS | 배송 후 교환/반품 신청 시 구매자부담 배송비 결제 사용 여부 T : 사용함 F : 사용안함 |
| 배송국가 | oversea_shipping_country_list | Shipping, Supply | Shipping, Shipping suppliers | 3 | ✅ 핵심 UDS | 배송국가 |
| 배송규격 | package_volume | Shipping | Shipping | 2 | ✅ 핵심 UDS | 배송규격 |
| 배송기간 | shipping_end_date, shipping_period, shipping_start_date | Product, Shipping, Supply | Bundleproducts, Products, Shipping, Shipping suppliers | 8 | ✅ 핵심 UDS | 배송기간 (개별배송비를 사용할 경우) 상품 배송시 평균적으로 소요되는 배송 기간. shipping_calculation이 A(자동계산)일 경우 null로 반환. |
| 배송메시지 | shipping_message | Order | Orders receivers, Orders receivers history, Subscription shipments | 5 | ✅ 핵심 UDS | 배송 메세지 |
| 배송방법 | shipping_method | Product, Shipping, Supply | Bundleproducts, Products, Shipping, Shipping suppliers | 8 | ✅ 핵심 UDS | 배송방법 shipping_01 : 택배 shipping_02 : 빠른등기 shipping_04 : 직접배송 shipping_05 : 퀵배송 shipping_06 : 기타 shipping_07 : 화물배송 shipping_08 : 매장직접수령 shipping_09 : 배송필요 없음 shipping_10 : 고객직접선택 |
| 배송번호 | shipping_code | Order | Fulfillments, Orders items, Orders receivers, Orders receivers history, Orders shipments, Reservations, Shipments | 11 | ✅ 핵심 UDS | 배송번호 배송번호. 품목별 주문번호를 배송준비중으로 처리하면 시스템이 자동으로 부여하는 번호. |
| 배송비 | country_shipping_fee, free_shipping_price, include_regional_shipping_rate, include_shipping_fee, permission_delivery_fee_inquiry, prepaid_shipping_fee, ship_benefits, shipping_fee, shipping_fee_criteria, shipping_fee_detail, shipping_fee_discount_amount, shipping_fee_information, shipping_fee_sale, shipping_fee_setting, shipping_fee_setting_detail, shipping_fee_type, shipping_rates | Customer, Order, Product, Promotion, Salesreport, Shipping, Store, Supply | Benefits, Benefits setting, Bundleproducts, Cancellation, Carriers, Coupons, Customergroups, Exchange, Orders, Orders calculation, Orders items, Products | 28 | ✅ 핵심 UDS | 배송비 설정 데이터 ※shipping_fee_setting_detail의 하위요소에 대한 값 정의 1)shipping_fee_setting_domestic > shipping_fee_type shipping_fee_type(배송비 설정) T : 배송비 무료 R : 고정배송비 사용 M : 구매 금액에 따른 부과 D : 구매 금액별 차등 배송료 사용 W : 상품 무게별 차등 배송료 사용 C : 상품 수량별 차등 배송료 사용 N : 상품 수량에 비례하여 배송료 부과 2)shipping_fee_setting_domestic > shipping_fee_criteria shipping_fee_criteria(배송비 청구 기준 주문금액 조건 설정) D : 할인전, 정상판매가격 기준(권장) A : 할인 적용 후 결제 금액 기준 3)shipping_fee_setting_oversea > additional_handling_fee_list > unit unit(해외배송 부가금액 단위) W : 정액 P |
| 배송비타입 | shipping_fee_type, shipping_fee_type_text | Order, Shipping, Supply | Orders items, Shipping, Shipping suppliers | 5 | ✅ 핵심 UDS | 배송비타입 T : 배송비 무료 R : 고정배송비 사용 M : 구매 금액에 따른 부과 D : 구매 금액별 차등 배송료 사용 W : 상품 무게별 차등 배송료 사용 C : 상품 수량별 차등 배송료 사용 N : 상품 수량에 비례하여 배송료 부과 |
| 배송비할인 | shipping_discount_amount, shipping_fee_discount_amount | Order | Cancellation, Exchange, Orders shippingfeecancellation, Refunds, Return | 5 | ✅ 핵심 UDS | 배송비할인 취소액 |
| 배송사 | carrier_id, shipping_carrier, shipping_carrier_code | Order, Shipping | Carriers, Exchange, Fulfillments, Orders, Orders calculation, Orders exchange, Orders return, Orders shipments, Return, Shipments | 20 | ✅ 핵심 UDS | 배송사 아이디 배송사에서 반송장번호 업데이트시 carrier_id 필수 |
| 배송상태 | shipping_status | Order | Orders | 1 | ✅ 핵심 UDS | 배송상태 F : 배송전 M : 배송중 T : 배송완료 W : 배송보류 X : 발주전 |
| 배송시작일 | expected_delivery_date, shipments_start_date, shipped_date | Order, Store | Orders items, Subscription shipments, Subscription shipments setting | 4 | ✅ 핵심 UDS | 배송시작일 설정 DEFAULT 3 |
| 배송안내 | shipping_info_by_product | Product | Products | 1 | ✅ 핵심 UDS | 배송안내 개별설정 사용여부 T : 개별설정 F : 기본설정 사용 |
| 배송업체 | carrier_id, shipping_company_id, shipping_company_type | Order, Shipping | Carriers, Orders items, Shipping | 4 | ✅ 핵심 UDS | 배송업체 아이디 배송업체의 아이디 |
| 배송예정일 | expected_delivery_date | Order | Subscription shipments items | 2 | ✅ 핵심 UDS | 배송예정일 |
| 배송완료 | auto_delivery_completion, delivery_completion_after_days, shipped_auto_check_start_day, use_shipped_auto_check_start_day | Store | Orders setting | 2 | ✅ 핵심 UDS | 배송완료 일괄체크 시작시점 사용여부 T : 사용함 F : 사용안함 |
| 배송완료일 | delivered_date | Order | Orders items | 1 | ✅ 핵심 UDS | 배송완료일 배송 완료일 |
| 배송정보 | shipping_scope | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 배송정보 국내에만 배송이 가능한 상품인지 해외에도 배송이 가능한 상품인지 표시. [쇼핑몰 설정 > 배송 설정 > '배송 정책 설정 > 배송비 설정 > 개별배송비 설정'] 에서 상품별 개별 배송료 설정이 사용안함인 경우 설정 불가. ※ 쇼핑몰이 EC Global 쇼핑몰일 경우 "C"를 필수로 입력해야한다. EC 베트남, 필리핀 버전에서는 사용할 수 없음. A : 국내배송 C : 해외배송 B : 국내/해외배송 DEFAULT A |
| 배송주기 | subscription_shipments_cycle, subscription_shipments_cycle_type | Order, Store | Subscription shipments, Subscription shipments items, Subscription shipments setting | 5 | ✅ 핵심 UDS | 배송주기 ,(콤마)로 여러 건을 검색할 수 있다. 1W : 1주 2W : 2주 3W : 3주 4W : 4주 1M : 1개월 2M : 2개월 3M : 3개월 4M : 4개월 5M : 5개월 6M : 6개월 1Y : 1년 |
| 배송지 | receiver_address_modify_button_exposure, show_shipping_address | Order, Store | Orders, Orders setting | 4 | ✅ 핵심 UDS | 배송지 변경 버튼 노출 범위 설정 N00 : 입금전 N10 : 상품준비중 N20 : 배송준비중 N22 : 배송보류 |
| 배송지역 | shipping_area, shipping_place | Product, Shipping, Supply | Bundleproducts, Products, Shipping, Shipping suppliers | 8 | ✅ 핵심 UDS | 배송지역 (개별배송비를 사용할 경우) 상품을 배송할 수 있는 지역. shipping_calculation이 A(자동계산)일 경우 null로 반환. |
| 배송추적 | track_shipment_url | Shipping | Carriers | 2 | ✅ 핵심 UDS | 배송추적 URL |
| 부가금액 | additional_fee | Shipping, Supply | Shipping additionalfees, Shipping suppliers additionalfees | 2 | ✅ 핵심 UDS | 부가금액 |
| 부과금액 | fee_name | Shipping, Supply | Shipping additionalfees, Shipping suppliers additionalfees | 2 | ✅ 핵심 UDS | 부과금액 명칭 |
| 불량회원 | blacklist_type | Customer, Privacy | Customers, Customersprivacy | 2 | ✅ 핵심 UDS | 불량회원 차단설정 해당 회원의 불량회원 타입. 불량회원 타입에 따라 상품구매 차단, 로그인 차단, 로그인과 상품구매 모두를 차단할 수 있음. P : 상품구매차단 L : 로그인차단 A : 로그인&상품구매 차단 |
| 불량회원설정 | use_blacklist | Customer, Privacy | Customers, Customersprivacy | 2 | ✅ 핵심 UDS | 불량회원설정 불량회원 여부. 불량회원일 경우 불량회원 타입에 따라 상품구매 차단, 로그인 차단, 로그인과 상품구매 모두를 차단할 수 있음. T : 설정함 F : 설정안함 |
| 비회원 | guest_purchase_button_display, show_coupon_to_non_members, show_message_to_non_members, use_non_member | Store | Coupons setting, Orderform setting, Privacy orders, Restocknotification setting | 8 | ✅ 핵심 UDS | 비회원 구매버튼 노출 buy_limit_type를 M(회원만 구매)으로 선택 하였을때만 설정 가능 T : 사용함 F : 사용안함 |
| 상태 | status | Product, Supply | Products approve, Suppliers | 4 | ✅ 핵심 UDS | 상태 공급사가 승인 요청한 해당 상품의 승인 상태 N : 승인요청 (신규상품) 상태값 E : 승인요청 (상품수정) 상태값 C : 승인완료 상태값 R : 승인거절 상태값 I : 검수진행중 상태값 Empty Value : 요청된적 없음 |
| 상품 판매가 | product_price | Order, Personal, Salesreport | Carts, Orders items, Refunds, Reports productsales, Reports salesvolume, Reservations | 6 | ✅ 핵심 UDS | 상품 판매가 상품의 판매가. 멀티쇼핑몰 운영 시에는 판매가를 쇼핑별 화폐단위로 환산하여 보여줌. |
| 상품결제안내 | payment_info | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 상품결제안내 상품의 결제 방법에 대한 안내 문구. HTML을 사용하여 입력이 가능하다. |
| 상품구매금액 | order_price_amount | Order | Cancellation, Cashreceipt, Exchange, Orders paymentamount, Return | 5 | ✅ 핵심 UDS | 상품구매금액 |
| 상품명 | product_name | Order, Product, Translation | Bundleproducts, Mains products, Orders items, Products, Reservations, Subscription shipments, Translations products | 10 | ✅ 핵심 UDS | 상품명 상품의 이름. 상품명은 상품을 구분하는 가장 기초적인 정보이며 검색 정보가 된다. HTML을 사용하여 입력이 가능하다. |
| 상품명(관리용) | internal_product_name | Order, Product | Bundleproducts, Orders items, Products | 5 | ✅ 핵심 UDS | 상품명(관리용) ,(콤마)로 여러 건을 검색할 수 있다. |
| 상품배송안내 | shipping_info | Product | Bundleproducts, Products | 4 | ✅ 핵심 UDS | 상품배송안내 상품의 배송 방법에 대한 안내 문구. HTML을 사용하여 입력이 가능하다. |
| 상품번호 | product_no | Community, Order, Personal, Privacy, Product, Salesreport, Translation | Boards articles, Bundleproducts, Carts, Categories products, Customers wishlist, Mains products, Orderform properties, Orders, Orders items, Products, Products additionalimages, Products approve | 47 | ✅ 핵심 UDS | 상품번호 상품의 고유한 일련 번호. 해당 쇼핑몰 내에서 상품 번호는 중복되지 않음. 조회시 상품번호(product_no)와 품목코드(variant_code) 둘 중에 하나는 반드시 포함하여야한다. ,(콤마)로 여러 건을 검색할 수 있다. |
| 상품상세페이지 | show_product_detail | Promotion | Coupons, Serialcoupons | 3 | ✅ 핵심 UDS | 상품상세페이지 노출여부 T : 상품상세페이지 노출 F : 상품상세페이지 미노출 |
| 상품옵션 | option_id | Order | Orders items | 1 | ✅ 핵심 UDS | 상품옵션 아이디 상품옵션의 아이디 |
| 상품코드 | product_code | Order, Product | Bundleproducts, Orders, Orders items, Products, Subscription shipments | 7 | ✅ 핵심 UDS | 상품코드 검색어를 상품코드에 포함하고 있는 상품 검색(대소문자 구분 필요) ,(콤마)로 여러 건을 검색할 수 있다. |
| 세트상품명 | product_bundle_name | Order | Orders items | 1 | ✅ 핵심 UDS | 세트상품명 분리형 세트상품의 이름 일체형 세트 상품의 이름은 product_name에서 표시됨 |
| 세트상품명( | product_bundle_name_default | Order | Orders items | 1 | ✅ 핵심 UDS | 세트상품명(기본) 분리형 세트상품의 이름 일체형 세트 상품의 이름은 product_name에서 표시됨 |
| 세트상품번호 | product_bundle_no | Order | Orders items | 1 | ✅ 핵심 UDS | 세트상품번호 분리형 세트상품의 번호 일체형 세트 상품의 번호는 product_no에서 표시됨. |
| 수량 | quantity | Order, Personal, Product | Carts, Orders items, Products carts, Products variants, Products variants inventories, Refunds, Reservations, Subscription shipments items | 11 | ✅ 핵심 UDS | 수량 해당 품목에 판매가 가능한 재고 수량. 재고 수량은 주문 또는 결제시 차감되며, 품절 표시를 위하여 체크된다. |
| 수령자 | cellphone, city_en, phone, receiver, receiver_address1, receiver_address2, receiver_zipcode, state_en, street_en, virtual_phone_no | Order | Exchange, Orders receivers, Orders receivers history, Subscription shipments | 6 | ✅ 핵심 UDS | 수령자 휴대 전화 한국몰일 경우 010-0000-0000 형태로 입력 그외 해외몰일 경우 국가번호-000-0000 형태로 입력 |
| 수령자 전화번호 | receiver_phone | Order | Subscription shipments | 2 | ✅ 핵심 UDS | 수령자 일반 전화 |
| 수령자 휴대전화 | receiver_cellphone | Order | Reservations, Subscription shipments | 3 | ✅ 핵심 UDS | 수령자 휴대 전화 |
| 수령자명 | name, name_en, name_furigana, receiver_name | Order | Orders, Orders migrations, Orders receivers, Orders receivers history, Reservations, Subscription shipments | 8 | ✅ 핵심 UDS | 수령자명 (발음) Youtube shopping 이용 시에는 미제공 해외몰 중 일본몰인 경우에만 필수 입력 |
| 수령자정보 | receivers | Order | Orders, Orders migrations | 4 | ✅ 핵심 UDS | 수령자정보 리소스 조회시 Embed 파라메터를 사용하여 조회할 수 있다. |
| 수령자주소 | receiver_address | Order | Orders | 1 | ✅ 핵심 UDS | 수령자주소 수령자 주소. 주문자 혹은 입금자 주소와는 다를 수 있음. |
| 승인상태 | approve_status | Product | Products | 1 | ✅ 핵심 UDS | 승인상태 검색 N : 승인요청 (신규상품) 상태값 E : 승인요청 (상품수정) 상태값 C : 승인완료 상태값 R : 승인거절 상태값 I : 검수진행중 상태값 |
| 시장주소 | market_zipcode | Supply | Suppliers | 2 | ✅ 핵심 UDS | 시장주소 우편번호 |
| 신규회원 | new_members_count | Store | Dashboard | 1 | ✅ 핵심 UDS | 신규회원 수 신규가입한 회원의 숫자 |
| 신청결제사 | pg_name | Order | Cashreceipt | 1 | ✅ 핵심 UDS | 신청결제사 |
| 실결제금액 | actual_order_amount, payed_amount | Order, Salesreport | Orders migrations, Reports hourlysales | 3 | ✅ 핵심 UDS | 실결제금액 |
| 실환불금액 | actual_refund_amount | Order | Refunds | 1 | ✅ 핵심 UDS | 실환불금액 |
| 심사상태 | review_status | Store | Paymentgateway | 2 | ✅ 핵심 UDS | 심사상태 AWAITING_PAYMENT : 결제대기 PENDING_REVIEW : 심사대기 APPROVED : 심사완료 DEFAULT AWAITING_PAYMENT |
| 안전재고수량 | safety_inventory, stock_safety_max, stock_safety_min | Product | Products, Products variants, Products variants inventories | 5 | ✅ 핵심 UDS | 안전재고수량 Youtube shopping 이용 시에는 미제공 |
| 여신상태 | loan_status | Order | Orders | 1 | ✅ 핵심 UDS | 여신상태 OK : GOOD NG : NOT GOOD ER : ERROR |
| 영문 상품명 | eng_product_name | Order, Product | Bundleproducts, Orders items, Products | 5 | ✅ 핵심 UDS | 영문 상품명 검색어를 영문 상품명에 포함하고 있는 상품 검색(대소문자 구분 없음) ,(콤마)로 여러 건을 검색할 수 있다. |
| 옵션 | change_option, has_option, option_list_type, option_preview, option_price, option_type, options | Order, Personal, Product, Store | Carts, Orders items, Products, Products options, Products setting, Products variants, Reservations, Subscription shipments setting | 12 | ✅ 핵심 UDS | 옵션 구성방식 옵션을 사용할 경우, 옵션의 유형 표시 ● 조합 일체선택형 : 하나의 셀렉스박스(버튼 이나 라디오버튼)에 모든 옵션이 조합되어 표시됨 ● 조합 분리선택형 : 옵션을 각각의 셀렉스박스(버튼 이나 라디오버튼)로 선택할 수 있으며 옵션명을 기준으로 옵션값을 조합할 수 있음 ● 상품 연동형 : 옵션표시방식은 조합형과 유사하지만 필수옵션과 선택옵션을 선택할 수 있음. 옵션의 조합을 제한 없이 생성할 수 있음. ● 독립 선택형 : 독립적인 조건 여러개를 각각 선택할 수 있는 옵션으로 옵션 값이 조합되지 않고 각각의 품목으로 생성됨. C : 조합 일체선택형 S : 조합 분리선택형 E : 상품 연동형 F : 독립 선택형 |
| 옵션 코드 | variant_code | Order, Personal, Product | Carts, Customers wishlist, Orders items, Products carts, Products variants, Products variants inventories, Subscription shipments | 10 | ✅ 핵심 UDS | 상품 품목 코드 시스템이 품목에 부여한 코드. 해당 쇼핑몰 내에서 품목 코드는 중복되지 않음. |
| 옵션값 | option_value | Order | Orders items, Reservations | 2 | ✅ 핵심 UDS | 옵션값 주문한 상품의 옵션값 |
| 옵션별로 | select_one_by_option | Product | Products, Products options | 3 | ✅ 핵심 UDS | 옵션별로 한 개씩 선택 (독립형 옵션) 독립형 옵션을 사용할 경우, 하나의 옵션을 여러개 중복하여 선택할 수 없고 한개씩만 선택 가능함. T : 사용함 F : 사용안함 독립형에만 존재 체크시 옵션별로 한개씩 선택 값 처리 |
| 옵션세트 | option_preset_code | Product | Products options | 2 | ✅ 핵심 UDS | 옵션세트 코드 상품연동형 옵션을 사용할 경우, 옵션 세트 코드 표시 |
| 우편번호 | zipcode | Collection, Order, Privacy, Shipping, Store, Supply | Customersprivacy, Manufacturers, Orders calculation, Orders receivers, Orders receivers history, Shippingorigins, Store, Suppliers | 14 | ✅ 핵심 UDS | 우편번호 Youtube shopping 이용 시에는 미제공 |
| 운송장번호 | tracking_no | Order | Exchangerequests, Fulfillments, Orders items, Orders shipments, Returnrequests, Shipments | 9 | ✅ 핵심 UDS | 반품 송장 번호 |
| 이메일 | email, email_duplication, exclude_unsubscribed, send_email, use_email_agree_point | Collection, Mileage, Privacy, Promotion, Shipping, Store, Supply | Carriers, Coupons, Customers setting, Customersprivacy, Manufacturers, Points, Points autoexpiration, Points report, Points setting, Store, Suppliers users, Users | 20 | ✅ 핵심 UDS | 이메일 공급사 운영자의 이메일 주소. 공급사 운영자의 연락처 저장 목적으로 사용함. 공급사 운영자 상세 조회 API에서만 확인 가능하다. |
| 이메일/모바일 | agree_restriction, agree_restriction_period | Promotion | Customerevents | 2 | ✅ 핵심 UDS | 이메일/모바일 메시지 수신동의 변경 불가 기간 1: 1개월 3: 3개월 6: 6개월 12: 12개월 -1: 무기한 |
| 잔여 건수 | balance | Notification | Sms balance | 1 | ✅ 핵심 UDS | SMS 잔여 건수 |
| 재고 | inventories, inventory_control_type, use_inventory | Product | Products, Products variants, Products variants inventories | 6 | ✅ 핵심 UDS | 재고 수량체크 기준 재고 수량을 어느 시점에 차감할 것인지 여부. 무통장 입금처럼 결제 시점과 주문 시점이 다른 경우 재고를 차감하는 기준을 다르게 설정할 수 있다. 주문 기준 : 주문한 시점에 재고 차감. 무통장 입금의 경우 입금 완료가 되지 않아도 재고를 차감한다. 결제 기준 : 결제한 시점에 재고 차감. 무통장 입금의 경우 입금 완료가 된 다음 재고를 차감한다. A : 주문기준 B : 결제기준 |
| 재고복구 | recover_inventory | Order | Cancellation, Exchange, Orders cancellation, Orders exchange, Orders return, Orders shortagecancellation, Payments, Return | 14 | ✅ 핵심 UDS | 재고복구 T : 복구함 F : 복구안함 DEFAULT F |
| 재고수량 | stock_quantity_max, stock_quantity_min | Product | Products | 1 | ✅ 핵심 UDS | 재고수량 검색 최대값 재고가 해당 값 이하로 남아있는 상품 검색. 품목을 여러개 갖고 있는 상품의 경우 해당 조건에 해당하는 품목이 하나라도 있을 경우 검색함. |
| 적립금보유회원 | is_point_check | Customer | Customers | 1 | ✅ 핵심 UDS | 적립금보유회원 탈퇴 처리 여부 F : 탈퇴 안 함 T : 탈퇴 처리 |
| 전 주문상태 | order_status_before_cs | Order | Orders items | 1 | ✅ 핵심 UDS | CS 전 주문상태 |
| 전체주소 | address_full | Order | Orders calculation, Orders receivers, Orders receivers history | 4 | ✅ 핵심 UDS | 전체주소 |
| 전화번호 | phone | Collection, Community, Order, Privacy, Store, Supply | Customersprivacy, Manufacturers, Orders receivers, Orders receivers history, Store, Suppliers, Suppliers users, Urgentinquiry, Users | 12 | ✅ 핵심 UDS | 전화번호 공급사 운영자의 전화번호. 공급사 운영자의 연락처 저장 목적으로 사용함. 공급사 운영자 상세 조회 API에서만 확인 가능하다. |
| 정기결제 | subscription | Order | Orders, Orders items | 3 | ✅ 핵심 UDS | 정기결제 여부 T : 정기결제 F : 정기결제 아님 |
| 정기배송 | max_delivery_limit, payment_method_id, product_binding_type, subscription_id, subscription_item_id, subscription_no, subscription_shipments_count, subscription_shipments_count_type, subscription_shipments_name, subscription_state, use_discount | Customer, Order, Store | Customers paymentinformation, Subscription shipments, Subscription shipments items, Subscription shipments setting | 10 | ✅ 핵심 UDS | 정기배송 횟수 0 : 제한없음 2 : 2회 3 : 3회 4 : 4회 6 : 6회 10 : 10회 12 : 12회 DEFAULT 0 |
| 조회 건수 | limit | Application, Category, Collection, Community, Customer, Mileage, Notification, Order, Personal, Privacy, Product, Promotion, Salesreport, Shipping, Store, Supply, Translation | Activitylogs, Appstore payments, Benefits, Boards articles, Boards articles comments, Boards comments, Brands, Bundleproducts, Carts, Cashreceipt, Categories, Categories products | 61 | ✅ 핵심 UDS | 조회결과 최대건수 조회하고자 하는 최대 건수를 지정할 수 있음. 예) 10 입력시 10건만 표시함. DEFAULT 100 |
| 조회 시작 위치 | offset | Application, Category, Collection, Community, Customer, Mileage, Notification, Order, Personal, Privacy, Product, Promotion, Salesreport, Shipping, Store, Supply, Translation | Activitylogs, Appstore payments, Benefits, Boards articles, Boards articles comments, Brands, Bundleproducts, Carts, Cashreceipt, Categories, Classifications, Commonevents | 56 | ✅ 핵심 UDS | 조회결과 시작위치 search_type이 created_date 일 경우 creted_start_date를 증가시키면서 전체 회원을 검색할 수 있으므로 offset은 사용할 수 없다. DEFAULT 0 |
| 조회 시작일 | start_date | Application, Category, Community, Customer, Mileage, Notification, Order, Privacy, Promotion, Salesreport, Store | Activitylogs, Appstore payments, Autodisplay, Boards articles, Cashreceipt, Credits, Credits report, Customerevents, Customers memos, Customersprivacy, Discountcodes, Financials dailysales | 31 | ✅ 핵심 UDS | 검색 시작일 Youtube shopping 이용 시에는 미제공 특정 조회기준에 대한 검색 시작일. 검색 종료일과 같이 사용해야함. 검색 시작일과 종료일이 동일할 경우 해당 날짜로만 검색함. ex) 2018-12-31 00:00:00 |
| 조회 종료일 | end_date | Application, Community, Customer, Mileage, Notification, Order, Privacy, Promotion, Salesreport, Store | Activitylogs, Appstore payments, Boards articles, Cashreceipt, Credits, Credits report, Customerevents, Customers memos, Customersprivacy, Discountcodes, Financials dailysales, Orders | 28 | ✅ 핵심 UDS | 검색 종료일 Youtube shopping 이용 시에는 미제공 특정 조회기준에 대한 검색 종료일. 검색 시작일과 같이 사용해야함. 검색 시작일과 종료일이 동일할 경우 해당 날짜로만 검색함. ex) 2018-12-31 23:59:59 |
| 주문경로 | issue_order_path, order_place_name | Order, Promotion | Coupons, Orders, Serialcoupons | 5 | ✅ 핵심 UDS | 주문경로 발급한 쿠폰의 사용 가능한 주문 경로 W : 웹 쇼핑몰 전용 M : 모바일 쇼핑몰 전용 P : 브랜드앱 전용 |
| 주문경로 ID | order_place_id | Order | Orders | 2 | ✅ 핵심 UDS | 주문경로 ,(콤마)로 여러 건을 검색할 수 있다. cafe24:카페24 mobile:모바일웹 mobile_d:모바일앱 NCHECKOUT:네이버페이 inpark:인터파크 auction:옥션 sk11st:11번가 gmarket:G마켓 coupang:쿠팡 shopn:스마트스토어 |
| 주문금액 | order_amount, order_amount_detail | Application, Order | Appstore orders, Orders paymenttimeline | 3 | ✅ 핵심 UDS | 주문금액 상세 order_amount_detail code |
| 주문번호 | order_id | Application, Community, Mileage, Order | Appstore orders, Appstore payments, Boards articles, Cancellation, Cancellationrequests, Cashreceipt, Cashreceipt cancellation, Collectrequests, Credits, Exchange, Exchangerequests, Fulfillments | 82 | ✅ 핵심 UDS | 주문번호 조회하고자하는 앱스토어 주문 번호 ,(콤마)로 여러 건을 검색할 수 있다. |
| 주문상태 | order_status, order_status_additional_info, process_status, status, status_additional_info, status_name_id, status_type | Order, Store | Cancellation, Cashreceipt, Exchange, Fulfillments, Orders, Orders cancellation, Orders exchange, Orders items, Orders migrations, Orders return, Orders shipments, Orders shippingfeecancellation | 35 | ✅ 핵심 UDS | 주문상태 주문상태. 주문 상태별로 각각의 코드가 있음. ,(콤마)로 여러 건을 검색할 수 있다. N00 : 입금전 N02 : 주문접수중 N10 : 상품준비중 N20 : 배송준비중 N21 : 배송대기 N22 : 배송보류 N30 : 배송중 N40 : 배송완료 N50 : 구매확정 C00 : 취소신청 C10 : 취소접수 - 관리자 C11 : 취소접수거부 - 관리자 C34 : 취소처리중 - 환불전 C35 : 취소처리중 - 환불완료 C36 : 취소처리중 - 환불보류 C40 : 취소완료 C41 : 취소 완료 - 환불전 C42 : 취소 완료 - 환불요청중 C43 : 취소 완료 - 환불보류 C47 : 입금전취소 - 구매자 C48 : 입금전취소 - 자동취소 C49 : 입금전취소 - 관리자 R00 : 반품신청 R10 : 반품접수 R11 : 반품 접수 거부 R12 : 반품보류 R13 : 반품접수 - 수거완료(자동) R20 : 반품 수거 완료 R30 : 반품처리중 - 수거전 R31 : 반품처리중 - 수거완 |
| 주문상품 | discount_amount_display | Store | Orderform setting | 2 | ✅ 핵심 UDS | 주문상품 할인금액 표시 T : 사용함 F : 사용안함 |
| 주문상품 코드 | order_item_code | Order | Cancellationrequests, Collectrequests, Exchangerequests, Fulfillments, Labels, Orders, Orders benefits, Orders coupons, Orders exchangerequests, Orders items, Orders items history, Orders items labels | 34 | ✅ 핵심 UDS | 품주코드 ,(콤마)로 여러 건을 검색할 수 있다. |
| 주문상품목록 | items | Order | Orders calculation, Subscription shipments | 4 | ✅ 핵심 UDS | 주문상품목록 |
| 주문수량 | order_quantity_limit_type | Product | Products | 2 | ✅ 핵심 UDS | 주문수량 제한 기준 해당 상품의 주문 수량 제한시 제한 기준을 품목 단위로 할 것인지, 상품 단위로 할 것인지에 대한 설정 P : 상품 기준 O : 품목 기준 DEFAULT O |
| 주문일시 | order_date | Mileage, Order | Orders, Orders migrations, Points, Refunds, Reservations, Unpaidorders | 7 | ✅ 핵심 UDS | 주문일 |
| 주문자 | buyer_address1, buyer_address2, buyer_zipcode, cellphone, email, names_furigana, phone, user_id, user_name | Order | Orders buyer, Orders buyer history, Orders receivers history, Subscription shipments | 6 | ✅ 핵심 UDS | 주문자 수정자 ID 주문자정보를 수정한 사람의 ID |
| 주문자 이메일 | buyer_email | Order | Orders, Refunds, Reservations, Subscription shipments | 6 | ✅ 핵심 UDS | 주문자 이메일 |
| 주문자 전화번호 | buyer_phone | Order | Orders, Orders migrations, Subscription shipments | 4 | ✅ 핵심 UDS | 주문자 일반 전화 |
| 주문자 휴대전화 | buyer_cellphone | Order | Orders, Orders migrations, Reservations, Subscription shipments | 5 | ✅ 핵심 UDS | 주문자 휴대 전화 |
| 주문자명 | buyer_name, name | Order | Orders, Orders buyer, Orders buyer history, Orders migrations, Reservations, Subscription shipments, Unpaidorders | 9 | ✅ 핵심 UDS | 주문자명 주문자 이름. 입금자 혹은 수령자 이름과는 다를 수 있음. |
| 주문자정보 | buyer | Order | Orders, Orders migrations | 4 | ✅ 핵심 UDS | 주문자정보 리소스 |
| 주소 | receiver_direct_input_check | Order | Orders receivers | 1 | ✅ 핵심 UDS | 주소 직접입력 |
| 중요재고 | important_inventory | Product | Products variants, Products variants inventories | 4 | ✅ 핵심 UDS | 중요재고 여부 해당 재고를 중요하게 관리하는지 여부. 쇼핑몰에서는 검색을 하기위한 구분 데이터로 사용한다. A : 일반재고 B : 중요재고 |
| 지역별배송비 | include_regional_shipping_rate | Store | Subscription shipments setting | 2 | ✅ 핵심 UDS | 지역별배송비 포함여부 T : 포함 F : 미포함 |
| 진열상태 | display | Product | Bundleproducts, Products, Products variants | 6 | ✅ 핵심 UDS | 진열상태 Youtube shopping 이용 시에는 미제공 해당 품목을 진열할지 여부. 품목을 진열할 경우 상품 상세 또는 상품 목록에서 해당 품목을 선택할 수 있다. 품목이 진열되어있지 않을 경우 해당 품목이 표시되지 않으며 해당 품목을 구매할 수 없다. T : 진열함 F : 진열안함 |
| 처리상태 | status | Order | Cashreceipt, Cashreceipt cancellation | 3 | ✅ 핵심 UDS | 처리상태 신청: request 발행대기: await_issuance 발행: issued 발행거부: issuance_rejected 신청취소: canceled_request 발행취소: canceled_issuance 발행실패: failed_issuance |
| 철회상태 | request_undone | Order | Orders items | 1 | ✅ 핵심 UDS | 철회상태 Cancellation : 취소철회 Exchange : 교환철회 Return : 반품철회 |
| 추가결제 | additional_payment | Order | Exchange | 1 | ✅ 핵심 UDS | 추가결제 |
| 추가금액 | additional_amount | Product | Products variants | 2 | ✅ 핵심 UDS | 추가금액 해당 품목을 구매할 경우, 상품의 판매가에 더하여 지불해야하는 추가 가격. |
| 취소 | canceled, type | Order | Cashreceipt cancellation, Orders | 2 | ✅ 핵심 UDS | 취소 타입 신청취소: request 발행취소: issue |
| 취소 요청 여부 | payment_gateway_cancel | Order | Orders refunds, Orders shippingfeecancellation, Orders shortagecancellation | 3 | ✅ 핵심 UDS | PG 취소 요청 여부 T : 취소함 F : 취소안함 DEFAULT F |
| 취소 요청 여부 주문을 반품처리함과 동시에 PG취소도 같 | payment_gateway_cancel | Order | Orders return | 1 | ✅ 핵심 UDS | PG 취소 요청 여부 주문을 반품처리함과 동시에 PG취소도 같이 처리할 수 있다. PG취소가 가능한 결제수단(신용카드, 실시간계좌이체)에서만 사용 가능하다. 결제수단이 복수인 주문(카드 등으로 결제한 주문을 결제 후 품목을 추가한 경우)의 경우에는 PG 결제를 취소할 수 없으며 관리자 화면에서 취소해야 한다. 오픈마켓/네이버페이 주문을 취소할 경우 사용 불가 T : 취소함 F : 취소안함 DEFAULT F |
| 취소 요청 여부 주문을 취소함과 동시에 PG취소도 같이 | payment_gateway_cancel | Order | Orders cancellation | 1 | ✅ 핵심 UDS | PG 취소 요청 여부 주문을 취소함과 동시에 PG취소도 같이 처리할 수 있다. PG취소가 가능한 결제수단(신용카드, 실시간계좌이체)에서만 사용 가능하다. 결제수단이 복수인 주문(카드 등으로 결제한 주문을 결제 후 품목을 추가한 경우)의 경우에는 PG 결제를 취소할 수 없으며 관리자 화면에서 취소해야 한다. 오픈마켓/네이버페이/카카오페이 주문을 취소할 경우 사용 불가 T : 취소함 F : 취소안함 DEFAULT F |
| 취소/교환/반품 | claim_quantity, claim_reason_type, claim_status, claim_type, refund_bank_account_required, refund_benefit_setting, refund_processing_setting | Order, Store | Orders items, Orders setting | 4 | ✅ 핵심 UDS | 취소/교환/반품 요청 사유 타입 구매자의 취소/교환/반품 신청 사유 구분. 판매자의 접수 사유는 각 취소/교환/반품 리소스의 claim_reason_type으로 조회할 수 있다. 구매자 취소 신청 A:고객변심 G:서비스불만족 B:배송지연 I:기타 구매자 교환/반품 신청 O:고객변심 P:상품 불만족 V:상품불량 W:배송오류 판매자 취소/교환/반품 신청 A:고객변심 B:배송지연 J:배송오류 C:배송불가지역 L:수출/통관 불가 D:포장불량 E:상품 불만족 F:상품정보상이 K:상품불량 G:서비스불만족 H:품절 I:기타 |
| 취소/교환/반품/환불 | permission_order_cs | Supply | Suppliers users | 2 | ✅ 핵심 UDS | 취소/교환/반품/환불 처리 권한 T : 사용함 F : 사용안함 DEFAULT F |
| 취소/반품 | stock_recover, stock_recover_base, stock_recover_individual | Store | Orders setting | 2 | ✅ 핵심 UDS | 취소/반품 시 자동 수량복구 - 기본설정 Youtube shopping 이용 시에는 미제공 T : 자동 복구함 F : 자동 복구 안함 M : 수량복구 여부를 확인함 |
| 취소/환불 | deduct_cancellation_refund | Customer | Customergroups setting | 1 | ✅ 핵심 UDS | 취소/환불 금액(건) 차감 여부 T : 취소/환불 금액(건) 차감 F : 취소/환불 금액(건) 미차감 |
| 취소사유 | claim_reason_type, reason, reason_type | Order | Cancellation, Cancellationrequests, Orders cancellation, Orders shippingfeecancellation, Orders shortagecancellation | 5 | ✅ 핵심 UDS | 취소사유 구분 오픈마켓/네이버페이/카카오페이 주문을 취소할 경우 사용 불가 A : 고객변심 B : 배송지연 C : 배송불가지역 L : 수출/통관 불가 D : 포장불량 E : 상품불만족 F : 상품정보상이 G : 서비스불만족 H : 품절 I : 기타 |
| 취소상세 | cancellation | Order | Orders | 2 | ✅ 핵심 UDS | 취소상세 리소스 |
| 취소상태 | payment_gateway_cancel_statuses | Order | Refunds | 1 | ✅ 핵심 UDS | PG 취소상태 F : 취소전 M : 부분취소 완료 T : 전체취소 완료 |
| 취소수수료 | cancel_fee_amount | Order | Cancellation, Exchange, Orders paymentamount, Refunds, Reservations, Return | 6 | ✅ 핵심 UDS | 취소수수료 |
| 취소신청 | cancellation_request_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 취소신청 건수 |
| 취소완료 | cancel_product_count | Salesreport | Reports productsales, Reports salesvolume | 2 | ✅ 핵심 UDS | 취소완료 수량 조회 기간동안 해당 품목이 취소된 수량 |
| 취소요청일 | cancel_request_date | Order | Orders items | 1 | ✅ 핵심 UDS | 취소요청일 주문취소 요청일 |
| 취소일 | cancel_date | Order | Orders, Orders items | 2 | ✅ 핵심 UDS | 주문취소일 주문 취소일 |
| 취소접수 | cancellation_received_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 취소접수 건수 |
| 취소처리 일자 | payment_gateway_cancel_dates | Order | Refunds | 1 | ✅ 핵심 UDS | PG 취소처리 일자 |
| 취소처리중 | cancellation_processing_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 취소처리중 건수 |
| 클레임 사유 | claim_reason | Order | Cancellation, Exchange, Orders items, Orders shippingfeecancellation, Return | 6 | ✅ 핵심 UDS | 취소/교환/반품 요청 사유 구매자의 취소/교환/반품 신청 사유 상세 내용. 판매자의 접수 사유는 각 취소/교환/반품 리소스의 claim_reason으로 조회할 수 있다. |
| 클레임 코드 | claim_code | Order | Cancellation, Exchange, Orders cancellation, Orders exchange, Orders items, Orders paymenttimeline, Orders return, Orders shippingfeecancellation, Orders shortagecancellation, Return | 16 | ✅ 핵심 UDS | 취소/교환/반품 번호 |
| 탈퇴회원 | unregistration_admin_approval | Store | Customers setting | 1 | ✅ 핵심 UDS | 탈퇴회원 관리자 승인 T:사용함 F:사용안함 |
| 택배사 코드 | shipping_company_code | Order | Fulfillments, Orders items, Orders shipments, Shipments | 7 | ✅ 핵심 UDS | 배송업체 코드 shipping_company_code |
| 택배사명 | shipping_company_name | Order | Collectrequests, Exchangerequests, Orders items, Returnrequests | 4 | ✅ 핵심 UDS | 배송업체 이름 배송업체의 이름 |
| 판매가 | additional_price, calculate_price_based_on, price_content, price_rounding_rule, price_rounding_unit, product_tax_type_text, strikethrough_price | Personal, Product, Store | Bundleproducts, Categories properties setting, Customers wishlist, Mains properties setting, Products, Products properties setting, Products setting | 12 | ✅ 핵심 UDS | 판매가 계산 절사 단위 F : 절사안함 -2 : 0.01단위 -1 : 0.1단위 0 : 1단위 1 : 10단위 2 : 100단위 3 : 1000단위 |
| 판매건수 | sales_count | Salesreport | Financials dailysales, Financials monthlysales | 2 | ✅ 핵심 UDS | 판매건수 |
| 판매상태 | selling | Product | Bundleproducts, Products, Products variants | 6 | ✅ 핵심 UDS | 판매상태 상품을 쇼핑몰에 판매할지 여부. 상품을 진열한 상태로 판매를 중지할 경우 상품은 쇼핑몰에 표시되지만 "품절"로 표시되어 상품을 구매할 수 없다. 상품이 "진열안함"일 경우 "판매함" 상태여도 상품에 접근할 수 없기 때문에 구매할 수 없다. T : 판매함 F : 판매안함 |
| 페이지 | page_display_count | Community | Boards | 2 | ✅ 핵심 UDS | 페이지 표시 수 |
| 페이지당 | page_size | Community | Boards | 2 | ✅ 핵심 UDS | 페이지당 목록 수 |
| 편의점결제 | auto_cancel_cvs_period | Store | Orders setting | 2 | ✅ 핵심 UDS | 편의점결제 자동취소 기간 Youtube shopping 이용 시에는 미제공 |
| 평생회원 | lifetime_member, popup_notification | Privacy, Promotion | Customerevents, Customersprivacy | 3 | ✅ 핵심 UDS | 평생회원 전환 이벤트 안내 팝업 사용 여부 T: 사용함 F: 사용안함 |
| 표시상태 | use_display | Category | Categories | 2 | ✅ 핵심 UDS | 표시상태 해당 상품분류의 표시 여부. 표시안함 일 경우 해당 상품분류에 접근할 수 없다. 해당 설정은 멀티쇼핑몰별로 설정할 수 없으며 모든 쇼핑몰에 적용된다. T : 표시함 F : 표시안함 |
| 할인 판매가 | pc_discount_price | Product | Products discountprice | 1 | ✅ 핵심 UDS | PC 할인 판매가 |
| 할인금액 | discount_amount, keep_auto_calculation, order_sale_price | Order, Promotion, Salesreport | Coupons, Orders shortagecancellation, Reports hourlysales, Serialcoupons | 6 | ✅ 핵심 UDS | 할인금액 자동계산 플래그 보존여부 보존함 : T 제거함 : F DEFAULT F |
| 할인판매가 | product_discount_price_text | Store | Categories properties setting, Mains properties setting, Products properties setting | 6 | ✅ 핵심 UDS | 할인판매가 할인금액 표시문구 |
| 해외배송 | additional_handling_fee, include_foreign_delivery, international_shipping_additional_fee, international_shipping_insurance, international_shipping_insurance_fee, oversea_additional_fee, oversea_additional_fee_list, unit | Order, Promotion, Shipping, Supply | Coupons, Orders, Orders shippingfeecancellation, Refunds, Return, Serialcoupons, Shipping, Shipping additionalfees, Shipping suppliers additionalfees | 11 | ✅ 핵심 UDS | 해외배송 보험료 EC 한국 버전에서만 사용할 수 있음. T : 사용함 F : 사용안함 |
| 해외배송가능 | oversea_shipping_country | Shipping, Supply | Shipping, Shipping suppliers | 3 | ✅ 핵심 UDS | 해외배송가능 국가 제한 여부 T : 제한함 F : 제한안함 |
| 해외배송비 | international_shipping_fee | Order | Orders shippingfeecancellation | 1 | ✅ 핵심 UDS | 해외배송비 |
| 혜택제공금액기준 | order_price_greater_than, use_order_price_condition | Store | Subscription shipments setting | 2 | ✅ 핵심 UDS | 혜택제공금액기준 사용여부 T : 사용함 F : 사용안함 |
| 홈페이지 | homepage, homepage_url | Collection, Shipping, Supply | Carriers, Manufacturers, Suppliers | 6 | ✅ 핵심 UDS | 홈페이지 주소 Youtube shopping 이용 시에는 미제공 |
| 환불 | permission_order_refund, refund_bank_account_no, refund_bank_code, refund_credits, refund_manager, refund_method, refund_method_code, refund_methods, refund_naver_cash, refund_naver_points, refund_payment_methods, refund_points | Order, Privacy, Salesreport, Supply | Cancellation, Cancellationrequests, Customersprivacy, Exchange, Exchangerequests, Orders cancellation, Orders items, Orders return, Orders shippingfeecancellation, Orders shortagecancellation, Refunds, Reports hourlysales | 20 | ✅ 핵심 UDS | 환불 결제수단 cash : 무통장 card : 신용카드 cell : 휴대폰 tcash : 계좌이체 prepaid : 선불금 credit : 예치금 point : 적립금 pointfy : 통합포인트 cvs : 편의점 cod : 후불 giftcard : 제휴상품권 pointcard : 제휴포인트 etc : 기타 |
| 환불계좌 | refund_bank_account_holder | Order, Privacy | Cancellation, Cancellationrequests, Customersprivacy, Exchangerequests, Orders cancellation, Orders items, Orders return, Orders shippingfeecancellation, Orders shortagecancellation, Refunds, Return, Returnrequests | 13 | ✅ 핵심 UDS | 환불계좌 예금주 명의 Youtube shopping 이용 시에는 미제공 |
| 환불금액 | refund_amount, refund_amounts | Application, Order, Salesreport | Appstore payments, Cancellation, Exchange, Financials dailysales, Financials monthlysales, Orders shippingfeecancellation, Refunds, Reports hourlysales, Return | 9 | ✅ 핵심 UDS | 환불 금액 |
| 환불배송비 | refund_shipping_fee | Order | Refunds, Return | 2 | ✅ 핵심 UDS | 환불배송비 DEFAULT 0.00 |
| 환불번호 | refund_code | Order | Orders refunds, Refunds | 4 | ✅ 핵심 UDS | 환불번호 |
| 환불사유 | refund_reason | Order | Refunds | 1 | ✅ 핵심 UDS | 환불사유 |
| 환불상세 | refunds | Order | Orders | 2 | ✅ 핵심 UDS | 환불상세 리소스 |
| 환불상태 | refund_status, status | Order | Orders, Orders refunds, Refunds | 5 | ✅ 핵심 UDS | CS(환불)상태 ,(콤마)로 여러 건을 검색할 수 있다. F : 환불전 T : 환불완료 M : 환불보류 |
| 환불승인일 | refund_date | Application | Appstore payments | 1 | ✅ 핵심 UDS | 환불승인일 |
| 환불완료 | refund_count | Salesreport | Reports productsales | 1 | ✅ 핵심 UDS | 환불완료 수량 |
| 환불완료일 | refund_date | Order | Orders items | 1 | ✅ 핵심 UDS | 환불완료일 환불 완료일 |
| 환불완료일자 | refund_date | Order | Refunds | 1 | ✅ 핵심 UDS | 환불완료일자 |
| 환불은행명 | refund_bank_name | Order | Cancellation, Cancellationrequests, Exchangerequests, Orders cancellation, Orders items, Orders return, Orders shippingfeecancellation, Orders shortagecancellation, Refunds, Return, Returnrequests | 11 | ✅ 핵심 UDS | 환불은행명 환불 방식(refund_method)이 현금(T)일 경우 필수 ※ 해당 쇼핑몰이 EC Global 쇼핑몰일 경우 필수 환불수단(refund_method)이 "현금(T)"일 때만 사용 가능 오픈마켓/네이버페이/카카오페이 주문을 취소할 경우 사용 불가 |
| 환불전 | refund_pending_count | Order | Orders dashboard | 1 | ✅ 핵심 UDS | 환불전 건수 |
| 환불접수일자 | accepted_refund_date | Order | Refunds | 1 | ✅ 핵심 UDS | 환불접수일자 |
| 환불처리후 | send_mail, send_sms | Order | Orders refunds, Refunds | 2 | ✅ 핵심 UDS | 환불처리후 SMS 발송 여부 T : 발송함 F : 발송안함 DEFAULT T |
| 회원 | customer_group_list, customer_tier_criteria, group_description, group_no, member_authentication, member_rejoin_restriction, member_rejoin_restriction_day, member_sale, use_member | Customer, Promotion, Salesreport, Store | Benefits, Customergroups, Customergroups setting, Customers setting, Privacy orders, Reports salesvolume | 9 | ✅ 핵심 UDS | 회원 등급 기준 purchase_amount : 구매금액 purchase_count : 구매건수 purchase_amount_and_count : 구매금액과 구매건수 purchase_amount_or_count : 구매금액 또는 구매건수 shopping_index : 쇼핑지수 |
| 회원 이메일 | member_email | Order | Orders, Refunds, Reservations | 5 | ✅ 핵심 UDS | 회원 이메일 |
| 회원/비회원 | display_price_scope | Store | Products setting | 1 | ✅ 핵심 UDS | 회원/비회원 가격표시 A : 모두 표시함 (회원+비회원) C : 회원만 표시함 |
| 회원/조건 | issued_member_scope | Promotion | Coupons issues | 1 | ✅ 핵심 UDS | 회원/조건 선택 쿠폰 발급 대상 회원의 범위를 특정하여 쿠폰을 발급할 수 있음. 특정회원그룹(G)을 입력할 경우 group_no를 필수로 입력해야한다. 특정회원(M)을 입력할 경우 member_id를 필수로 입력해야한다. A : 전체 회원 G : 특정 회원 그룹 M : 특정 회원 |
| 회원가입 | agree_change_type, join_point, link_social_account, member_join_confirmation, privacy_join, use_privacy_join | Store | Customers setting, Points setting, Policy | 5 | ✅ 핵심 UDS | 회원가입 시 SNS 계정 연동 T:SNS 가입 시 동일한 이메일을 가진 계정이 있으면 연동 화면을 제공 F:연동 화면을 제공하지 않음 |
| 회원가입시 | issue_member_join, issue_member_join_recommend, issue_member_join_type | Promotion | Coupons | 2 | ✅ 핵심 UDS | 회원가입시 쿠폰 발급 대상 A : 모바일 메시지 수신동의 AND 이메일 수신동의 O : 모바일 메시지 수신동의 OR 이메일 수신동의 S : 모바일 메시지 수신동의 E : 이메일 수신동의 N : 제한없음 |
| 회원가입항목 | simple_member_join, type | Customer, Store | Customers properties, Customers setting | 4 | ✅ 핵심 UDS | 회원가입항목 표시 "F"(상세항목 표시)에서 "T"(기본항목 표시)로 변경할 경우, 아래 기능은 자동으로 사용 불가 상태로 변경됨. - 회원 가입인증 - 14세 미만 가입제한 - 19세 미만 가입제한 - 성별 가입제한 - 회원가입 입력 정보 확인 - 본인인증 서비스 설정 - 비밀번호 확인시 질문/답변 T:기본항목 표시 F:상세항목 표시 |
| 회원구분 | member_class | Notification, Privacy | Customersprivacy, Recipientgroups | 3 | ✅ 핵심 UDS | 회원구분 EC 일본, 베트남 버전에서는 사용할 수 없음. p : 개인 c : 사업자 f : 외국인 |
| 회원권한구분 | member_authority | Privacy | Customersprivacy | 2 | ✅ 핵심 UDS | 회원권한구분 Youtube shopping 이용 시에는 미제공 회원 권한 구분. 회원 권한은 일반회원, 대표운영자, 부운영자, 공급사로 권한이 구분됨. C : 일반회원 P : 대표 운영자 A : 부운영자 S : 공급사 DEFAULT C |
| 회원당 | max_usage_per_user | Promotion | Discountcodes | 2 | ✅ 핵심 UDS | 회원당 사용가능 횟수 DEFAULT 0 |
| 회원등급 | auto_update, auto_update_set_date, display_group, except_member_points, fixed_group, group_icon, member_group_discount_amount, membership_discount_amount, use_auto_update | Customer, Order, Privacy, Product, Store | Bundleproducts, Customergroups, Customergroups customers, Customergroups setting, Customers, Customers setting, Customersprivacy, Orders calculation, Products, Refunds | 14 | ✅ 핵심 UDS | 회원등급 고정 여부 특정 회원이 회원자동등급변경에 적용되지 않기 위한 등급 고정 여부 회원자동등급변경 기능을 사용하는 몰에서만 사용 가능하다. T : 고정함 F : 고정안함 DEFAULT F |
| 회원등급명 | group_name | Customer, Mileage | Credits, Customergroups, Points | 4 | ✅ 핵심 UDS | 회원등급명 ,(콤마)로 여러 건을 검색할 수 있다. |
| 회원등급번호 | group_no, member_group_no | Customer, Mileage, Notification, Order, Privacy, Promotion | Coupons issuancecustomers, Coupons issues, Customergroups, Customergroups customers, Customers, Customersprivacy, Orders, Points, Points report, Recipientgroups, Sms | 15 | ✅ 핵심 UDS | 회원등급번호 Youtube shopping 이용 시에는 미제공 해당 회원의 회원등급의 번호 |
| 회원등급할인 | member_grade_discount_amount | Order | Cancellation, Exchange, Return | 3 | ✅ 핵심 UDS | 회원등급할인 취소액 |
| 회원등급할인이 | show_group_coupon_to_non_members | Store | Coupons setting | 2 | ✅ 핵심 UDS | 회원등급할인이 지정된 쿠폰 포함 T : 포함 F : 미포함 |
| 회원아이디 | member_id | Community, Customer, Mileage, Notification, Order, Personal, Privacy, Promotion | Boards articles, Boards articles comments, Boards comments, Carts, Cashreceipt, Coupons issuancecustomers, Coupons issues, Credits, Customergroups customers, Customers, Customers autoupdate, Customers coupons | 54 | ✅ 핵심 UDS | 회원아이디 검색할 쇼핑몰 회원의 아이디. 개인정보 보호를 위해 전체 아이디를 입력해야 합니다.cellphone 또는 member_id 중 하나는 반드시 검색 조건으로 지정되어야 한다. ,(콤마)로 여러 건을 검색할 수 있다. |
| 회원여부 | member_type | Order | Orders | 1 | ✅ 핵심 UDS | 회원여부 회원여부. 회원과 비회원 각각의 코드가 있음. 2 : 회원 3 : 비회원 |
| 회원인증여부 | member_authentication | Customer, Order, Privacy | Customers, Customersprivacy, Orders | 3 | ✅ 핵심 UDS | 회원인증여부 회원 인증여부. 인증에 따라 회원은 4종류로 구분된다. 인증회원을 특별관리회원으로 설정할 경우 해당 회원은 가장 마지막에 설정한 특별관리회원으로 표시된다. T : 인증 F : 미인증 B : 특별관리회원 J : 14세미만회원 |
| 회원정보수정 | password_authentication | Store | Customers setting | 1 | ✅ 핵심 UDS | 회원정보수정 페이지 접속 시 비밀번호 인증 T:사용함 F:사용안함 |
| 회원타입 | member_type | Notification, Privacy | Customersprivacy, Recipientgroups | 4 | ✅ 핵심 UDS | 회원타입 Youtube shopping 이용 시에는 미제공 해당 회원의 회원 타입 vip : 특별관리회원 poor : 블랙리스트 pointfy : 통합멤버쉽 사용자 |
| 후불결제 | payment_confirmation | Order | Orders | 1 | ✅ 핵심 UDS | 후불결제 입금확인 가능 여부 T : 입금확인 F : 입금미확인 |
| 후불결제여부 | postpay | Order | Orders | 1 | ✅ 핵심 UDS | 후불결제여부 T : 후불결제 F : 후불결제 아님 |
| 휴대전화 | cellphone | Customer, Notification, Order, Privacy | Cashreceipt, Customers, Customersprivacy, Sms receivers | 7 | ✅ 핵심 UDS | 휴대전화 검색할 쇼핑몰 회원의 휴대전화번호. 개인정보 보호를 위해 전체 휴대전화번호를 입력해야 한다. cellphone 또는 member_id 중 하나는 반드시 검색 조건으로 지정되어야 한다. ,(콤마)로 여러 건을 검색할 수 있다. |
| 휴면회원 | account_reactivation_date | Privacy | Customersprivacy | 1 | ✅ 핵심 UDS | 휴면회원 해제일 |
| 희망배송사 | wished_carrier_id, wished_carrier_name | Order | Orders | 2 | ✅ 핵심 UDS | 희망배송사 아이디 ,(콤마)로 여러 건을 검색할 수 있다. |
| 희망배송시간 | wished_delivery_time | Order, Shipping | Orders, Orders receivers, Shipping | 4 | ✅ 핵심 UDS | 희망배송시간 Youtube shopping 이용 시에는 미제공 희망배송 시작시간(start_hour) 00~23 까지 입력 가능 희망배송 종료시간(end_hour) 00~23 까지 입력 가능 |
| 희망배송시작시간 | wished_delivery_start_hour | Order | Subscription shipments | 2 | ✅ 핵심 UDS | 희망배송시작시간 |
| 희망배송일 | wished_delivery, wished_delivery_date | Order, Shipping | Orders, Orders receivers, Shipping, Subscription shipments | 6 | ✅ 핵심 UDS | 희망배송일 사용여부 T : 사용함 F : 사용안함 DEFAULT F |
| 희망배송종료시간 | wished_delivery_end_hour | Order | Subscription shipments | 2 | ✅ 핵심 UDS | 희망배송종료시간 |
| 게시판 | admin_name, board_category_no, board_exposure_setting, board_guide, board_list, board_name, board_type, linked_board, og_board, password_rules, permission_board_manage, use_additional_board, use_board, use_nick_name_icon, use_writer_name_icon | Community, Store, Supply | Boards, Boards articles, Boards setting, Commenttemplates, Dashboard, Seo setting, Suppliers users, Users | 14 | 🟡 후보 | 게시판 닉네임 아이콘 노출 설정 공급사 운영자가 게시판에 게시글 작성시 별명 아이콘을 노출할 것인지 여부 표시 공급사 운영자 상세 조회 API에서만 확인 가능하다. |
| 게시판 문의내용에 대한 답변 메일 여부 | reply_mail | Community | Boards articles | 2 | 🟡 후보 | 1:1 게시판 문의내용에 대한 답변 메일 여부 Y : 사용함 N : 사용안함 DEFAULT N |
| 게시판 문의내용에 대한 답변여부 | reply | Community | Boards articles | 2 | 🟡 후보 | 1:1 게시판 문의내용에 대한 답변여부 T : 사용함 F : 사용안함 DEFAULT F |
| 게시판 번호 | board_no | Community | Boards, Boards articles, Boards articles comments, Boards comments, Boards seo | 10 | 🟡 후보 | 게시판 번호 |
| 공급사 | applicable_suppliers, supplier_code, supplier_product_name, supplier_regional_surcharge, supplier_selection, supplier_shipping_calculation, supplier_shipping_fee, supplier_transaction_type, supply_product_name, use_supplier, user_id | Notification, Order, Product, Shipping, Supply | Automails, Bundleproducts, Orders items, Products, Products approve, Shipping, Shipping suppliers, Suppliers, Suppliers users | 14 | 🟡 후보 | 공급사 운영자 아이디 공급사 운영자가 로그인할 경우 사용하는 로그인 아이디. 부운영자와 마찬가지로 쇼핑몰 관리자 화면에 로그인하면 공급사 관리자 화면에 접근할 수 있다. |
| 공급사 ID | supplier_id | Community, Notification, Order, Salesreport, Supply | Boards articles, Orders, Orders items, Reports salesvolume, Reservations, Shipping suppliers, Shipping suppliers additionalfees, Sms receivers, Suppliers users regionalsurcharges, Suppliers users regionalsurcharges setting | 16 | 🟡 후보 | 공급사 아이디 판매 수량 중 특정 공급사 ID로 등록된 수량 조회 |
| 공급사구조 | supplier_type | Supply | Suppliers | 2 | 🟡 후보 | 공급사구조 공급사의 영업 형태. 도매업체 : 최종 고객에게는 판매하지 않고 소매업체에 판매하는 업체 사입업체 : 도매업체로부터 물건을 구입해서 소매업체에 판매하는 업체 입점업체 : 쇼핑몰에 입점하여 판매중인 업체 WS : 도매업체 SF : 사입업체 BS : 입점업체 ET : 기타 DEFAULT WS |
| 공급사명 | supplier_name | Notification, Order, Supply | Orders items, Reservations, Sms receivers, Suppliers, Suppliers users | 8 | 🟡 후보 | 공급사명 공급사의 이름. 공급사명은 쇼핑몰 관리자 화면에서 공급사를 구분할 수 있는 기본적인 정보이다. ,(콤마)로 여러 건을 검색할 수 있다. |
| 공급사운영자명 | user_name | Supply | Suppliers users | 2 | 🟡 후보 | 공급사운영자명 공급사 운영자의 이름. 공급사 운영자 명은 공급사 운영자가 쇼핑몰 관리자 화면에서 어떤 작업을 할 경우 "작업을 실행한 사람(처리자)" 부분에 표시되는 이름을 의미한다. 공급사 운영자 상세 조회 API에서만 확인 가능하다. |
| 공급사유형 | trading_type | Supply | Suppliers | 2 | 🟡 후보 | 공급사유형 상품이 공급사에서 배송되는 형태. 사입 : 상품을 판매자가 구입하여 구매자에게 배송함. 직배송 : 상품에 주문이 들어오면 공급사가 구매자에게 바로 배송함. D : 사입 C : 직배송 DEFAULT D |
| 공급사정보 | show_supplier_info | Supply | Suppliers | 1 | 🟡 후보 | 공급사정보 표시 SP : 전화번호 SM : 사업장주소 MA : 시장주소 EA : 반품주소 MN : 담당자명 MI : 담당자연락처 |
| 내용 | content | Community, Notification, Order, Promotion, Store | Activitylogs, Boards articles, Boards articles comments, Boards comments, Commenttemplates, Commonevents, Information, Orders memos, Privacy boards, Privacy join, Privacy orders, Sms | 25 | 🟡 후보 | 자주 쓰는 답변 내용 |
| 멀티쇼핑몰 | multishop_access_authority | Store | Users | 1 | 🟡 후보 | 멀티쇼핑몰 접근 권한 T : 허용함 F : 허용안함 |
| 멀티쇼핑몰 번호 | shop_no | Application, Category, Collection, Community, Customer, Design, Mileage, Notification, Order, Personal, Privacy, Product, Promotion, Salesreport, Shipping, Store, Supply, Translation | Autodisplay, Automails, Automessages arguments, Automessages setting, Benefits, Benefits setting, Boards, Boards articles, Boards articles comments, Boards comments, Boards seo, Boards setting | 367 | 🟡 후보 | 멀티쇼핑몰 번호 멀티쇼핑몰 구분을 위해 사용하는 멀티쇼핑몰 번호. DEFAULT 1 |
| 메모 | memo, memo_no, memos | Customer, Notification, Order, Product, Store, Supply | Bundleproducts, Customers memos, Orders memos, Products, Products memos, Sms senders, Suppliers, Users | 16 | 🟡 후보 | 메모 번호 시스템에서 부여한 상품 메모의 고유한 번호. 상품 메모 번호는 쇼핑몰 내에서 중복되지 않는다. |
| 브랜드 | brand_code, brand_name, use_brand | Collection, Product | Brands, Products | 4 | 🟡 후보 | 브랜드 코드 브랜드를 등록하면 자동으로 생성되는 코드로 상품에 특정 브랜드를 지정할 때 사용. 미입력시 자체브랜드(B0000000) 사용 |
| 브랜드앱 | plusapp_member_join | Notification | Recipientgroups | 2 | 🟡 후보 | 브랜드앱 경로 가입회원 여부 T : 사용함 F : 사용안함 |
| 생성일시 | created_date | Application, Collection, Community, Customer, Design, Notification, Order, Personal, Privacy, Product, Promotion, Supply | Appstore orders, Benefits, Boards articles, Boards articles comments, Boards comments, Brands, Bundleproducts, Carts, Classifications, Commenttemplates, Coupons, Customerevents | 33 | 🟡 후보 | 혜택 등록일 해당 혜택이 등록된 일시 |
| 서비스문의/안내 | service_info, service_info_by_product | Product | Bundleproducts, Products | 4 | 🟡 후보 | 서비스문의/안내 제품의 사후 고객 서비스 방법 대한 안내 문구. HTML을 사용하여 입력이 가능하다. |
| 쇼핑몰 | basket_button_size, display_type, input_channel, mall_url, product_detail_button_size, terms_using_mall, use_dark_mode, use_signup_result_page | Category, Community, Store, Supply | Boards articles, Boards articles comments, Boards comments, Categories, Kakaopay setting, Policy, Socials kakaosync, Store, Suppliers | 15 | 🟡 후보 | 쇼핑몰 표시설정 해당 상품분류가 PC 쇼핑몰이나 모바일 쇼핑몰, 둘 다에 노출되는지 표시. A : PC + 모바일 P : PC M : 모바일 F : 모두 사용안함 |
| 쇼핑몰 ID | mall_id | Application, Store | Databridge logs, Socials navershopping, Store, Webhooks logs | 4 | 🟡 후보 | 상점 아이디 쇼핑몰 아이디. 대표운영자의 아이디이자, 쇼핑몰 기본 제공 도메인(mallid.cafe24.com)에 사용한다. |
| 쇼핑몰 대표 디자인 번호 멀티 | pc_skin_no | Store | Shops | 1 | 🟡 후보 | PC 쇼핑몰 대표 디자인 번호 멀티쇼핑몰의 PC 쇼핑몰 대표 디자인 번호. 현재 쇼핑몰에서 사용하고 있는 디자인 번호를 나타낸다. |
| 쇼핑몰명 | shop_name | Privacy, Store | Customersprivacy, Shops, Store | 3 | 🟡 후보 | 쇼핑몰명 해당 상점의 쇼핑몰명([쇼핑몰 설정 > 기본 설정 > '쇼핑몰 정보 > 내 쇼핑몰 정보']) |
| 수정일시 | updated_date | Application, Design, Order, Product, Salesreport, Supply | Bundleproducts, Orders buyer, Orders buyer history, Orders receivers history, Products, Reports salesvolume, Scripttags, Suppliers, Themes | 9 | 🟡 후보 | 최종 데이터 갱신 시간 판매 수량 통계 데이터가 갱신된 시간 표시 |
| 작성자 | author_display, author_id, author_protection, client_ip, ip, use_writer_block, writer, writer_email | Community, Customer, Order, Product | Boards, Boards articles, Boards articles comments, Boards comments, Customers memos, Orders memos, Products memos, Urgentinquiry | 13 | 🟡 후보 | 작성자 표시 설정 N : 이름 U : 별명(별명기입전 이름으로 노출) I : 별명(별명기입전 아이디로 노출) |
| 적립금 | allow_point_payment, allow_using_coupons_with_points, amount, available_min_point, available_min_price, available_points_decrease, available_points_increase, available_points_max, available_points_min, case, collect_points, display_type, format, include_point_usage, issue_date, mileage_used, name, payment_period, point_issuance_standard, points_amount, points_by_product, points_category, points_information, points_spent_amount, refund_point, round_type, round_unit, type, used_points | Customer, Mileage, Notification, Order, Product, Salesreport, Store | Benefits setting, Bundleproducts, Coupons setting, Customergroups, Orders, Orders calculation, Orders migrations, Points, Points setting, Products, Recipientgroups, Refunds | 24 | 🟡 후보 | 적립금 타입 적립금 타입 지정 없이 전체 조회시에는 D: 적립금 환불 타입은 제외되고 조회 되므로, 적립금 환불 타입을 조회하려면 타입을 지정해야 합니다. A : 관리자 직접 적립금 부여 B : 주문취소로 인한 환불시 환불금을 적립금으로 부여 C : 적립대기중이던 적립금 취소 D : 반품완료 후 사용가능 E : csv파일로 등록된 회원 F : 주문취소로 인해 상품에 대한 적립금 차감 G : 추천한 신규 가입자에게 적립금 부여 H : (기존 적립금 내역용 레거시 타입) 주문시 회원등급에 따른 적립금 부여(회원 등급 적립금) I : 주문취소로 인해 회원등급에 대한 적립금 환불 J : 주문취소로 인해 쿠폰에 대한 적립금 환불 K : 주문시 회원등급에 따른 적립금 부여(회원 등급 적립금) L : 주문시 사용한 쿠폰에 따른 적립금 부여(쿠폰 적립금) M : 상품구매시 사용한 적립금 N : 신규가입시 적립금 부여 O : 적립금 즉시지급 쿠폰(온라인/시리얼) P : 주문시 구매한 상품에 대한 적 |
| 정기쿠폰 | recurring_issuance, recurring_issuance_day, recurring_issuance_hour, recurring_issuance_interval, recurring_issuance_minute | Promotion | Coupons | 2 | 🟡 후보 | 정기쿠폰 발급 단위 |
| 제목 | title | Application, Community, Notification | Appstore payments, Boards articles, Commenttemplates, Sms, Urgentinquiry | 7 | 🟡 후보 | 결제 명 앱스토어 주문의 주문 이름. 주문 생성시 지정이 가능하며, 사용자가 결제시 해당 결제의 내용이 무엇인지 알 수 있는 내용이어야 함. |
| 제조사 | manufacturer_code, use_manufacturer | Collection, Product | Manufacturers, Products | 4 | 🟡 후보 | 제조사 코드 제조사를 등록하면 자동으로 생성되는 코드로 상품에 특정 제조사를 지정할 때 사용. 미입력시 자체제작(M0000000) 사용 |
| 제조사명 | manufacturer_name | Collection | Manufacturers | 2 | 🟡 후보 | 제조사명 제조사의 이름. 제조사명은 쇼핑몰 관리자 화면에서 제조사를 구분할 수 있는 기본적인 정보이다. |
| 참조화폐 | use_reference_currency | Store | Shops | 1 | 🟡 후보 | 참조화폐 사용여부 |
| 카테고리 | categories, category_no, use_category | Community, Product, Promotion | Boards, Categories properties, Commonevents | 6 | 🟡 후보 | 카테고리 기능 사용여부 T : 사용함 F : 사용안함 |
| 쿠폰 | available_coupon, available_date, available_issue_type, coupon_direct_url, coupon_discount_amount, coupon_discount_price, coupon_image_path, coupon_image_type, coupon_percent, coupon_value, coupons, expiration_notice_date_setting, is_stopped_issued_coupon, issue_no, issue_quantity_min, issue_quntity_type, issued_date, max_coupon_count, pause_begin_date, pause_begin_datetime, pause_end_date, pause_end_datetime, recover_coupon, recover_coupon_setting, send_email_for_issue, status, use_coupon, used_coupon, used_date | Order, Promotion, Salesreport, Store | Benefits, Cancellation, Coupons, Coupons issuancecustomers, Coupons issues, Coupons setting, Customers coupons, Orders, Orders calculation, Orders cancellation, Orders coupons, Orders return | 26 | 🟡 후보 | 쿠폰 완전삭제 (발급된 쿠폰 사용정지) 여부 쿠폰이 완전 삭제되었는지 여부. 쿠폰이 완전 삭제되면 기존에 발급된 쿠폰도 더 이상 사용이 불가함. T : 완전삭제 F : 완전삭제 아님 |
| 쿠폰명 | coupon_name | Order, Promotion | Coupons, Customers coupons, Orders coupons, Serialcoupons | 6 | 🟡 후보 | 쿠폰명 쿠폰의 이름 |
| 쿠폰발급 | issue_count_per_once, issue_order_end_date, issue_order_start_date, send_sms_for_issue | Promotion | Coupons, Coupons issues, Serialcoupons | 4 | 🟡 후보 | 쿠폰발급 SMS 발송 여부 쿠폰 발급정보를 SMS로 발송할지 여부 EC 일본, 베트남, 필리핀 버전에서는 사용할 수 없음. T : 발송함 F : 발송안함 DEFAULT F |
| 쿠폰번호 | coupon_code, coupon_no | Order, Promotion | Coupons, Coupons issuancecustomers, Coupons issues, Customers coupons, Orders coupons, Serialcoupons, Serialcoupons issues | 13 | 🟡 후보 | 쿠폰번호 |
| 쿠폰삭제 | deleted | Promotion | Coupons, Serialcoupons, Serialcoupons issues | 5 | 🟡 후보 | 쿠폰삭제 여부 쿠폰이 삭제되었는지 여부. ,(콤마)로 여러 건을 검색할 수 있다. T : 삭제된 쿠폰 F : 삭제되지 않은 쿠폰 DEFAULT F |
| 쿠폰설명 | coupon_description | Promotion | Coupons, Serialcoupons | 2 | 🟡 후보 | 쿠폰설명 쿠폰의 설명 |
| 쿠폰유형 | coupon_type | Promotion | Coupons | 2 | 🟡 후보 | 쿠폰유형 쿠폰유형. 온라인 쿠폰과 오프라인 시리얼 쿠폰 유형이 있음. O : 온라인 쿠폰 S : 오프라인 시리얼 쿠폰 |
| 쿠폰적용 | available_category, available_category_list, available_product, available_product_list | Promotion | Coupons, Serialcoupons | 4 | 🟡 후보 | 쿠폰적용 상품 선택 쿠폰의 적용가능 상품 선택. 특정 상품을 제외하거나, 적용하거나 혹은 모든 상품에 대해서 쿠폰적용 여부를 선택할 수 있음. |
| 쿠폰할인 | coupon_discount_amount | Order | Cancellation, Exchange, Orders shippingfeecancellation, Return | 4 | 🟡 후보 | 쿠폰할인 취소액 |
| 쿠폰혜택 | benefit_text | Promotion | Coupons, Serialcoupons | 2 | 🟡 후보 | 쿠폰혜택 상세내역 출력 쿠폰혜택의 상세 내역이 출력됨. |
| 파일 내용 | auth_key_file_contents | Store | Socials apple | 1 | 🟡 후보 | Auth Key 파일 내용 .p8파일을 텍스트 파일로 열어 줄바꿈 없이 값을 작성 |
| 화폐단위 | currency | Application, Order | Appstore orders, Appstore payments, Orders, Refunds | 5 | 🟡 후보 | 화폐단위 KRW : ￦ 원 USD : $ 달러 JPY : ¥ 엔 PHP : ₱ 페소 |
| 1회 | single_issue_per_once | Promotion | Coupons issues | 1 | ⚪ 선택 | 1회 발급시 1장만 발급할지 여부 쿠폰을 발급할 때 1회 발급시 1장만 발급할지 여부 T : 1장씩 발급 F : 동시발행수량 설정만큼 발급 DEFAULT T |
| HS코드 | hs_code, hscode | Order, Product, Shipping, Supply | Bundleproducts, Orders items, Products, Shipping, Shipping suppliers | 9 | ⚪ 선택 | HS코드 해외 배송시 관세 부과를 위해 사용하는 HS코드. 국제 배송시 통관을 위해 반드시 정확한 번호를 입력해야 함. ※ HS코드 : 세계무역기구(WTO) 및 세계관세기구(WCO)가 무역통계 및 관세분류의 목적상 수출입 상품을 숫자 코드로 분류화 한 것으로, 수입 시 세금부과와 수출품의 통제 및 통계를 위한 분류법 |
| PG사 | etc_code, hash_code, partner_id, payment_gateway_name, pg_shipping_registration | Order, Salesreport, Store | Cashreceipt, Financials dailysales, Financials monthlysales, Financials paymentgateway, Payment setting, Paymentgateway, Paymentservices | 10 | ⚪ 선택 | PG사 배송등록 A : 자동 등록(매일 오후 8시 수집) M : 수동 등록 |
| add_category_no | add_category_no | Product | Bundleproducts, Products | 2 | ⚪ 선택 |  |
| additional_information | additional_information | Privacy, Product, Store | Bundleproducts, Customersprivacy, Paymentgateway, Products | 4 | ⚪ 선택 |  |
| additional_options | additional_options | Order, Product | Orders items options, Products options | 2 | ⚪ 선택 |  |
| address1 | address1 | Collection, Order, Privacy, Shipping, Store, Supply | Customersprivacy, Manufacturers, Orders receivers, Orders receivers history, Shippingorigins, Store, Suppliers | 12 | ⚪ 선택 | 기본 주소 Youtube shopping 이용 시에는 미제공 |
| admin_reply_fixed | admin_reply_fixed | Community | Boards | 1 | ⚪ 선택 |  |
| admin_title_fixed | admin_title_fixed | Community | Boards | 1 | ⚪ 선택 |  |
| attach_file_urls | attach_file_urls | Community | Boards articles, Boards articles comments, Urgentinquiry reply | 3 | ⚪ 선택 |  |
| author_protection | author_protection | Community | Boards | 1 | ⚪ 선택 |  |
| available_begin_datetime | available_begin_datetime | Promotion | Coupons, Customers coupons, Serialcoupons | 5 | ⚪ 선택 | 사용 기간 시작 일시 available_period_type이 'F'로 입력된 경우만 필수 입력 |
| available_datetime | available_datetime | Promotion | Coupons, Serialcoupons | 2 | ⚪ 선택 | 해당 날짜에 발급 가능한 쿠폰 검색 해당하는 날짜에 발급 가능한 쿠폰 검색 available_period_type이 F일 때만 유효 |
| available_day_from_issued | available_day_from_issued | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 사용 가능 일수 available_period_type이 'R'로 입력된 경우만 필수 입력 |
| available_end_datetime | available_end_datetime | Promotion | Coupons, Customers coupons, Serialcoupons | 5 | ⚪ 선택 | 사용 기간 종료 일시 available_period_type이 'F'로 입력된 경우만 필수 입력 |
| available_min_price | available_min_price | Promotion | Coupons, Customers coupons, Serialcoupons | 5 | ⚪ 선택 | 사용가능 구매 금액 쿠폰을 사용가능한 구매 금액 |
| available_order_price_type | available_order_price_type | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 사용가능 구매 금액 상세 유형 U : 모든 상품의 주문 금액 I : 쿠폰 적용 상품의 주문 금액 |
| available_payment_method | available_payment_method | Promotion | Coupons, Serialcoupons | 3 | ⚪ 선택 | 사용가능 결제수단 all : 제한없음 R : 무통장입금 E : 가상계좌 C : 신용카드 A : 계좌이체 H : 휴대폰 M : 적립금 K : 케이페이 P : 페이나우 N : 페이코 O : 카카오페이 S : 스마일페이 V : 네이버페이 B : 편의점 D : 토스 |
| available_payment_methods | available_payment_methods | Promotion | Customers coupons | 1 | ⚪ 선택 | 사용가능 결제수단 all : 제한없음 R : 무통장입금 E : 가상계좌 C : 신용카드 A : 계좌이체 H : 휴대폰 M : 적립금 K : 케이페이 P : 페이나우 N : 페이코 O : 카카오페이 S : 스마일페이 V : 네이버페이 B : 편의점 D : 토스 |
| available_period_type | available_period_type | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 사용기간 유형 쿠폰 사용기간의 유형 ,(콤마)로 여러 건을 검색할 수 있다. F : 일반 기간 R : 쿠폰 발급일 기준 M : 당월 말까지 사용 |
| available_price_type | available_price_type | Promotion | Coupons, Customers coupons, Serialcoupons | 5 | ⚪ 선택 | 사용가능 구매 금액 유형 쿠폰의 사용가능 금액에 대한 기준. 상품 금액 기준일 경우 상품 가격에 수량을 곱한 금액을 기준으로 하며, 주문 금액 기준일 경우 해당 금액에 기타 할인, 배송비가 적용된 금액을 기준으로 계산한다. U : 제한 없음 O : 주문 금액 기준 P : 상품 금액 기준 |
| available_price_type_detail | available_price_type_detail | Promotion | Customers coupons | 1 | ⚪ 선택 | 사용가능 구매 금액 유형 상세 U : 모든 상품의 주문 금액 I : 쿠폰 적용 상품의 주문 금액 |
| available_site | available_site | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 사용 범위 유형 발급한 쿠폰의 사용 가능한 주문 경로 W : 웹 쇼핑몰 전용 M : 모바일 쇼핑몰 전용 P : 브랜드앱 전용 |
| available_user | available_user | Promotion | Discountcodes | 2 | ⚪ 선택 | 사용가능 대상 M : 회원 A : 전체 DEFAULT A |
| benefit_end_date | benefit_end_date | Promotion | Benefits | 1 | ⚪ 선택 | 검색 종료일 |
| benefit_start_date | benefit_start_date | Promotion | Benefits | 1 | ⚪ 선택 | 검색 시작일 |
| bulk_purchase_sale | bulk_purchase_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| bundle_additional_options | bundle_additional_options | Order | Orders items options | 1 | ⚪ 선택 |  |
| bundle_product_components | bundle_product_components | Product | Bundleproducts | 1 | ⚪ 선택 |  |
| bundle_product_sales | bundle_product_sales | Product | Bundleproducts | 1 | ⚪ 선택 |  |
| buyer | buyer | Order | Orders migrations | 1 | ⚪ 선택 |  |
| cancel_request | cancel_request | Order | Payments | 1 | ⚪ 선택 |  |
| change_default_shipping_address | change_default_shipping_address | Order | Orders receivers | 2 | ⚪ 선택 | 기본배송지 변경 여부 T : 변경함 F : 변경안함 DEFAULT F |
| comment_author_protection | comment_author_protection | Community | Boards | 1 | ⚪ 선택 |  |
| comment_no | comment_no | Community | Commenttemplates | 1 | ⚪ 선택 | 해당 댓글번호 이후 검색 |
| country_hscode | country_hscode | Supply | Shipping suppliers | 1 | ⚪ 선택 |  |
| country_shipping_fee_list | country_shipping_fee_list | Shipping | Shipping | 1 | ⚪ 선택 |  |
| created_end_date | created_end_date | Promotion | Coupons, Serialcoupons | 2 | ⚪ 선택 | 검색 종료일 쿠폰 생성일 기준 검색의 검색 종료일 검색 시작일과 같이 사용해야함. |
| created_start_date | created_start_date | Promotion | Coupons, Serialcoupons | 2 | ⚪ 선택 | 검색 시작일 쿠폰 생성일 기준 검색의 검색 시작일 검색 종료일과 같이 사용해야함. |
| credit_used | credit_used | Order | Cancellation, Exchange, Orders shippingfeecancellation, Return | 4 | ⚪ 선택 | 사용된 예치금 반환액 |
| custom_properties | custom_properties | Product | Products, Products customproperties | 2 | ⚪ 선택 | 사용자 정의 속성 |
| date_type | date_type | Notification, Order, Privacy | Customersprivacy, Orders, Orders paymenttimeline, Recipientgroups, Refunds, Reservations, Subscription shipments | 8 | ⚪ 선택 | 검색날짜 유형 검색을 위한 날짜 유형 기준. 기본값은 주문일로 설정되어 있음. order_date : 주문일 pay_date : 결제일 shipbegin_date : 배송시작일 shipend_date : 배송완료일 cancel_date : 주문취소일 place_date : 발주일 cancel_request_date : 취소신청일 cancel_accept_date : 취소접수일 cancel_complete_date : 취소완료일 exchange_request_date : 교환신청일 exchange_accept_date : 교환접수일 exchange_complete_date : 교환완료일 return_request_date : 반품신청일 return_accept_date : 반품접수일 return_complete_date : 반품완료일 purchaseconfirmation_date : 구매확정일 DEFAULT order_date |
| default_shipping_carrier | default_shipping_carrier | Shipping | Carriers | 2 | ⚪ 선택 | 기본배송사 여부 T : 사용함 F : 사용안함 DEFAULT T |
| default_shipping_fee | default_shipping_fee | Order, Shipping | Carriers, Orders shippingfeecancellation | 3 | ⚪ 선택 | 기본 배송비 |
| delete_default_carrier | delete_default_carrier | Shipping | Carriers | 1 | ⚪ 선택 | 기본배송사 삭제 여부 T : 삭제함 F : 삭제안함 DEFAULT F |
| discount_amount | discount_amount | Promotion | Coupons, Serialcoupons | 2 | ⚪ 선택 |  |
| discount_rate | discount_rate | Promotion | Coupons, Serialcoupons | 2 | ⚪ 선택 |  |
| end_month | end_month | Community, Salesreport | Financials monthlyreviews, Financials monthlysales | 2 | ⚪ 선택 | 검색 종료월 |
| exchange_items | exchange_items | Order | Exchangerequests | 1 | ⚪ 선택 |  |
| expiration_date | expiration_date | Product | Products | 1 | ⚪ 선택 |  |
| gift | gift | Promotion | Benefits | 1 | ⚪ 선택 |  |
| gift_product_bundle | gift_product_bundle | Promotion | Benefits | 1 | ⚪ 선택 |  |
| hit | hit | Community | Boards articles, Urgentinquiry | 2 | ⚪ 선택 | 조회수 |
| image_list | image_list | Product | Products decorationimages, Products icons | 2 | ⚪ 선택 |  |
| input_form | input_form | Community | Boards | 1 | ⚪ 선택 |  |
| issued_end_date | issued_end_date | Promotion | Coupons issues | 1 | ⚪ 선택 | 검색 종료일 |
| issued_start_date | issued_start_date | Promotion | Coupons issues | 1 | ⚪ 선택 | 검색 시작일 |
| items | items | Order | Cancellation, Cancellationrequests, Exchange, Exchangerequests, Orders calculation, Orders cancellation, Orders exchange, Orders migrations, Orders return, Orders shortagecancellation, Return, Returnrequests | 13 | ⚪ 선택 |  |
| keyword | keyword | Community, Mileage, Privacy, Store | Boards articles, Credits, Credits report, Customersprivacy, Urgentinquiry, Users | 6 | ⚪ 선택 | 검색어 Youtube shopping 이용 시에는 미제공 조회하고자 하는 회원의 검색필드에 대한 검색어를 입력함. ex) search_field : mail keyword : cafe24@cafe24.com ,(콤마)로 여러 건을 검색할 수 있다. |
| links | links | Community, Shipping | Boards comments, Carriers | 2 | ⚪ 선택 | link |
| manager_information | manager_information | Supply | Suppliers | 1 | ⚪ 선택 |  |
| member_sale | member_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| multi_invoice | multi_invoice | Order | Orders items | 1 | ⚪ 선택 |  |
| new_product_sale | new_product_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| nick_name | nick_name | Supply | Suppliers users | 1 | ⚪ 선택 |  |
| option_value_default | option_value_default | Order | Orders items, Reservations | 2 | ⚪ 선택 | 기본옵션값 |
| options | options | Product | Products, Products options | 2 | ⚪ 선택 |  |
| original_options | original_options | Product | Products options | 1 | ⚪ 선택 |  |
| oversea_additional_fee_list | oversea_additional_fee_list | Shipping | Shipping | 1 | ⚪ 선택 |  |
| oversea_shipping_country_list | oversea_shipping_country_list | Shipping | Shipping | 1 | ⚪ 선택 |  |
| package_volume | package_volume | Shipping | Shipping | 1 | ⚪ 선택 |  |
| period_sale | period_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| pickup | pickup | Order | Exchangerequests, Orders exchange, Orders return, Return, Returnrequests | 5 | ⚪ 선택 |  |
| point_used | point_used | Order | Cancellation, Exchange, Orders shippingfeecancellation, Return | 4 | ⚪ 선택 | 사용된 적립금 반환액 |
| points_amount | points_amount | Product | Products | 1 | ⚪ 선택 |  |
| product_name_default | product_name_default | Order | Orders items, Reservations | 2 | ⚪ 선택 | 기본 상품명 |
| product_volume | product_volume | Product | Products | 1 | ⚪ 선택 |  |
| properties | properties | Customer, Product | Categories properties, Customers properties, Mains properties, Products properties | 4 | ⚪ 선택 |  |
| property | property | Product | Categories properties, Mains properties, Products properties | 3 | ⚪ 선택 |  |
| receivers | receivers | Order | Orders migrations | 1 | ⚪ 선택 |  |
| recurring_issuance | recurring_issuance | Promotion | Coupons | 1 | ⚪ 선택 |  |
| relational_product | relational_product | Product | Bundleproducts, Products | 2 | ⚪ 선택 |  |
| repurchase_sale | repurchase_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| return_address | return_address | Shipping | Shipping | 1 | ⚪ 선택 |  |
| search | search | Community | Boards articles | 1 | ⚪ 선택 | 검색 영역 subject : 제목 content : 내용 writer_name : 작성자 product : 상품명 member_id : 회원 아이디 |
| search_date | search_date | Promotion | Customerevents | 1 | ⚪ 선택 | 검색 기준일 created_date: 이벤트 생성일 start_date: 이벤트 시작일 end_date: 이벤트 종료일 DEFAULT created_date |
| search_engine_exposure | search_engine_exposure | Category, Product | Categories seo, Products seo | 4 | ⚪ 선택 | 검색 엔진 노출 설정 해당 상품을 검색엔진에 노출할 것인지 설정. '노출안함'으로 설정할 경우 해당 상품이 검색엔진에 노출되지 않는다. T : 사용함 F : 사용안함 |
| search_field | search_field | Mileage, Privacy | Credits, Credits report, Customersprivacy | 3 | ⚪ 선택 | 검색필드 Youtube shopping 이용 시에는 미제공 조회하고자 하는 회원의 검색필드. id : 아이디 name : 이름 hp : 핸드폰 tel : 전화번호 mail : 이메일 shop_name : 상호명 |
| search_keyword | search_keyword | Collection | Brands | 2 | ⚪ 선택 | 검색어 설정 |
| search_type | search_type | Community, Privacy, Store | Customersprivacy, Urgentinquiry, Users | 3 | ⚪ 선택 | 검색 타입 Youtube shopping 이용 시에는 미제공 회원 검색을 회원정보 기반으로 할지 가입일 기준으로 할지 선택하여 검색할 수 있다. 가입일 기준으로 검색할 경우 offset과 관계 없이 전체 회원을 검색할 수 있다. ※ 가입일 기준 사용시 created_start_date 외의 모든 검색 조건은 사용할 수 없다. customer_info : 회원정보 기반 검색 created_date : 가입일 기준 검색 DEFAULT customer_info |
| serial_generate_auto | serial_generate_auto | Promotion | Serialcoupons | 1 | ⚪ 선택 |  |
| shipping_company_type | shipping_company_type | Shipping | Shipping | 1 | ⚪ 선택 |  |
| shipping_fee_sale | shipping_fee_sale | Promotion | Benefits | 1 | ⚪ 선택 |  |
| shipping_fee_setting_detail | shipping_fee_setting_detail | Shipping | Carriers | 1 | ⚪ 선택 |  |
| shipping_period | shipping_period | Product, Shipping | Bundleproducts, Products, Shipping | 3 | ⚪ 선택 |  |
| shipping_rates | shipping_rates | Product, Shipping, Supply | Products, Shipping, Shipping suppliers | 3 | ⚪ 선택 |  |
| since_comment_no | since_comment_no | Community | Boards comments | 1 | ⚪ 선택 | 해당 댓글번호 이후 검색 |
| since_issue_no | since_issue_no | Promotion | Coupons issues | 1 | ⚪ 선택 | 해당 쿠폰 발급번호 이후 검색 특정 쿠폰발급 이후의 쿠폰을 검색. 해당 검색조건 사용시 offset과 관계 없이 모든 쿠폰 발급번호를 검색할 수 있다. ※ 해당 검색 조건 사용시 다음 파라메터로는 사용할 수 없다. offset |
| since_member_id | since_member_id | Promotion | Coupons issuancecustomers | 1 | ⚪ 선택 | 해당 쿠폰 회원 ID 이후 검색 |
| since_product_no | since_product_no | Product | Products | 1 | ⚪ 선택 | 해당 상품번호 이후 검색 특정 상품번호 이후의 상품들을 검색. 해당 검색조건 사용시 offset과 관계 없이 모든 상품을 검색할 수 있다. ※ 해당 검색 조건 사용시 다음 파라메터로는 사용할 수 없다. product_no sort order offset |
| size_guide | size_guide | Product | Products | 1 | ⚪ 선택 |  |
| spam_auto_prevention | spam_auto_prevention | Community, Store | Boards, Boards setting | 2 | ⚪ 선택 |  |
| start_month | start_month | Community, Salesreport | Financials monthlyreviews, Financials monthlysales | 2 | ⚪ 선택 | 검색 시작월 |
| use_classification | use_classification | Collection | Classifications | 2 | ⚪ 선택 | 사용여부 |
| use_manufacturer | use_manufacturer | Collection | Manufacturers | 2 | ⚪ 선택 | 사용여부 해당 제조사를 사용하는지 여부 표시 T : 사용함 F : 사용안함 |
| use_supplier | use_supplier | Supply | Suppliers | 2 | ⚪ 선택 | 사용여부 해당 공급사를 사용하는지 여부 표시 T : 사용함 F : 사용안함 DEFAULT T |
| used_credits | used_credits | Order | Refunds | 1 | ⚪ 선택 | 사용된 예치금 반환액 |
| used_datetime | used_datetime | Promotion | Serialcoupons issues | 1 | ⚪ 선택 | 사용일시 |
| used_points | used_points | Customer, Order, Privacy | Customers, Customersprivacy, Refunds | 3 | ⚪ 선택 | 사용된 적립금 반환액 |
| user_name | user_name | Supply | Suppliers users | 1 | ⚪ 선택 |  |
| wished_delivery_time | wished_delivery_time | Order | Orders receivers | 1 | ⚪ 선택 |  |
| write_permission_extra | write_permission_extra | Community | Boards | 1 | ⚪ 선택 |  |
| 가능한 | use_fast_delivery_date, use_fast_delivery_time, wished_delivery_hour_asap | Order | Orders receivers, Subscription shipments | 4 | ⚪ 선택 | 가능한 빠른 배송일 설정 여부 Youtube shopping 이용 시에는 미제공 가능한 빠른 배송시간 설정 여부'가 'T' 일때는 null 로 응답함 T: 사용함 F: 사용안함 |
| 가용 | available_credits, available_points, available_points_decrease, available_points_increase, available_points_total | Customer, Mileage, Privacy | Customers, Customersprivacy, Points, Points report | 4 | ⚪ 선택 | 가용 적립금 증가 |
| 개수 | count | Community, Promotion | Coupons issues, Financials monthlyreviews, Urgentinquiry reply | 3 | ⚪ 선택 | 리뷰 개수 합계 |
| 거래개시일 | account_start_date | Supply | Suppliers | 2 | ⚪ 선택 | 거래개시일 |
| 거래상품 | business_item | Supply | Suppliers | 2 | ⚪ 선택 | 거래상품 유형 공급사와 거래하는 상품의 유형 정보. |
| 거래중지일 | account_stop_date | Supply | Suppliers | 2 | ⚪ 선택 | 거래중지일 |
| 거부 | reject_reason | Order | Cancellationrequests, Exchangerequests, Orders exchangerequests, Returnrequests | 4 | ⚪ 선택 | 거부 사유 고객에게 노출되는 접수 거부 사유 |
| 게시 | display, is_display | Community | Boards articles | 3 | ⚪ 선택 | 게시 여부 T : 게시함 F : 게시안함 |
| 게시글 | admin_title_fixed, input_form, password, use_report | Community | Boards, Boards articles | 3 | ⚪ 선택 | 게시글 신고기능 사용 여부 T : 사용함 F : 사용안함 |
| 게시글 번호 | article_no | Community | Boards articles, Boards articles comments, Boards comments, Urgentinquiry, Urgentinquiry reply | 8 | ⚪ 선택 | 게시물 번호 ,(콤마)로 여러 건을 검색할 수 있다. |
| 게시물 | article_display_type, article_type, input_channel | Community | Boards, Boards articles, Urgentinquiry | 6 | ⚪ 선택 | 게시물 유형 ,(콤마)로 여러 건을 검색할 수 있다. all : 전체 normal : 일반글 notice : 공지글 fixed : 고정글 |
| 계좌번호 | accounts, bank_account_no | Order, Store, Supply | Orders, Store accounts, Suppliers, Unpaidorders | 4 | ⚪ 선택 | 계좌번호 공급사 정산시 사용하는 계좌의 계좌 번호 |
| 고정 | fixed_sort | Product | Categories products, Mains products | 3 | ⚪ 선택 | 고정 여부 T : 진열순위 고정 사용함 F : 진열순위 고정 사용안함 |
| 고정글 | fixed | Community | Boards articles | 2 | ⚪ 선택 | 고정글 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 공급가액 | supply_price | Order | Cashreceipt | 1 | ⚪ 선택 | 공급가액 |
| 공지 | is_notice, notice | Community | Boards articles | 3 | ⚪ 선택 | 공지 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 과세 | tax_amount, tax_type | Order, Product | Orders calculation, Products | 3 | ⚪ 선택 | 과세 구분 해당 상품의 과세 정보. 해당 상품의 부가세 포함 유형. 과세상품 = 세금이 부과된 상품. 면세상품 = 세금이 면제되는 상품. 가공되지 않은 농/수/축산물, 연탄, 도서류, 보험, 여성용품 등의 상품이 이에 해당하며, 과세사업자로 등록해야 함 영세상품 = 부가세가 0%로 적용되는 수출용 외화 획득 상품 tax_calculation이 A(자동계산)이면서, C(영세상품) 일 경우 'A(과세상품)'으로 반환. A : 과세상품 B : 면세 상품 C : 영세상품 |
| 과세율 | tax_rate | Order, Product | Orders items, Products | 3 | ⚪ 선택 | 과세율 |
| 관련 | related_order_id | Promotion | Coupons issuancecustomers, Coupons issues | 2 | ⚪ 선택 | 관련 주문번호 |
| 관련상품 | relational_product | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 관련상품 Youtube shopping 이용 시에는 미제공 해당 상품과 비슷한 상품 혹은 대체 가능한 상품. 관련 상품 등록시 해당 상품의 상세페이지 하단에 노출된다. |
| 관리자 | add_memo_too, admin_additional_amount, admin_confirm, admin_id, admin_name, manually_input_amount | Community, Mileage, Order | Boards, Cancellation, Credits, Credits report, Exchange, Orders, Orders cancellation, Orders exchange, Orders payments, Orders return, Orders shortagecancellation, Points | 23 | ⚪ 선택 | 관리자 메모에도 추가 오픈마켓/네이버페이/카카오페이 주문을 취소할 경우 사용 불가 T : 사용함 F : 사용안함 DEFAULT F |
| 관리자명 | admin_name, manager_name | Order, Store | Orders items history, Store | 2 | ⚪ 선택 | 관리자명 쇼핑몰의 대표운영자의 이름 |
| 구간별 | shipping_rates | Product | Bundleproducts, Products | 2 | ⚪ 선택 | 구간별 배송비 개별배송비를 사용할 경우 상품의 개별 배송비. shipping_fee_type이 R, N일 경우 배열 안에 shipping_fee를 정의하여 배송비를 설정할 수 있다. shipping_fee_type이 M, D, W, C일 경우 배열 안에 다음과 같이 정의하여 배송비 구간을 설정할 수 있다. shipping_rates_min : 배송비 구간 시작 기준 shipping_rates_max : 배송비 구간 종료 기준 shipping_fee : 배송비 shipping_calculation이 A(자동계산)일 경우 null로 반환. |
| 구매 | buy_limit_type, review_button_mode, standard_purchase_amount, standard_purchase_count | Customer, Store | Boards setting, Customergroups setting, Orderform setting | 5 | ⚪ 선택 | 구매 금액 정의 total_order_amount : 총 주문 금액 total_paid_amount : 총 결제 금액 credit_price : 총실결제금액 + 예치금 |
| 구매가능 | buy_group_list, buy_member_id_list | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 구매가능 회원 등급 Youtube shopping 이용 시에는 미제공 |
| 구매단위 | buy_unit, buy_unit_type | Product | Products | 2 | ⚪ 선택 | 구매단위 타입 해당 상품의 구매 단위를 1개 이상으로 설정한 경우 해당 구매 단위를 품목 단위로 할 것인지, 상품 단위로 할 것인지에 대한 설정 P : 상품 기준 O : 품목 기준 DEFAULT O |
| 구매시 | buy_benefits | Customer | Customergroups | 1 | ⚪ 선택 | 구매시 할인/적립 혜택 F : 혜택없음 D : 구매금액 할인 M : 적립금 지급 P : 할인/적립 동시 적용 |
| 구매제한 | buy_limit_by_product, buy_limit_type | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 구매제한 Youtube shopping 이용 시에는 미제공 N : 회원만 구매하며 구매버튼 감추기 M : 회원만 구매하며 구매버튼 보이기 F : 구매제한 안함 O : 지정된 회원만 구매하며 구매버튼 감추기 D : 지정된 회원만 구매하며 구매버튼 보이기 DEFAULT F |
| 구매확정 | purchase_confirmation, purchase_confirmation_auto_check_day, purchase_confirmation_auto_check_set_date, purchase_confirmation_button_set_date, use_purchase_confirmation_auto_check, use_purchase_confirmation_button | Order, Store | Orders, Orders setting | 4 | ⚪ 선택 | 구매확정 자동체크 사용여부 T : 사용함 F : 사용안함 |
| 구매확정일 | purchaseconfirmation_date | Order | Orders items | 1 | ⚪ 선택 | 구매확정일 |
| 구분 | claim_reason_type, type | Order, Store | Activitylogs, Cancellation, Exchange, Orders shippingfeecancellation, Return | 6 | ⚪ 선택 | 구분 판매자의 반품 접수 사유 구분. 구매자의 반품 신청 사유는 items(품목 주문) > claim_reason_type으로 조회할 수 있다. A:고객변심 B:배송지연 J:배송오류 C:배송불가지역 L:수출/통관 불가 D:포장불량 E:상품 불만족 F:상품정보상이 K:상품불량 G:서비스불만족 H:품절 I:기타 |
| 국가명 | country_name, country_name_en | Order | Orders receivers, Orders receivers history | 2 | ⚪ 선택 | 국가명 (영문) |
| 국가별 | country_hs_code, country_hscode, country_shipping_fee_list | Product, Shipping, Supply | Bundleproducts, Products, Shipping, Shipping suppliers | 7 | ⚪ 선택 | 국가별 HS 코드 해외 배송시 관세 부과를 위해 사용하는 HS코드. 국제 배송시 통관을 위해 반드시 정확한 번호를 입력해야 함. 국가별로 HS 코드의 표준이 다르기 때문에 해당 국가에 맞는 코드 입력이 필요함. |
| 국가코드 | country_code | Collection, Order, Privacy, Shipping, Store, Supply | Customersprivacy, Manufacturers, Orders calculation, Orders receivers, Orders receivers history, Shipping additionalfees, Shipping suppliers additionalfees, Shippingorigins, Store, Suppliers users regionalsurcharges | 16 | ⚪ 선택 | 국가코드 해외몰인 경우 필수 입력 한국 : KR / 중국: CN / 일본: JP / 필리핀: PH / 미국: US / 대만: TW / 베트남 : VN |
| 기간 | period_sale | Promotion | Benefits | 2 | ⚪ 선택 | 기간 할인 설정 혜택의 상세유형이 기간 할인인 경우 그와 관련한 상세 설정 하위 요소가 입력되어야 정상적인 등록이 가능함 할인 금액(discount_value_unit)이 비율(P)인 경우 할인 반올림 단위(discount_truncation_unit), 할인 단위 처리(discount_truncation_method) 필수 입력 할인 금액(discount_value_unit)이 금액(W)인 경우 discount_purchasing_quantity 필수 입력 |
| 기존 | original_item_no | Order | Orders items | 1 | ⚪ 선택 | 기존 품주 아이디 |
| 기획전 | project_no | Product | Bundleproducts, Products | 2 | ⚪ 선택 | 기획전 번호 |
| 꾸미기 | code, decorationimages, image_list, path | Product | Bundleproducts, Products, Products decorationimages | 7 | ⚪ 선택 | 꾸미기 이미지 리스트 수평위치(image_horizontal_position) L : 왼쪽 C : 가운데 R : 오른쪽 수직위치(image_vertical_position) T : 상단 C : 중단 B : 하단 |
| 끝 | end_zipcode | Supply | Suppliers users regionalsurcharges | 2 | ⚪ 선택 | 끝 우편번호 지역 설정 방식(region_setting_type)이 'Z'로 설정 되어있는 경우 필수 입력 |
| 날짜 | date | Salesreport | Financials dailysales | 1 | ⚪ 선택 | 날짜 |
| 네이버 | authentication_key, certi_key, image_key, is_show_review, is_used_order, is_used_review, naver_button_mobile_basket, naver_button_mobile_product, naver_button_pc_basket, naver_button_pc_product, naver_search_advisor, refund_naver_cash, refund_naver_point, use_naver_search_advisor, use_naverlogin, used_naver_points | Order, Salesreport, Store | Naverpay setting, Refunds, Reports hourlysales, Seo setting, Socials naverlogin | 8 | ⚪ 선택 | 네이버 버튼 디자인 : Mobile 상품상세페이지 DEFAULT MA\|1\|2 |
| 네이버캐시 | naver_cash, used_naver_cash | Order, Salesreport | Refunds, Reports hourlysales | 2 | ⚪ 선택 | 네이버캐시 |
| 네이버페이 | is_button_show, is_order_page, naver_pay_claim_status, naver_pay_order_id, naverpay_cancel_reason_type, naverpay_payment_information, naverpay_return_reason_type, naverpay_review_id, naverpay_type, naverpay_version, use_naverpay | Community, Order, Product, Store | Boards articles, Bundleproducts, Cancellation, Naverpay setting, Orders, Orders cancellation, Orders items, Orders return, Orders shortagecancellation, Products, Return | 15 | ⚪ 선택 | 네이버페이 클레임 타입 네이버페이 주문의 클레임 타입 PAYMENT_WAITING : 입금대기 PAYED : 결제완료 DELIVERING : 배송중 DELIVERED : 배송완료 PURCHASE_DECIDED : 구매확정 EXCHANGED : 교환 CANCELED : 취소 RETURNED : 반품 CANCELED_BY_NOPAYMENT : 미입금취소 NOT_YET : 발주 미확인 OK : 발주 확인 CANCEL : 발주 확인 해제 CANCEL_REQUEST : 취소요청 CANCELING : 취소처리중 CANCEL_DONE : 취소처리완료 CANCEL_REJECT : 취소철회 RETURN_REQUEST : 반품요청 COLLECTING : 수거처리중 COLLECT_DONE : 수거완료 RETURN_DONE : 반품완료 RETURN_REJECT : 반품철회 EXCHANGE_REQUEST : 교환요청 COLLECTING : 수거처리중 COLLECT_DONE : 수거완료 EXCHANGE_RE |
| 네이버포인트 | naver_point | Order | Orders, Refunds | 2 | ⚪ 선택 | 네이버포인트 |
| 년월 | month | Community, Salesreport | Financials monthlyreviews, Financials monthlysales | 2 | ⚪ 선택 | 년월 |
| 노출시간 | display_time, display_time_end_hour, display_time_start_hour | Community | Boards articles | 2 | ⚪ 선택 | 노출시간 시작 시각 |
| 누적 | total_cancel_count, total_sale_count | Salesreport | Reports productsales | 1 | ⚪ 선택 | 누적 판매 수량 |
| 뉴스메일 | news_mail | Customer, Notification, Privacy | Customers, Customersprivacy, Recipientgroups | 5 | ⚪ 선택 | 뉴스메일 수신여부 Youtube shopping 이용 시에는 미제공 이메일을 수신할지 여부. '수신거부' 시 광고, 영리성 목적 외 서비스에 필요한 주요 메일은 정상적으로 수신함. T : 수신 F : 수신안함 |
| 다수 | issue_count_per_once | Promotion | Coupons issues | 1 | ⚪ 선택 | 다수 발행시 발행 수량 쿠폰 1회 발급시 여러장 발행하는 경우 그 수량 DEFAULT 2 |
| 다음 | next_grade, required_purchase_amount, required_purchase_count | Customer | Customers autoupdate | 1 | ⚪ 선택 | 다음 등급까지 필요 금액 |
| 단독구매 | single_purchase, single_purchase_restriction | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 단독구매 제한 Youtube shopping 이용 시에는 미제공 단독구매 설정(single_purchase)에 값을 입력했을 경우, single_purchase 값이 우선 적용됨 T : 단독구매 불가 F : 제한안함 DEFAULT F |
| 담당자 | manager_information | Supply | Suppliers | 2 | ⚪ 선택 | 담당자 공급사의 담당자 연락처 정보. 담당자는 세명까지 지정 가능하다. |
| 답변 | method, reply_article_no, reply_depth, reply_sequence, reply_status, status | Community | Boards articles, Urgentinquiry, Urgentinquiry reply | 5 | ⚪ 선택 | 답변 게시물 번호 게시물에 답변을 추가하고자 할 경우 게시물의 번호를 입력한다. |
| 답변글 | admin_reply_fixed | Community | Boards | 2 | ⚪ 선택 | 답변글 제목을 관리자가 설정한 값으로 고정할지 여부 |
| 답변기능 | reply_feature | Community | Boards | 2 | ⚪ 선택 | 답변기능 T : 사용함 F : 사용안함 |
| 답변쓰기 | reply_member_group_no, reply_permission | Community | Boards | 2 | ⚪ 선택 | 답변쓰기 권한 A : 관리자 M : 회원이상 N : 비회원이상 G : 접근회원그룹설정 |
| 당일 | issue_on_anniversary | Promotion | Coupons | 2 | ⚪ 선택 | 당일 발급 여부 S : 당일 P: 선발행 |
| 대량구매 | bulk_purchase_sale | Promotion | Benefits | 2 | ⚪ 선택 | 대량구매 수량 설정 혜택의 상세유형이 대량구매 할인인 경우 그와 관련한 상세 설정 |
| 대표 | contact | Shipping | Carriers, Shippingorigins | 4 | ⚪ 선택 | 대표 연락처 |
| 대표자명 | president_name | Collection, Store, Supply | Manufacturers, Store, Suppliers | 5 | ⚪ 선택 | 대표자명 사업자 등록시 공급사에서 등록한 대표자명 |
| 댓글 | comment_author_display, comment_author_protection, comment_no, password, rating, use_comment | Community | Boards, Boards articles comments, Boards comments | 6 | ⚪ 선택 | 댓글 작성자 표시 설정 N : 이름 U : 별명(별명기입전 이름으로 노출) I : 별명(별명기입전 아이디로 노출) |
| 댓글여부 | comment | Community | Boards articles | 1 | ⚪ 선택 | 댓글여부 T : 있음 F : 없음 |
| 데이터 | period | Category | Autodisplay | 2 | ⚪ 선택 | 데이터 집계 기간 1: 1일 3: 3일 7: 1주(7일) 30: 30일 |
| 도로명 | address_street | Order | Orders receivers, Orders receivers history | 2 | ⚪ 선택 | 도로명 |
| 도서산간 | remote_area_surcharge_amount | Shipping, Supply | Regionalsurcharges, Suppliers users regionalsurcharges setting | 4 | ⚪ 선택 | 도서산간 추가 배송비 |
| 동일인 | issue_max_count_by_user, same_user_reissue | Promotion | Coupons, Serialcoupons | 3 | ⚪ 선택 | 동일인 재발급 가능여부 issue_limit가 'T'로 입력된 경우만 필수 입력 T : 동일인 재발급 가능 F : 동일인 재발급 불가능 |
| 등급 | total_period, total_purchase_amount, total_purchase_count | Customer | Customergroups setting, Customers autoupdate | 2 | ⚪ 선택 | 등급 산정 누적 기간 now : 변경시점 직전까지 1m : 최근 1개월 3m : 최근 3개월 6m : 최근 6개월 12m : 최근 12개월 24m : 최근 24개월 36m : 최근 36개월 |
| 등급별 | use_discount_limit | Customer | Customergroups setting | 1 | ⚪ 선택 | 등급별 할인 제한 사용여부 T : 사용함 F : 사용안함 |
| 등록 | payment_methods, permission_product_delete | Store, Supply | Paymentservices, Suppliers users | 3 | ⚪ 선택 | 등록 상품 삭제 권한 공급사 운영자가 자신이 등록한 상품을 삭제할 수 있는 권한 설정 |
| 등록기준 | attach_type | Order | Orders memos | 2 | ⚪ 선택 | 등록기준 O : 주문별 P : 품목별 DEFAULT O |
| 등록일 | issue_date, register_date | Mileage, Promotion | Commonevents, Credits | 2 | ⚪ 선택 | 등록일 |
| 로그인 | use_notification_when_login | Promotion | Coupons | 2 | ⚪ 선택 | 로그인 시 쿠폰발급 알람 사용여부 회원 로그인 시 쿠폰발급 알람을 사용할지 여부 |
| 리뷰 | rating_average | Community | Financials monthlyreviews | 1 | ⚪ 선택 | 리뷰 평점 평균 |
| 리사이징할 | image_resize | Community | Boards | 1 | ⚪ 선택 | 리사이징할 이미지 폭 (px) |
| 마진률 | margin_rate | Product | Products | 2 | ⚪ 선택 | 마진률 상품의 원가에 더하여 판매가 계산을 위한 마진율. Api에서는 해당 값은 참고용으로만 사용된다. tax_calculation이 A(자동계산)일 경우 null로 반환됨. |
| 만료일 | expiration_date | Application, Promotion | Appstore payments, Coupons issuancecustomers, Coupons issues | 3 | ⚪ 선택 | 만료일 |
| 매장수령여부 | store_pickup | Order | Orders, Orders items | 2 | ⚪ 선택 | 매장수령여부 매장수령 상품 여부 T : 매장수령 F : 매장수령 아님 |
| 매체사 | sales_channel | Community | Boards articles | 2 | ⚪ 선택 | 매체사 |
| 멀티 | multi_invoice, multiple_addresses | Order | Orders, Orders items | 4 | ⚪ 선택 | 멀티 송장 Youtube shopping 이용 시에는 미제공 ※ 멀티 송장 수정시 "claim_type" "claim_status" "claim_reason_type", "claim_quantity", "claim_quantity"은 사용 불가합니다. ※ 메인송장의 송장번호와 배송업체 코드는 shipments 에서만 수정이 가능하고 배송처리 이후부터는 수정만 가능하며 추가/삭제는 안됩니다. ※ 멀티 송장에는 연동 배송업체를 입력할 수 없습니다. ※ 해당 속성에 대한 어드민 UI는 24년 7월 8일부터 확인 가능합니다. |
| 메인분류 | display_group, group_name, use_main | Category, Product, Store | Autodisplay, Categories, Mains, Mains products, Seo setting | 10 | ⚪ 선택 | 메인분류 표시상태 해당 상품분류가 쇼핑몰 메인에 표시되는지 여부. 메인분류에 표시하는 경우 중/소/상세 분류도 대분류처럼 최상위에 표시된다. T : 표시함 F : 표시안함 |
| 메인진열 | main | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 메인진열 Youtube shopping 이용 시에는 미제공 상품을 "추천상품", "신상품"과 같은 메인진열에 진열할 경우, 메인 진열 번호를 표시한다. |
| 메타태그1 | meta_author | Category, Community, Product | Boards seo, Categories seo, Products seo | 6 | ⚪ 선택 | 메타태그1 : Author [MALL_NAME] : 쇼핑몰명 [BOARD_NAME] : 게시판 제목 [BOARD_GUIDE] : 게시판 안내글 [ARTICLE_TITLE] : 게시물 제목 |
| 메타태그2 | meta_description | Category, Community, Product | Boards seo, Categories seo, Products seo | 6 | ⚪ 선택 | 메타태그2 : Description 해당 상품의 상품 상세 페이지의 태그에 표시되는 정보. description 태그에 검색 결과 페이지에서 검색 결과 아래에 표시될 간략한 정보를 입력할 수 있다. |
| 메타태그3 | meta_keywords | Category, Community, Product | Boards seo, Categories seo, Products seo | 6 | ⚪ 선택 | 메타태그3 : Keywords [MALL_NAME] : 쇼핑몰명 [BOARD_NAME] : 게시판 제목 [BOARD_GUIDE] : 게시판 안내글 [ARTICLE_TITLE] : 게시물 제목 |
| 면세 | tax_free_amount | Order | Orders calculation | 1 | ⚪ 선택 | 면세 + 영세 |
| 모델명 | model_name | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 모델명 검색어를 모델명에 포함하고 있는 상품 검색(대소문자 구분 없음) ,(콤마)로 여러 건을 검색할 수 있다. |
| 모듈 | module_code | Category | Mains | 1 | ⚪ 선택 | 모듈 코드 각 메인분류에 지정된 모듈 코드 |
| 모바일 | display_mobile, mobile, mobile_description, mobile_discount_information, mobile_discount_price, mobile_points_information, mobile_skin_no, order_from_mobile, separated_mobile_description, sms, use_mobile_domain_redirection, use_mobile_page, use_sms_agree_point | Customer, Notification, Order, Privacy, Product, Salesreport, Store | Bundleproducts, Customergroups, Customers, Customersprivacy, Information, Mobile setting, Orders, Orders calculation, Points setting, Products, Products discountprice, Recipientgroups | 22 | ⚪ 선택 | 모바일 메시지 수신여부 SMS를 수신할지 여부. '수신거부' 시 광고, 영리성 목적 외 서비스에 필요한 주요 메일은 정상적으로 수신함. T : 수신 F : 수신안함 |
| 모바일앱 | use_mobile_app | Customer, Notification, Privacy | Customers, Customersprivacy, Recipientgroups | 5 | ⚪ 선택 | 모바일앱 사용여부 Youtube shopping 이용 시에는 미제공 T : 사용 F : 사용안함 |
| 목록이미지 | list_image | Product | Bundleproducts, Products, Products images | 6 | ⚪ 선택 | 목록이미지 Youtube shopping 이용 시에는 미제공 상품 분류 화면, 메인 화면, 상품 검색 화면에 표시되는 상품의 목록 이미지. |
| 무통장 | bank_account_id | Order, Store | Orders payments, Store accounts | 2 | ⚪ 선택 | 무통장 입금 은행 ID 결제수단을 무통장입금으로 변경할 경우("change_payment_method:"T"이고 "payment_method":"cash"일 경우) 사용 가능 |
| 문화비 | cultural_tax_deduction | Product | Bundleproducts, Products | 3 | ⚪ 선택 | 문화비 소득공제 Youtube shopping 이용 시에는 미제공 T : 사용함 F : 사용안함 |
| 미가용 | available_date, unavailable_coupon_points, unavailable_points, unusable_points_change_type | Mileage, Store | Points, Points report, Points setting | 4 | ⚪ 선택 | 미가용 적립금 변환 기준 설정 M: 최초 상품 배송완료일/구매확정일 기준으로 적립 T: 마지막 상품 배송완료일/구매확정일 기준으로 적립 |
| 미입금 | auto_cancel, unpaid_amount | Order, Store | Orders setting, Unpaidorders | 3 | ⚪ 선택 | 미입금 주문 자동취소 사용설정 Youtube shopping 이용 시에는 미제공 T : 사용함 F : 사용안함 |
| 미적용 | category_unapplied | Product | Bundleproducts, Products | 2 | ⚪ 선택 | 미적용 분류 검색 분류가 등록되지 않은 상품에 대하여 검색함. T: 미적용 분류 검색 |
| 반송장 | return_invoice_fail_reason, return_invoice_success | Order | Exchange, Orders exchange, Orders return, Return | 8 | ⚪ 선택 | 반송장 처리 성공 여부 T : 성공 F : 실패 N : 미집하 |
| 발급 | issue_anniversary_pre_issue_day, issue_anniversary_type, issue_module_type, issue_order_amount_limit, issue_order_amount_max, issue_order_amount_min, issue_order_available_category, issue_order_available_category_list, issue_order_available_product, issue_order_available_product_list, issue_review_count, issue_review_has_image, issue_sub_type, issue_type, issued_by_event_type | Promotion | Coupons, Coupons issues, Serialcoupons | 5 | ⚪ 선택 | 발급 사유 구분 혜택으로 인한 쿠폰발급 시 해당되는 혜택 C : 출석체크 이벤트 U : 회원정보 수정 이벤트 B : 배너수익쉐어프로그램 R : 룰렛게임(CMC)팀 Z : 브랜드앱 설치(브랜드앱) Y : 푸시알림 ON(브랜드앱) X : 브랜드앱 주문(브랜드앱) M : 리마인드 Me 주문 W : 리마인드 Me 리워드 V : 통합멤버십 L : 평생회원 전환 이벤트 |
| 발급가능 | issue_order_amount_type | Promotion | Coupons, Serialcoupons | 3 | ⚪ 선택 | 발급가능 구매금액 유형 쿠폰으로 할인 시 할인 대상이 되는 금액의 기준 |
| 발급단위 | issue_order_type | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 발급단위 쿠폰의 발급 단위가 상품인지 주문서단위 쿠폰인지 여부 P : 상품 쿠폰 O : 주문서 쿠폰 |
| 발급대상 | group_no, issue_member_group_name, issue_member_group_no, issue_order_date | Promotion | Coupons, Coupons issuancecustomers, Coupons issues | 4 | ⚪ 선택 | 발급대상 주문기간 설정 T : 주문기간 설정 F : 주문기간 설정 불가 |
| 발급된 | issued_count, issued_flag, show_issued_coupon | Promotion, Store | Coupons, Coupons setting, Discountcodes, Serialcoupons | 7 | ⚪ 선택 | 발급된 쿠폰 여부 쿠폰이 기존에 발급된 이력이 있는지 여부 T : 발급이력이 있는 쿠폰 F : 발급이력이 없는 쿠폰 |
| 발급수 | issue_limit | Promotion | Coupons | 2 | ⚪ 선택 | 발급수 제한여부 T : 발급 제한 F : 발급 제한 아님 |
| 발급자 | request_admin_id | Promotion | Coupons issues | 1 | ⚪ 선택 | 발급자 ID |
| 발급처 | issued_place_type | Promotion | Coupons issues | 1 | ⚪ 선택 | 발급처 구분 쿠폰이 발행된 출처 구분 W : 웹 M : 모바일 P : 브랜드앱 |
| 발송 | requested_end_date, requested_start_date, send_method, send_sms, type | Application, Mileage, Notification, Store | Databridge logs, Points autoexpiration, Restocknotification setting, Sms, Webhooks logs | 7 | ⚪ 선택 | 발송 타입 SMS 의 발송 타입. SMS 는 1건당 최대 90byte 까지 입력 가능하고 90byte 초과 시 여러 개로 나눠서 발송한다. LMS 는 1건당 최대 2000byte 까지 입력 가능하다. SMS : 단문 LMS : 장문 DEFAULT SMS |
| 발송예정일 | shipping_expected_date | Order | Orders items | 2 | ⚪ 선택 | 발송예정일 |
| 발행 | type | Order | Cashreceipt | 2 | ⚪ 선택 | 발행 타입 개인: personal 사업자: business |
| 발행일 | issued_date | Promotion | Customers coupons | 1 | ⚪ 선택 | 발행일 |
| 변경 | current_order_status, previous_order_status | Order | Orders items history | 1 | ⚪ 선택 | 변경 전 주문상태 |
| 변경된 | changed_refund_amount, changed_variant_code | Order | Refunds, Subscription shipments items | 3 | ⚪ 선택 | 변경된 옵션 품목코드 |
| 별명 | nick_name, nick_name_icon_type, nick_name_icon_url | Community, Store, Supply | Boards articles, Suppliers users, Users | 5 | ⚪ 선택 | 별명 아이콘 타입 공급사 운영자의 별명 옆에 표시되는 아이콘을 설정할 수 있다. 직접 아이콘 등록 : 별명 아이콘을 직접 업로드하여 설정할 수 있다. 샘플 아이콘 등록 : 미리 제공되는 아이콘을 선택하여 설정할 수 있다. 공급사 운영자 상세 조회 API에서만 확인 가능하다. D : 직접 S : 샘플 |
| 보조 | additional_payment_amount, secondary_contact | Order, Shipping | Carriers, Orders paymentamount, Orders paymenttimeline, Shippingorigins | 6 | ⚪ 선택 | 보조 연락처 Youtube shopping 이용 시에는 미제공 |
| 복원할 | recover_coupon_no | Order | Cancellation, Orders cancellation, Orders return, Orders shortagecancellation, Return | 5 | ⚪ 선택 | 복원할 쿠폰 번호 Youtube shopping 이용 시에는 미제공 |
| 복합 | mixed_refund_amount, mixed_refund_methods | Order | Orders shippingfeecancellation | 1 | ⚪ 선택 | 복합 환불 금액 |
| 부가세 | product_tax_type_text, vat, vat_amount | Order, Product | Cashreceipt, Orders calculation, Products | 3 | ⚪ 선택 | 부가세 표시 문구 [쇼핑몰 설정 > 상품 설정 > '상품 보기 설정 > 상품 정보 표시 설정 > 추가설정 > 판매가 부가세 표시문구']에서 설정한 문구 표시 tax_calculation이 A(자동계산)일 경우 null로 반환됨. |
| 부모 | parent_article_no, parent_category_no, parent_comment_no, parent_skin_no | Category, Community, Design | Boards articles, Boards articles comments, Boards comments, Categories, Themes | 7 | ⚪ 선택 | 부모 분류 번호 해당 상품분류가 2차(중분류), 3차(소분류), 4차(세분류)일 경우 상위에 있는 상품분류의 번호를 표시함. parent_category_no = 1일 경우 해당 분류는 대분류를 의미한다. |
| 분류 | category, category_depth, category_no, display_sub_category, full_category_name, full_category_no, menu_image_mobile, menu_image_pc, menu_over_image_pc, title_image_mobile, title_image_pc, top_images_mobile, top_images_pc, use_menu_image_mobile, use_menu_image_pc, use_title_image_mobile, use_title_image_pc, use_top_image_mobile, use_top_image_pc | Category, Community, Personal, Product, Salesreport, Store, Translation | Autodisplay, Boards articles, Bundleproducts, Carts, Categories, Categories decorationimages, Categories products, Categories seo, Products, Products setting, Reports salesvolume, Translations categories | 21 | ⚪ 선택 | 분류 Depth 해당 상품분류가 하위 몇 차 상품분류에 있는 카테고리인지 표시함. 1~4차까지 상품분류가 존재한다. |
| 분류명 | category_name | Category | Categories | 2 | ⚪ 선택 | 분류명 검색어를 분류명에 포함하고 있는 상품분류 검색 |
| 분류별 | separated_category | Product | Categories properties | 2 | ⚪ 선택 | 분류별 별도등록 T : 사용함 F : 사용안함 DEFAULT F |
| 분리된 | original_bundle_item_no | Order | Orders items | 2 | ⚪ 선택 | 분리된 세트상품의 기존 품주번호 분리형 세트 상품의 기존 품목 번호 |
| 브라우저 | meta_title | Category, Community, Product | Boards seo, Categories seo, Products seo | 6 | ⚪ 선택 | 브라우저 타이틀 [MALL_NAME] : 쇼핑몰명 [BOARD_NAME] : 게시판 제목 [BOARD_GUIDE] : 게시판 안내글 [ARTICLE_TITLE] : 게시물 제목 |
| 비고 | refund_reason | Order | Cancellation, Exchange, Return | 3 | ⚪ 선택 | 비고 |
| 비밀글 | secret | Community | Boards articles, Boards articles comments, Boards comments | 5 | ⚪ 선택 | 비밀글 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 비밀글만 | secret_only | Community | Boards | 2 | ⚪ 선택 | 비밀글만 등록 가능여부 T: 비밀글만 등록 F: 공개글과 비밀글을 선택하여 등록 |
| 사업자등록번호 | company_registration_no | Order, Store, Supply | Cashreceipt, Orders buyer, Store, Suppliers | 6 | ⚪ 선택 | 사업자등록번호 해당 공급사의 사업자 등록 번호. 국가에 따라 해당 사업자의 등록 고유 번호가 발급되는 경우 표시한다. |
| 사업장 | country, country_code | Store, Supply | Store, Suppliers | 3 | ⚪ 선택 | 사업장 국가 사업장이 있는 국가명. |
| 사유 | reason, reason_type | Order | Cancellationrequests, Exchangerequests, Orders exchangerequests, Returnrequests | 5 | ⚪ 선택 | 사유 구분 A:고객변심 B:배송지연 J:배송오류 C:배송불가지역 L:수출/통관 불가 D:포장불량 E:상품 불만족 F:상품정보상이 K:상품불량 G:서비스불만족 H:품절 I:기타 |
| 사은품 | allow_gift_review, available_payment_methods, collect_gift, gift, gift_available_condition, gift_grant_mode, gift_grant_type, gift_selection_mode, gift_selection_step | Order, Promotion, Store | Benefits, Benefits setting, Orders items, Orders shortagecancellation | 6 | ⚪ 선택 | 사은품 신청 가능 조건 사은품선택단계(gift_selection_step)에서 주문상세조회(order_detail)항목이 선택된 경우만 입력 가능 during_period : 설정 기간 동안만 신청 가능 after_period : 설정 기간 이후에도 신청 가능 |
| 사은품증정 | item_granting_gift | Order | Orders items | 1 | ⚪ 선택 | 사은품증정 조건품주목록 |
| 사이즈 | size_guide | Product | Products | 2 | ⚪ 선택 | 사이즈 가이드 Youtube shopping 이용 시에는 미제공 |
| 삭제 | delete_category_no, deleted | Community, Product | Boards articles, Bundleproducts, Products | 4 | ⚪ 선택 | 삭제 분류 번호 Youtube shopping 이용 시에는 미제공 상품분류 번호를 입력하여 해당 상품에 특정 상품분류 삭제 |
| 상단고정 | fixed | Order | Orders memos | 2 | ⚪ 선택 | 상단고정 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 상담결과 | status | Order | Orders memos | 2 | ⚪ 선택 | 상담결과 F : 처리중 T : 처리완료 |
| 상담분류 | topic_type | Order | Orders memos | 2 | ⚪ 선택 | 상담분류 cs_01 : 배송문의 cs_02 : 상품문의 cs_03 : 결제문의 cs_04 : 주문취소 cs_05 : 상품변경 |
| 상세 | address2, detail_authority_setting, display_group | Category, Collection, Order, Privacy, Product, Shipping, Store, Supply | Autodisplay, Categories products, Categories properties, Customersprivacy, Mains properties, Manufacturers, Orders receivers, Orders receivers history, Shippingorigins, Store, Suppliers, Users | 21 | ⚪ 선택 | 상세 상품분류 1 : 일반상품 2 : 추천상품 3 : 신상품 DEFAULT 1 |
| 상세이미지 | detail_image, image, path | Product | Bundleproducts, Products, Products images | 7 | ⚪ 선택 | 상세이미지 ● 이미지 파일 용량 제한 : 10MB ● 한 호출당 이미지 전체 용량 제한 : 30MB |
| 상품 | additional_product_amount, channeldiscountprices, code, created_end_date, created_start_date, custom_properties, discountprice, display_product_count, hits, image_list, item_discount_amount, meta_alt, og_category, og_product, options, order_price_amount, permission_category_select, permission_product_display, permission_product_modify, permission_product_selling, permitted_category_list, price_max, price_min, product_binding_type, product_condition, product_image_size, product_list, product_option_price, product_page_size, product_shipping_type, product_tag, product_tax_type, product_volume, product_weight, retail_price, retail_price_max, retail_price_min, seo, shipping_fee_by_quantity, simple_description, supply_price, supply_price_max, supply_price_min, tag, tags, translate_product_material, translated_additional_description, updated_end_date, updated_start_date, volume_size, volume_size_weight | Community, Order, Product, Promotion, Salesreport, Shipping, Store, Supply | Benefits, Boards, Bundleproducts, Images setting, Orders calculation, Orders items, Orders memos, Orders paymentamount, Products, Products icons, Products seo, Products setting | 41 | ⚪ 선택 | 상품 범위 해당 혜택이 적용되는 상품의 범위 전체상품 : 전체 상품에 혜택 적용 특정상품 : 선택한 특정 상품에 대해서만 혜택 적용 제외상품 : 선택한 특정 상품에 대해서만 혜택 적용 제외 상품분류 : 선택한 상품 분류에 속한 상품에 대해서만 혜택 적용 |
| 상품가(세금 | price_excluding_tax | Product | Products | 2 | ⚪ 선택 | 상품가(세금 제외) 상품설정조회 상품설정조회 Docs 바로가기 에서 "판매가 계산 기준(calculate_price_based_on)"이 "B(상품가)"일 경우 "price" 대신 필수 입력 필요. |
| 상품별 | coupon_discount_price, individual_shipping_fee, market_discount_amount, product_availability, product_discount_amount, shipping_fee_by_product | Customer, Order, Shipping, Supply | Customergroups, Orders calculation, Orders items, Refunds, Shipping, Shipping suppliers | 8 | ⚪ 선택 | 상품별 할인 중복설정 P : 상품별 가격할인만 적용 M : 회원등급별 가격할인만 적용 A : 둘다적용 |
| 상품별추가할인 | add_discount_amount | Order | Cancellation, Exchange, Return | 3 | ⚪ 선택 | 상품별추가할인 취소액 |
| 상품분류 | new_product_display_key, new_product_display_sort, new_product_display_type, normal_product_display_key, normal_product_display_sort, normal_product_display_type, product_display_key, product_display_scope, product_display_sort, product_display_type, recommend_product_display_key, recommend_product_display_sort, recommend_product_display_type, use_except_category | Category, Promotion | Benefits, Categories | 4 | ⚪ 선택 | 상품분류 진열영역 구분 상품 분류에 상품을 동일하게 정렬할 것인지, 영역별로 정렬할 것인지 설정 "전체"로 설정할 경우 다음 필드는 반드시 입력되어야 한다. product_display_type product_display_key product_display_sort product_display_period (key가 S, C일 때만 필수) "영역별"로 설정할 경우 다음 필드는 반드시 입력되어야 한다. normal_product_display_type normal_product_display_key normal_product_display_sort normal_product_display_period (key가 S, C일 때만 필수) recommend_product_display_type recommend_product_display_key recommend_product_display_sort recommend_product_display_period (key가 S, C일 때만 필 |
| 상품상세설명 | description, translated_description | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 상품상세설명 상품에 보다 상세한 정보가 포함되어있는 설명. HTML을 사용하여 입력이 가능하다. |
| 상품소재 | product_material | Order, Product | Bundleproducts, Orders items, Products | 5 | ⚪ 선택 | 상품소재 Youtube shopping 이용 시에는 미제공 상품의 소재. 복합 소재일 경우 상품의 소재와 함유랑을 함께 입력해야함. (예 : 면 80%, 레이온 20%) |
| 상품수 | product_count | Collection | Brands, Classifications, Trends | 3 | ⚪ 선택 | 상품수 |
| 상품요약설명 | summary_description | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 상품요약설명 상품에 대한 요약 정보. 상품 진열 화면에서 노출 가능한 설명. HTML을 사용하여 입력이 가능하다. [쇼핑몰 설정 > 상품 설정 > '상품 보기 설정 > 상품 정보 표시 설정']에서 노출되도록 설정 가능하다. |
| 상품정보 | has_product | Community | Boards articles | 1 | ⚪ 선택 | 상품정보 포함 여부 T : 있음 F : 없음 |
| 상품중량 | product_weight | Shipping, Supply | Shipping, Shipping suppliers | 4 | ⚪ 선택 | 상품중량 |
| 상품추가할인액 | additional_discount_price | Order | Orders items | 1 | ⚪ 선택 | 상품추가할인액 상품에 대한 추가 할인금액 |
| 상호명 | company_name | Order, Store, Supply | Orders buyer, Store, Suppliers | 4 | ⚪ 선택 | 상호명 사업자 등록시 등록한 상호명 또는 법인명. |
| 서비스 | contact_us_contents, contact_us_mobile, service_available_end_date, service_available_start_date, service_completion_date, service_limit_type, service_status, service_use_date | Order, Store | Paymentgateway, Reservations, Socials navershopping, Store | 5 | ⚪ 선택 | 서비스 문의안내 모바일 표시여부 서비스 문의 안내를 모바일에 노출시킬 것인지 여부. T : 표시함 F : 표시안함 |
| 선/착불 | shipping_payment_option | Order | Orders items | 1 | ⚪ 선택 | 선/착불 구분 C : 착불 P : 선결제 F : 무료 |
| 설치일 | install_date | Customer | Customers plusapp | 1 | ⚪ 선택 | 설치일 |
| 성별 | gender, gender_restriction | Customer, Notification, Privacy, Store | Customers, Customers setting, Customersprivacy, Recipientgroups | 5 | ⚪ 선택 | 성별 Youtube shopping 이용 시에는 미제공 해당 회원의 성별 M : 남자 F : 여자 |
| 성인인증 | adult_certification, adult_image_restriction, adult_purchase_restriction | Product, Store | Bundleproducts, Customers setting, Products | 5 | ⚪ 선택 | 성인인증 성인인증이 필요한 상품인지 여부. 성인인증이 필요한 상품인 구매를 위해서는 본인인증을 거쳐야함. [쇼핑몰 설정 > 고객 설정 > '회원 정책 설정 > 회원 관련 설정 > 회원가입 및 본인인증 설정'] 에서 성인인증 사용 시 구매차단 설정이 사용함이어야 성인인증이 적용된다. EC 베트남, 필리핀 버전에서는 사용할 수 없음. T : 사용함 F : 사용안함 DEFAULT F |
| 세금 | tax, tax_calculation, tax_detail, use | Order, Product, Store | Cancellation, Exchange, Orders, Orders shippingfeecancellation, Products, Refunds, Return, Taxmanager | 8 | ⚪ 선택 | 세금 정보 세금 관리자 앱을 사용 안 할 경우 null로 반환 |
| 세트 | bundle_product_components | Product | Bundleproducts | 2 | ⚪ 선택 | 세트상품의 구성상품 정보 |
| 세트상품 | bundle_additional_options, product_bundle, product_bundle_discount_amount, product_bundle_list, product_bundle_type, set_product_type | Order, Personal, Product | Carts, Customers wishlist, Orders items, Orders items options, Products, Products carts, Refunds | 9 | ⚪ 선택 | 세트상품 타입 세트상품의 타입 C : 일체형 S : 분리형 |
| 세트품주 | was_product_bundle | Order | Orders items | 2 | ⚪ 선택 | 세트품주 분리여부 T : 세트상품 나눔 F : 세트상품 나눔 안함 DEFAULT F |
| 세트할인 | bundle_product_sales | Product | Bundleproducts | 2 | ⚪ 선택 | 세트할인 정보 |
| 소멸 | group_no, interval_month, standard_point, target_period_month | Mileage | Points autoexpiration | 2 | ⚪ 선택 | 소멸 대상 적립금 6: 소멸일 기준 6개월 이전 적립금 12: 소멸일 기준 1년 이전 적립금 18: 소멸일 기준 1년 6개월 이전 적립금 24: 소멸일 기준 2년 이전 적립금 30: 소멸일 기준 2년 6개월 이전 적립금 36: 소멸일 기준 3년 이전 적립금 |
| 송장번호입력일 | tracking_no_updated_date | Order | Orders shipments | 1 | ⚪ 선택 | 송장번호입력일 |
| 쇼핑 | hash_tags, hashtag_product_display | Category | Categories | 2 | ⚪ 선택 | 쇼핑 큐레이션 해시태그 상품진열 해시태그 상품 진열 기능을 사용할 것인지 여부 ※ 해당 기능은 쇼핑 큐레이션 서비스를 사용하는 경우에만 사용 가능하다. T : 진열함 F : 진열안함 |
| 수거 | collect_tracking_no, pickup_request_state | Order | Collectrequests, Return | 3 | ⚪ 선택 | 수거 신청 상태 E : 수거 미신청 W : 수거 미접수 S : 수거접수대기(송장발급전) F : 수거접수실패 T : 수거접수완료(송장발급완료) N : 미집하 |
| 수거신청 | request_pickup | Order | Exchangerequests, Orders exchange, Orders return, Return, Returnrequests | 8 | ⚪ 선택 | 수거신청 여부 T : 수거신청 F : 직접발송 |
| 수거완료 | pickup_completed | Order | Exchange, Orders exchange, Orders return, Return | 8 | ⚪ 선택 | 수거완료 여부 T : 수거완료 F : 수거전 DEFAULT F |
| 수거완료시 | exchanged_after_collected | Order | Exchange, Orders exchange | 4 | ⚪ 선택 | 수거완료시 교환완료 여부 T : 사용함 F : 사용안함 |
| 수거지 | pickup | Order | Exchange | 1 | ⚪ 선택 | 수거지 - 주소 |
| 수거지역 | pickup | Order | Exchangerequests, Orders exchange, Orders return, Return, Returnrequests | 8 | ⚪ 선택 | 수거지역 상세 |
| 수수료 | commission | Supply | Suppliers | 1 | ⚪ 선택 | 수수료 정산유형이 수수료형(P)일 경우 사용하는 수수료 정보 |
| 수수료율 | commission | Supply | Suppliers | 1 | ⚪ 선택 | 수수료율 정산유형이 수수료형(P)일 경우 사용하는 수수료 정보 DEFAULT 10 |
| 수정되기전 | original_options | Product | Products options | 1 | ⚪ 선택 | 수정되기전 옵션값 |
| 순매출 | sales | Salesreport | Reports hourlysales | 1 | ⚪ 선택 | 순매출 |
| 스토어픽업 | store_pickup | Order | Subscription shipments | 2 | ⚪ 선택 | 스토어픽업 T : 사용함 F : 사용안함 DEFAULT F |
| 스팸 | spam_auto_prevention | Community, Store | Boards, Boards setting | 4 | ⚪ 선택 | 스팸 자동 생성 방지 설정 |
| 승인번호 | approval_no | Application, Order | Appstore payments, Cashreceipt | 3 | ⚪ 선택 | 승인번호 결제 승인 번호 |
| 승인요청 | approve_status | Product | Products | 1 | ⚪ 선택 | 승인요청 결과 N : 승인요청 (신규상품) E : 승인요청 (상품수정) C : 승인완료 R : 승인거절 I : 검수진행중 Empty Value : 요청된적 없음 |
| 시/군/도시 | address_city, city | Order, Privacy | Customersprivacy, Orders receivers, Orders receivers history | 5 | ⚪ 선택 | 시/군/도시 Youtube shopping 이용 시에는 미제공 |
| 시리얼 | serial_generate_auto, serial_generate_method | Promotion | Coupons, Serialcoupons | 3 | ⚪ 선택 | 시리얼 쿠폰 생성방법 시리얼 쿠폰을 생성하는 방법 A : 자동 생성 M : 직접 등록 E : 엑셀 업로드 |
| 시리얼넘버 | serial_code_list | Promotion | Serialcoupons issues | 1 | ⚪ 선택 | 시리얼넘버 목록 |
| 시리얼코드 | serial_code, serial_code_type | Promotion | Serialcoupons, Serialcoupons issues | 3 | ⚪ 선택 | 시리얼코드 생성 방식 R: 다른 시리얼 코드로 생성 S: 동일 시리얼 코드로 생성 |
| 시작 | start_zipcode | Supply | Suppliers users regionalsurcharges | 2 | ⚪ 선택 | 시작 우편번호 지역 설정 방식(region_setting_type)이 'Z'로 설정 되어있는 경우 필수 입력 |
| 시작일 | available_start_date | Promotion | Discountcodes | 2 | ⚪ 선택 | 시작일 |
| 시작일 available | search_date_type | Promotion | Discountcodes | 1 | ⚪ 선택 | available_start_date : 시작일 available_end_date : 종료일 created_date : 등록일 available_start_date : 시작일 available_end_date : 종료일 created_date : 등록일 |
| 시장 | market_address1, market_address2, market_country_code | Supply | Suppliers | 2 | ⚪ 선택 | 시장 주소 국가 코드 |
| 신규상품할인 | new_product_sale | Promotion | Benefits | 2 | ⚪ 선택 | 신규상품할인 설정 혜택의 상세유형이 신규상품 할인인 경우 그와 관련한 상세 설정 하위 요소가 입력되어야 정상적인 등록이 가능함 할인 금액(discount_value_unit)이 비율(P)인 경우 할인 반올림 단위(discount_truncation_unit), 할인 단위 처리(discount_truncation_method) 필수 입력 할인 금액(discount_value_unit)이 금액(W)인 경우 discount_purchasing_quantity 필수 입력 |
| 신청일자 | request_date | Order | Cashreceipt | 1 | ⚪ 선택 | 신청일자 |
| 쓰기 | write_member_group_no, write_permission | Community | Boards | 2 | ⚪ 선택 | 쓰기 권한 A : 관리자 V : 회원이상노출 I : 회원이상 비노출 N : 비회원이상 G : 접근회원그룹설정 |
| 쓰기권한 | write_permission_extra | Community | Boards | 2 | ⚪ 선택 | 쓰기권한 부가설정 |
| 아이콘 | code, description, display, icon, icon_show_period, icon_url, id, path | Design, Product, Promotion | Benefits, Bundleproducts, Icons, Products, Products icons | 9 | ⚪ 선택 | 아이콘 상품에 표시되는 아이콘. 상품 판매를 강조하기 위한 목적으로 사용이 가능함. |
| 안심번호 | use_virtual_phone_no | Order | Subscription shipments | 2 | ⚪ 선택 | 안심번호 T : 사용함 F : 사용안함 DEFAULT F |
| 알람시기 | notification_time_day | Mileage | Points autoexpiration | 2 | ⚪ 선택 | 알람시기 선택 3: 3일 전 발송 7: 7일 전 발송 15: 15일 전 발송 30: 1개월 전 발송 |
| 알림 | expiration_period, use_push_flag | Customer, Store | Customers plusapp, Restocknotification setting | 3 | ⚪ 선택 | 알림 유효기간 설정 1:1개월 3:3개월 6:6개월 12:1년 |
| 암호화된 | data | Order | Orders completions | 1 | ⚪ 선택 | 암호화된 PG 결제 데이터 |
| 앱 | app_discount_amount, app_discount_price, app_item_discount_amount, benefit_app_key, client_id, contains_app_url, issued_by_action_type | Order, Product, Promotion, Store | Coupons issues, Menus, Orders benefits, Orders items, Paymentgateway, Paymentgateway paymentmethods, Products discountprice, Refunds | 11 | ⚪ 선택 | 앱 설치시 쿠폰 발급 앱 설치시 쿠폰이 발급되는 시점 INSTALLATION : 앱 설치시 쿠폰 발급 ACCEPTING_PUSH : 앱 푸시 수신 On시 쿠폰 발급 |
| 양력여부 | solar_calendar | Customer, Notification, Privacy | Customers, Customersprivacy, Recipientgroups | 5 | ⚪ 선택 | 양력여부 Youtube shopping 이용 시에는 미제공 T : 양력 F : 음력 |
| 업데이트 | timetable | Category | Autodisplay | 2 | ⚪ 선택 | 업데이트 시간 |
| 업태 | company_condition | Privacy, Store, Supply | Customersprivacy, Store, Suppliers | 4 | ⚪ 선택 | 업태 사업자 등록시 공급사에서 등록한 업태 |
| 에스크로 | use_escrow | Order, Store | Orders, Payment setting | 3 | ⚪ 선택 | 에스크로 사용여부 에스크로를 사용했는지 여부 T : 에스크로 사용 F : 에스크로 미사용 |
| 연결 | direct_url, slave_domain | Order, Store | Control, Shops | 3 | ⚪ 선택 | 연결 도메인 쇼핑몰에 연결된 도메인 |
| 연동 | linked_date, linked_end_date, linked_start_date, social_member_code, social_name | Customer, Order | Customers social, Orders, Social | 4 | ⚪ 선택 | 연동 된 SNS 제공코드 |
| 연동택배 | express_exception_setting | Shipping | Carriers | 1 | ⚪ 선택 | 연동택배 예외정보 설정 |
| 연동형 | option_preset_name | Product | Products options | 2 | ⚪ 선택 | 연동형 옵션 세트명 상품연동형 옵션을 사용할 경우, 옵션 세트의 이름 표시 |
| 영문 | english_product_material, product_material_eng | Order, Product | Bundleproducts, Orders items, Products | 5 | ⚪ 선택 | 영문 상품 소재 Youtube shopping 이용 시에는 미제공 상품의 소재의 영어 표기. 해외 배송사를 이용할 경우 의류의 소재를 통관시 요구하는 경우가 있음. |
| 예금주 | bank_account_holder, bank_account_name, bank_account_owner_name | Order, Store, Supply | Orders, Orders migrations, Store accounts, Suppliers | 5 | ⚪ 선택 | 예금주 공급사 정산시 사용하는 계좌의 예금주 명 |
| 예약진열 | use_reservation | Category | Autodisplay | 2 | ⚪ 선택 | 예약진열 사용여부 T: 사용함 F: 사용안함 |
| 예치금 | case, credit_amount, credits_spent_amount, credits_total, deposit_used, refund_credit, type, used_credits | Mileage, Order, Promotion, Salesreport | Credits, Credits report, Customers coupons, Orders migrations, Refunds, Reports hourlysales | 9 | ⚪ 선택 | 예치금 유형 A : 주문취소 B : 예치금환불 C : 상품구매 D : 임의조정 E : 현금환불 G : 충전 |
| 오프라인 | offline_purchase_amount, offline_purchase_count | Customer | Customergroups setting | 1 | ⚪ 선택 | 오프라인 구매금액 포함여부 T : 포함 F : 미포함 |
| 옷감 | cloth_fabric | Order, Product | Bundleproducts, Orders items, Products | 5 | ⚪ 선택 | 옷감 Youtube shopping 이용 시에는 미제공 상품이 의류인 경우, 옷감. 일본 택배사를 이용할 경우, 택배사에 따라 의류 통관시 옷감 정보를 입력 받는 경우가 있음. woven : 직물(woven) knit : 편물(knit) |
| 외부 | market_item_no | Order | Orders items | 1 | ⚪ 선택 | 외부 품목별 번호 |
| 요청 | request_body, request_endpoint, request_no | Application, Order | Collectrequests, Databridge logs, Webhooks logs | 4 | ⚪ 선택 | 요청 URL |
| 요청자 | name | Order | Cashreceipt | 2 | ⚪ 선택 | 요청자 이름 |
| 우체국 | post_express_flag | Order | Fulfillments, Orders items | 3 | ⚪ 선택 | 우체국 택배연동 S : 송장 전송 완료 |
| 원산지 | made_in_code, origin_classification, origin_place_code, origin_place_name, origin_place_no | Collection, Order, Product | Orders items, Origin, Products | 5 | ⚪ 선택 | 원산지 번호 원산지 번호를 Retrieve a list of origins API를 통해 원산지를 조회하여 입력 origin_classification이 F(국내)인 경우, 해외 여부(foreign)가 "F"인 원산지만 입력 가능함. origin_classification이 T(해외)인 경우, 해외 여부(foreign)가 "T"인 원산지만 입력 가능함. |
| 원산지기타정보 | origin_place_value | Order, Product | Orders items, Products | 3 | ⚪ 선택 | 원산지기타정보 원산지가 "기타(1800)"일 경우 원산지로 입력 가능한 정보. |
| 원산지정보 | origin_place, origin_place_value | Order, Product | Orders items, Products | 2 | ⚪ 선택 | 원산지정보 원산지가 "기타(1800)"일 경우 원산지로 입력 가능한 정보. ,(콤마)로 여러 건을 검색할 수 있다. |
| 유입경로 | group_id, inflow_group_id, inflow_group_name, inflow_icon, inflow_id, inflow_name, inflow_path, inflow_path_detail | Notification, Order | Orders, Orders inflowgroups, Orders inflowgroups inflows, Recipientgroups | 8 | ⚪ 선택 | 유입경로 그룹 멤버 아이디 |
| 유효기간 | expiration_date | Product | Products | 2 | ⚪ 선택 | 유효기간 상품을 정상적으로 사용할 수 있는 기간. 상품권이나 티켓 같은 무형 상품, 식품이나 화장품 같은 유형 상품의 유효기간을 표시. 주로 상품권이나 티켓 같은 무형 상품에 사용되며, 해당 무형 상품의 유효기간을 표시. |
| 은행명 | bank_name | Order, Store | Store accounts, Unpaidorders | 2 | ⚪ 선택 | 은행명 |
| 은행코드 | bank_code | Order, Store, Supply | Orders, Store accounts, Suppliers, Unpaidorders | 4 | ⚪ 선택 | 은행코드 공급사 정산시 사용하는 계좌의 입금은행 코드 bank_code |
| 이름 | name, name_input_style, payment_gateway, payment_gateway_name, payment_gateway_names | Customer, Order, Privacy, Salesreport, Store | Customers paymentinformation, Customersprivacy, Financials dailysales, Financials monthlysales, Financials paymentgateway, Financials store, Orders, Payment freeinstallments, Paymentmethods paymentproviders, Store setting | 13 | ⚪ 선택 | 이름 입력 방식 SEPARATE: 성/이름 각각 입력 COMBINED: 성/이름 한번에 입력 |
| 이미지 | image_display, image_upload_type | Community, Product | Boards, Bundleproducts, Products, Products images | 6 | ⚪ 선택 | 이미지 업로드 타입 Youtube shopping 이용 시에는 미제공 이미지 업로드시 이미지 업로드 타입. "대표이미지 등록"시 상세이미지를 리사이징하여 목록이미지, 작은목록이미지, 축소이미지에 업로드 "개별이미지 등록"시 상세이미지, 목록이미지, 작은목록이미지, 축소이미지를 각각 따로 업로드 ※ EC Global은 FTP를 지원하지 않으므로 C는 사용할 수 없음 A : 대표이미지등록 B : 개별이미지등록 C : 웹FTP 등록 DEFAULT A |
| 이벤트 | description, event_no, items, name, no, reward_condition, status, type | Application, Promotion | Commonevents, Customerevents, Webhooks logs | 9 | ⚪ 선택 | 이벤트 항목 zipcode: 새 우편번호 주소 address: 주소 수정 cellphone: 휴대폰번호 password: 비밀번호 수정 모바일 메시지: 모바일 메시지 수신 동의 email: 이메일 수신 동의 |
| 이벤트 설정 혜택의 상세유형이 1 | gift_product_bundle | Promotion | Benefits | 2 | ⚪ 선택 | 1+N 이벤트 설정 혜택의 상세유형이 1+N 이벤트인 경우 그와 관련한 상세 설정 하위 요소가 입력되어야 정상적인 등록이 가능함 |
| 이벤트 여부 1개 구매시 N개 증정하는 이벤트 여부 | one_plus_n_event | Order | Orders items | 1 | ⚪ 선택 | 1+N이벤트 여부 1개 구매시 N개 증정하는 이벤트 여부 |
| 이용 | available_min_price | Promotion | Discountcodes | 2 | ⚪ 선택 | 이용 주문 최소 금액 DEFAULT 0 |
| 인증 | auth_status, authentication_method | Customer, Notification, Privacy | Customers, Customersprivacy, Sms senders | 3 | ⚪ 선택 | 인증 상태 발신자의 전화번호의 인증 상태. 인증완료 상태인 발신자로만 SMS 를 발송할 수 있다. 00 : 삭제 10 : 등록 20 : 심사중 30 : 인증완료 40 : 반려 |
| 인증여부 | verify | Promotion | Serialcoupons issues | 1 | ⚪ 선택 | 인증여부 Y:인증 N:미인증 |
| 인증일시 | verify_datetime | Promotion | Serialcoupons issues | 1 | ⚪ 선택 | 인증일시 |
| 일정기간 | issue_no_purchase_period | Promotion | Coupons | 2 | ⚪ 선택 | 일정기간 미구매 대상 회원의 미구매 기간 일정 기간 미구매 회원 대상 발급시 발급 조건으로 설정한 구매이력이 없는 기간 |
| 입금자 | bank_code_name | Order | Orders, Orders migrations | 3 | ⚪ 선택 | 입금자 은행명 |
| 입금자명 | billing_name | Order | Orders payments, Unpaidorders | 2 | ⚪ 선택 | 입금자명 결제수단을 무통장입금으로 변경할 경우("change_payment_method:"T"이고 "payment_method":"cash"일 경우) 사용 가능 |
| 입력값 | input_scope | Order | Orderform properties | 2 | ⚪ 선택 | 입력값 적용 범위 (공통 또는 상품별) A : 공통으로 한번만 입력 받기 P : 상품별로 입력 받기 |
| 입력일 | created_datetime | Order | Orders paymenttimeline | 1 | ⚪ 선택 | 입력일 |
| 자동 | auto_login, auto_sort, auto_translation, auto_update_criteria, interval_auto_update, interval_month, interval_week, issue_reserved, issue_reserved_date, offer_only_one_in_automatic, send_method, translation_items | Customer, Product, Promotion, Store | Automessages setting, Benefits setting, Categories products, Coupons, Customergroups setting, Products setting, Serialcoupons, Socials kakaosync | 14 | ⚪ 선택 | 자동 번역 항목 product_name : 상품명 summary_description : 상품요약설명 simple_description : 상품간략설명 description : 상품상세설명 category_name : 상품 분류 option : 옵션 material : 상품소재 |
| 자동로그인 | auto_login_flag | Customer | Customers plusapp | 1 | ⚪ 선택 | 자동로그인 설정 여부 |
| 자동입금 | auto_paid | Order | Payments | 2 | ⚪ 선택 | 자동입금 여부 T: 자동입금 F: 수동입금 |
| 자동진열 | display_count, display_no, use_autodisplay | Category | Autodisplay, Mains | 4 | ⚪ 선택 | 자동진열 T : 사용함 F : 사용안함 |
| 자주 | comment_no, since_comment_no | Community | Commenttemplates | 3 | ⚪ 선택 | 자주 쓰는 답변 번호 |
| 자체 | custom_properties, custom_variant_code, property_name, property_no, property_value | Order, Product | Orders items, Products, Products customproperties, Products variants | 8 | ⚪ 선택 | 자체 품목 코드 Youtube shopping 이용 시에는 미제공 사용자가 품목에 부여 가능한 코드. 재고 관리 등의 이유로 자체적으로 상품을 관리하고 있는 경우 사용함. |
| 자체분류 | classification_code, classification_description, classification_name | Collection, Product | Classifications, Products | 4 | ⚪ 선택 | 자체분류 코드 ,(콤마)로 여러 건을 검색할 수 있다. |
| 자체상품 코드 | custom_product_code | Order, Product | Bundleproducts, Orders items, Products | 5 | ⚪ 선택 | 자체상품 코드 검색어를 자체상품코드에 포함하고 있는 상품 검색(대소문자 구분 필요) ,(콤마)로 여러 건을 검색할 수 있다. |
| 자체품목코드 | duplicated_custom_variant_code | Product | Products variants | 1 | ⚪ 선택 | 자체품목코드 중복여부 T : 중복됨 F : 중복안됨 |
| 작은목록이미지 | tiny_image | Product | Bundleproducts, Products, Products images | 6 | ⚪ 선택 | 작은목록이미지 Youtube shopping 이용 시에는 미제공 상품 상세 화면 하단에 표시되는 상품 목록 이미지. |
| 잔액 | balance | Mileage | Credits | 1 | ⚪ 선택 | 잔액 |
| 재구매 | repurchase_restriction, repurchase_sale | Product, Promotion | Benefits, Bundleproducts, Products | 6 | ⚪ 선택 | 재구매 제한 Youtube shopping 이용 시에는 미제공 T : 재구매 불가 F : 제한안함 DEFAULT F |
| 적립 | reason | Mileage | Points | 2 | ⚪ 선택 | 적립 사유 적립금을 증가/차감하는 사유를 입력할 수 있다. |
| 적용 | available_amount_type, available_product_type, available_scope, category_list, product_list | Order, Promotion, Store | Coupons, Orderform properties, Serialcoupons, Subscription shipments setting | 10 | ⚪ 선택 | 적용 계산 기준 쿠폰을 적용할 기준이 되는 결제 금액. 쿠폰할인을 각종 할인(회원등급할인, 상품할인 등)전 주문금액에 적용할지, 각종 할인 후 금액에 적용할지 여부. |
| 절사 | discount_truncation_unit, rounding_rule | Promotion, Shipping, Supply | Discountcodes, Shipping additionalfees, Shipping suppliers additionalfees | 4 | ⚪ 선택 | 절사 단위 C : 0.01단위 B : 0.1단위 F : 절사안함 O : 1원단위 T : 10원단위 M : 100원단위 H : 1000원 단위 |
| 절사단위 | rounding_unit | Shipping, Supply | Shipping additionalfees, Shipping suppliers additionalfees | 2 | ⚪ 선택 | 절사단위 F : 절사안함 0 : 1원단위 1 : 10원단위 2 : 100원단위 3 : 1000원단위 |
| 접근가능 | permission_shop_no | Supply | Suppliers users | 2 | ⚪ 선택 | 접근가능 쇼핑몰 멀티쇼핑몰 구분을 위해 사용하는 멀티쇼핑몰 번호. |
| 접근권한 | access_authority | Category | Categories | 1 | ⚪ 선택 | 접근권한 F : 모두 이용 가능 T : 회원만 이용가능 G : 특정회원등급만 이용 가능 A : 특정 운영자만 이용 가능 |
| 접속 | access_permission, device, password | Order, Store, Supply | Orders calculation, Suppliers users, Users | 4 | ⚪ 선택 | 접속 허용 권한 T : 접속 허용시간 설정과 상관없이 항상 관리자 페이지 접속을 허용함 F : 사용안함 |
| 접수거부 | undone | Order | Cancellationrequests, Exchangerequests, Orders exchangerequests, Returnrequests | 8 | ⚪ 선택 | 접수거부 여부 T : 접수거부함 |
| 정렬 | display_order, order, sort, sorting_type | Community, Order, Product, Promotion, Store | Boards, Bundleproducts, Coupons setting, Discountcodes, Orders migrations, Products, Reservations, Unpaidorders | 9 | ⚪ 선택 | 정렬 순서 값 discount_code_name : 혜택이름 discount_code : 할인코드 created_date : 등록시간 available_start_date : 시작시간 available_end_date : 종료시간 DEFAULT created_date |
| 정렬순서 | display_sort | Category | Autodisplay | 2 | ⚪ 선택 | 정렬순서 정렬 조건(RD, RA, UD, UA, NA, ND, PD, PA, SD, SA, AD, AA, LD, LA)은 use_hashtag가 "T"일 경우에만 사용 가능 AOD: 주문 수 높은 순서대로 AOA: 주문 수 낮은 순서대로 AVD: 조회 수 높은 순서대로 AVA: 조회 수 낮은 순서대로 ARD: 주문율 높은 순서대로 ARA: 주문율 낮은 순서대로 ACD: 클릭 가치 높은 순서대로 AND: 신규 등록된 순서대로 APD: 판매가 높은 순서대로 APA: 판매가 낮은 순서대로 RD : 최근 등록상품이 위로 RA : 최근 등록상품이 아래로 UD : 최근 수정상품이 위로 UA : 최근 수정상품이 아래로 NA : 상품명 가나다순 ND : 상품명 가나다역순 PD : 판매가 높은 상품이 위로 PA : 판매가 높은 상품이 아래로 SD : 판매량 높은 상품이 위로 SA : 판매량 높은 상품이 아래로 CD : 조회수가 높은 상품이 위로 CA : 조회수가 높은 상품이 아래로 LD : 좋아요수 |
| 정산 | collection_date, collection_hour | Salesreport | Reports hourlysales, Reports productsales, Reports salesvolume | 5 | ⚪ 선택 | 정산 수집 시간 수집 시간을 특정하여 검색 00 ~ 23 까지의 값을 입력할 수 있다. |
| 정산시작 | payment_start_date, payment_start_day | Supply | Suppliers | 2 | ⚪ 선택 | 정산시작 요일 정산주기가 주간정산(B)일 경우 아래 요일에 따라 정산이 진행됨. 0 : 일요일마다 정산 진행 1 : 월요일마다 정산 진행 2 : 화요일마다 정산 진행 3 : 수요일마다 정산 진행 4 : 목요일마다 정산 진행 5 : 금요일마다 정산 진행 6 : 토요일마다 정산 진행 0 : 일요일 1 : 월요일 2 : 화요일 3 : 수요일 4 : 목요일 5 : 금요일 6 : 토요일 |
| 정산유형 | payment_type | Supply | Suppliers | 2 | ⚪ 선택 | 정산유형 공급사에 지불할 금액을 어떤 유형으로 정산할 것인지 설정할 수 있음. 수수료형 : 상품의 판매가격에 수수료를 책정하여 수수료 금액을 반영하여 정산함 매입형 : 상품 등록시 입력한 공급가격을 기준으로 정산함 P : 수수료형 D : 매입형 DEFAULT P |
| 정산종료 | payment_end_date, payment_end_day | Supply | Suppliers | 2 | ⚪ 선택 | 정산종료 요일 정산주기가 주간정산(B)일 경우 아래 요일에 따라 정산이 진행됨. 0 : 일요일마다 정산 진행 1 : 월요일마다 정산 진행 2 : 화요일마다 정산 진행 3 : 수요일마다 정산 진행 4 : 목요일마다 정산 진행 5 : 금요일마다 정산 진행 6 : 토요일마다 정산 진행 0 : 일요일 1 : 월요일 2 : 화요일 3 : 수요일 4 : 목요일 5 : 금요일 6 : 토요일 |
| 정산주기 | payment_period | Supply | Suppliers | 2 | ⚪ 선택 | 정산주기 공급사에 정산을 얼마나 자주할 것인지 설정할 수 있음. 0 : 선택안함 C : 일일정산 B : 주간정산 A : 월간정산 DEFAULT 0 |
| 제외 | except_categories, except_categories_scope, exclude_path | Application, Category | Autodisplay, Scripttags | 4 | ⚪ 선택 | 제외 분류 설정 A: 모든 분류에 적용 C : 이 분류만 적용 DEFAULT A |
| 제조일자 | made_date | Product | Products | 2 | ⚪ 선택 | 제조일자 상품을 제조한 제조일자. |
| 제주 | jeju_surcharge_amount | Shipping, Supply | Regionalsurcharges, Suppliers users regionalsurcharges setting | 4 | ⚪ 선택 | 제주 추가 배송비 |
| 제휴할인 | partner_discount_amount | Order | Cancellation, Exchange, Return | 3 | ⚪ 선택 | 제휴할인 취소액 |
| 조건 | max_value, min_value | Shipping, Supply | Shipping additionalfees, Shipping suppliers additionalfees | 2 | ⚪ 선택 | 조건 최소값 |
| 종료일 | available_end_date | Promotion | Discountcodes | 2 | ⚪ 선택 | 종료일 |
| 종목 | company_line | Privacy, Store, Supply | Customersprivacy, Store, Suppliers | 4 | ⚪ 선택 | 종목 사업자 등록시 공급사에서 등록한 종목 |
| 주/도 | address_state, state | Order, Privacy | Customersprivacy, Orders calculation, Orders receivers, Orders receivers history | 7 | ⚪ 선택 | 주/도 Youtube shopping 이용 시에는 미제공 |
| 주문 | labels, name, names, order_discount_amount, payments_control, permission_amount_inquiry, permission_order_menu, service_data, service_type | Order, Supply | Control, Labels, Orders, Orders items, Orders items labels, Orders paymentamount, Suppliers users | 13 | ⚪ 선택 | 주문 메뉴 접근 권한 T : 사용함 F : 사용안함 DEFAULT T |
| 주문당시 | member_group_no | Order | Orders buyer | 1 | ⚪ 선택 | 주문당시 주문자 회원 등급 번호 |
| 주문상세내역 | display_reject_reason, expose_order_detail, exposed_undone_reason | Order | Cancellation, Cancellationrequests, Exchange, Exchangerequests, Orders cancellation, Orders exchange, Orders exchangerequests, Orders return, Return, Returnrequests | 16 | ⚪ 선택 | 주문상세내역 노출설정 T : 노출함 F : 노출안함 DEFAULT F |
| 주문서 | additional_items, additional_order_info_list, available_coupon_count_by_order, category_no, check_order_info, description, field_length, input_type, is_required, is_simple_join, max_input_length, option_values, order_coupons, order_form_input_type, order_info, order_item_delete, orderform_additional_enabled, orderform_property_id, quick_signup, shipping_info, subject, textarea_rows, width_percentage | Order, Privacy, Promotion, Store | Coupons, Customersprivacy, Orderform properties, Orderform setting, Orders, Orders calculation, Serialcoupons | 13 | ⚪ 선택 | 주문서 추가항목 입력값 input_type를 "R", "C", "S", "I"로 선택 하였을때만 입력 가능 input_type를 "R", "C", "S" 로 입력한 경우 구분자 "/" 로 입력(빨강/노랑/파랑) input_type를 "I" 로 입력한 경우 아래와 같이 시간정보를 입력 예) "{"time_start":"00:00","time_end":"01:00","time_interval":"60"} 예) 빨강/노랑/파랑 |
| 주문수 | order_count | Salesreport | Reports hourlysales | 1 | ⚪ 선택 | 주문수 |
| 주문시 | customer_group_no_when_ordering, group_no_when_ordering | Order | Orders | 1 | ⚪ 선택 | 주문시 회원등급 주문 당시의 회원등급 |
| 주문일 | ordered_date | Order | Orders items | 1 | ⚪ 선택 | 주문일 |
| 중고상품 | product_used_month | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 중고상품 사용 개월 상품 상태(product_condition)가 중고 상품일 경우 중고 상품의 사용 개월 수 |
| 중복발급설정 | allow_duplication | Promotion | Coupons issues | 1 | ⚪ 선택 | 중복발급설정 쿠폰의 중복발급설정 여부. T : 발급함 F : 발급안함 S : 발급안함(사용유무 사용기간 추가검증 안 함) DEFAULT F |
| 중요 | important_flag, starred_memo | Customer, Order | Customers memos, Orders memos | 4 | ⚪ 선택 | 중요 메모 여부 중요 메모의 구분여부. T : 중요 메모 F : 일반 메모 |
| 즉시 | immediate_issue_pause, immediate_issue_restart | Promotion | Coupons | 2 | ⚪ 선택 | 즉시 발급 재개 I 입력 시 status 항목을 restart 로 전송 필요 I : 즉시 발급 재개 |
| 지급 | increase_amount | Mileage | Credits, Credits report | 2 | ⚪ 선택 | 지급 금액 |
| 지역 | region_setting_type, regional_surcharge_amount | Shipping, Supply | Regionalsurcharges, Suppliers users regionalsurcharges, Suppliers users regionalsurcharges setting | 6 | ⚪ 선택 | 지역 설정 방식 A : 간편 설정 N : 지명 설정 Z : 우편번호 설정 |
| 지역명 | surcharge_region_name | Supply | Suppliers users regionalsurcharges | 2 | ⚪ 선택 | 지역명 추가배송비를 부과할 지역이름 지역 설정방식(region_setting_type)이 'N'으로 설정 되어있는 경우 필수 입력 |
| 지역별 | refund_regional_surcharge, regional_surcharge_amount, regional_surcharge_detail, regional_surcharge_list, regional_surcharge_no, return_regional_surcharge, return_regional_surcharge_detail, use_regional_surcharge | Order, Shipping, Supply | Orders, Orders shippingfeecancellation, Refunds, Regionalsurcharges, Return, Suppliers users regionalsurcharges, Suppliers users regionalsurcharges setting | 11 | ⚪ 선택 | 지역별 배송비 사용여부 T : 사용함 F : 사용안함 |
| 진열 | display_order, sequence | Category, Product | Categories, Categories products, Products variants | 5 | ⚪ 선택 | 진열 순서 조합형 옵션 품목에 대해서만 사용 가능함 |
| 진열순서에 | new_product_display_period, normal_product_display_period, product_display_period, recommend_product_display_period | Category | Categories | 2 | ⚪ 선택 | 진열순서에 대한 기간 일반 상품 영역의 진열 방법이 판매량 높은 상품(S), 조회수가 높은 상품(C) 일 경우 기준이 되는 기간 W : 전체기간 1D : 1일 3D : 3일 7D : 7일 15D : 15일 1M : 1개월 3M : 3개월 6M : 6개월 |
| 진열순위 | fix_product_no | Product | Mains products | 2 | ⚪ 선택 | 진열순위 고정 상품번호 진열순위를 고정하고자 하는 상품번호를 지정 |
| 진행여부 | use_benefit | Promotion | Benefits | 2 | ⚪ 선택 | 진행여부 T : 진행함 F : 진행안함 |
| 차감 | decrease_amount | Mileage | Credits, Credits report | 2 | ⚪ 선택 | 차감 금액 |
| 참여대상 | use_group_binding | Promotion | Benefits | 2 | ⚪ 선택 | 참여대상 설정 해당 혜택이 적용되는 대상을 설정 A : 회원 + 비회원 N : 비회원 M : 회원 |
| 처리 | return_code, return_message | Order | Orders completions | 1 | ⚪ 선택 | 처리 결과 메시지 |
| 처리사유 | reason | Mileage, Order | Credits, Orders refunds | 3 | ⚪ 선택 | 처리사유 |
| 처리일시 | process_date | Order, Store | Activitylogs, Orders items history | 2 | ⚪ 선택 | 처리일시 |
| 처리중 | reply_user_id, user_id | Community | Boards articles, Urgentinquiry reply | 4 | ⚪ 선택 | 처리중 또는 답변완료 한 운영자 아이디 |
| 처리한 | manager_id | Order | Orders items history | 1 | ⚪ 선택 | 처리한 운영자 아이디 |
| 철회 | undone, undone_reason, undone_reason_type | Order | Cancellation, Exchange, Orders cancellation, Orders exchange, Orders return, Return | 12 | ⚪ 선택 | 철회 사유 구분 A:고객변심 B:배송지연 J:배송오류 C:배송불가지역 L:수출/통관 불가 D:포장불량 E:상품 불만족 F:상품정보상이 K:상품불량 G:서비스불만족 H:품절 I:기타 |
| 첨부 | attach_file_urls, attached_file_detail, attached_file_urls | Community | Boards articles, Boards articles comments, Boards comments, Urgentinquiry, Urgentinquiry reply | 8 | ⚪ 선택 | 첨부 파일 상세 |
| 첨부파일 | attached_file | Community | Boards articles | 1 | ⚪ 선택 | 첨부파일 여부 T : 있음 F : 없음 |
| 첨부파일용량제한 | attached_file_size_limit | Community | Boards | 2 | ⚪ 선택 | 첨부파일용량제한 (Byte) |
| 총 | subtotal, total_discount_amount, total_order_amount, total_order_count, total_paid_amount, total_paid_count, total_points, total_refund_amount, total_refund_count, total_sales, total_supply_price | Customer, Order, Privacy, Salesreport | Cashreceipt, Customers, Customersprivacy, Orders, Orders calculation, Orders dashboard, Reports salesvolume | 7 | ⚪ 선택 | 총 판매 건수 해당 품목이 검색한 기간 동안 총 판매된 수량 |
| 최근 | last_login_date | Customer, Privacy, Store | Customers, Customersprivacy, Users | 3 | ⚪ 선택 | 최근 접속일시 해당 회원의 최종 로그인 일시 |
| 최대 | available_issue_count, issue_max_count, maximum_quantity | Product, Promotion | Coupons, Discountcodes, Products, Serialcoupons | 7 | ⚪ 선택 | 최대 주문수량 주문 가능한 최대한의 주문 수량. 주문 수량을 초과하여 구매 할 수 없음. 최대 주문수량을 "제한없음"으로 입력하려면 0을 입력 DEFAULT 0 |
| 최상위 | root_category_no | Category | Categories | 1 | ⚪ 선택 | 최상위 분류 번호 해당 상품분류가 속해있는 최상위 상품분류의 분류 번호 표시. |
| 최소 | minimum_quantity | Product | Products | 2 | ⚪ 선택 | 최소 주문수량 주문 가능한 최소한의 주문 수량. 주문 수량 미만으로 구매 할 수 없음. DEFAULT 1 |
| 최종 | coupon_value_final, payment_amount | Order | Orders, Orders coupons | 2 | ⚪ 선택 | 최종 결제 금액 |
| 최초 | expiration_date, first_order, first_payment_date, first_payment_methods, initial_estimated_payment_amount, initial_order_amount, initial_version | Application, Mileage, Order, Store | Apps, Financials store, Orders, Orders payments, Points autoexpiration | 7 | ⚪ 선택 | 최초 결제수단 코드 cash : 무통장 card : 신용카드 cell : 휴대폰 tcash : 계좌이체 icash : 가상계좌 prepaid : 선불금 credit : 예치금 point : 적립금 pointfy : 통합포인트 cvs : 편의점 cod : 후불 giftcard : 제휴상품권 pointcard : 제휴포인트 etc : 기타 |
| 추가 | add_category_no, additional_coupon_no, additional_information, additional_payment_gateway_cancel, additional_shipping_fee, additionalimages, use_additional_coupon | Order, Product, Shipping, Store | Bundleproducts, Coupons setting, Exchangerequests, Orders, Orders exchangerequests, Orders shippingfeecancellation, Paymentgateway, Products, Refunds, Return, Returnrequests, Shipping | 19 | ⚪ 선택 | 추가 분류 번호 Youtube shopping 이용 시에는 미제공 분류 번호를 사용하여 진열을 원하는 카테고리에 상품 등록 |
| 추가발급 | additional_conditions, additional_targets | Promotion | Coupons | 2 | ⚪ 선택 | 추가발급 조건설정 I : 브랜드앱 설치 P : 브랜드앱 푸시ON |
| 추가이미지 | additional_image, additional_image_action | Product, Store | Bundleproducts, Products, Products additionalimages, Products setting | 7 | ⚪ 선택 | 추가이미지 상품 상세 화면 하단에 표시되는 상품의 추가 이미지. 축소 이미지와 비슷한 위치에 표시되며 PC 쇼핑몰에서는 마우스 오버시, 모바일 쇼핑몰에서는 이미지 스와이프(Swipe)시 추가 이미지를 확인할 수 있다. 특정 상품 상세 조회 API에서만 확인 가능하다. |
| 추가입력 | additional_option, additional_option_value, additional_option_values, additional_options, use_additional_option | Order, Personal, Product | Carts, Customers wishlist, Orders items, Orders items options, Products options, Reservations | 8 | ⚪ 선택 | 추가입력 옵션 사용여부 T : 사용함 F : 사용안함 |
| 추가항목 | additional_information, additional_information_key, additional_information_value, use_additional_fields | Privacy, Product, Store | Bundleproducts, Customersprivacy, Orders setting, Products | 9 | ⚪ 선택 | 추가항목 [쇼핑몰 설정 > 상품 설정 > '상품 보기 설정 > 상품 정보 표시 설정']에서 추가한 추가항목. 기본적인 상품 정보 외에 추가로 표시항 항목이 있을 때 추가하여 사용함. |
| 추천 | list_icon | Product | Bundleproducts, Products | 2 | ⚪ 선택 | 추천 / 품절 / 신상품 아이콘 노출 여부 추천, 품절, 신상품 아이콘을 목록에서 표시하는지 여부 ※ 품절 아이콘 ● 상품이 품절 상태임을 알려주는 아이콘 ● 재고관리 및 품절 기능을 사용하는 상품에 대해 재고가 없을 경우 표시 ※ 추천, 신상품 아이콘 ● 상품분류나 메인화면의 추천상품, 신상품 영역에 진열된 상품인 경우, 설정에 따라 해당 아이콘을 표시함 ※ 아이콘 노출 여부 설정위치 : [쇼핑몰 설정 > 상품 설정 > '상품 정책 설정 > 상품 관련 설정 > 상품 아이콘 설정'] |
| 축소이미지 | small_image | Product | Bundleproducts, Products, Products images | 6 | ⚪ 선택 | 축소이미지 Youtube shopping 이용 시에는 미제공 최근 본 상품 영역에 표시되는 상품의 목록 이미지. |
| 출고지 | default, origin_code, origin_name, variants | Product, Shipping | Products variants inventories, Shippingorigins | 5 | ⚪ 선택 | 출고지 기본설정 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 출시일자 | release_date | Product | Products | 2 | ⚪ 선택 | 출시일자 상품이 시장에 출시된 일자. |
| 카드 | transaction_ids | Order | Orders | 1 | ⚪ 선택 | 카드 거래 아이디 |
| 카카오페이 | kakaopay_cancel_reason_type, use_kakaopay | Order, Product, Store | Cancellation, Kakaopay setting, Orders cancellation, Orders shortagecancellation, Products | 7 | ⚪ 선택 | 카카오페이 취소사유 구분 오픈마켓/네이버페이 주문을 취소할 경우 사용 불가 K1 : 변심에 의한 상품 취소 K2 : 다른 옵션이나 상품을 잘못 주문함 K3 : 배송지연 K4 : 상품 파손 또는 불량 K5 : 다른 상품 오배송 또는 구성품 누락 K6 : 상품정보와 다름 K7 : 품절로 인한 배송 불가 |
| 타입 | os_type | Customer | Customers plusapp | 1 | ⚪ 선택 | OS 타입 |
| 통관정보 | clearance_information, clearance_information_type | Order | Orders receivers | 2 | ⚪ 선택 | 통관정보 유형 I : 신분증 ID P : 여권번호 C : 개인통관고유부호 |
| 트렌드 | trend_code, trend_name, use_trend | Collection, Product | Products, Trends | 4 | ⚪ 선택 | 트렌드 코드 트렌드를 등록하면 자동으로 생성되는 코드로 상품에 특정 트렌드를 지정할 때 사용. 미입력시 기본트렌드(T0000000) 사용 |
| 특수지역명 | region_name | Supply | Suppliers users regionalsurcharges | 2 | ⚪ 선택 | 특수지역명 |
| 특정분류 | available_category | Promotion | Discountcodes | 2 | ⚪ 선택 | 특정분류 리스트 할인코드 적용범위(available_product_type)가 C(특정분류) 의 경우 분류번호를 배열로 입력한다. |
| 특정상품 | available_product | Promotion | Discountcodes | 2 | ⚪ 선택 | 특정상품 리스트 할인코드 적용범위(available_product_type)가 P(특정상품) 의 경우 상품번호를 배열로 입력한다. |
| 파일 | attach_file_url1, attach_file_url2, attach_file_url3, attach_file_url4, attach_file_url5, attached_file, attached_file_option, path, use_attached_file_option | Community, Design, Personal, Product | Boards, Boards articles, Customers wishlist, Products options, Themes pages | 8 | ⚪ 선택 | 파일 첨부 옵션 사용여부 T : 사용함 F : 사용안함 |
| 판매안함 | not_for_sale | Product | Categories products | 1 | ⚪ 선택 | 판매안함 여부 |
| 판매완료 | sale_count | Salesreport | Reports productsales | 1 | ⚪ 선택 | 판매완료 수량 |
| 판매처 | sales_channel_icon, sales_channel_id, sales_channel_name | Order | Orders saleschannels | 2 | ⚪ 선택 | 판매처 아이디 |
| 팩스번호 | fax | Store, Supply | Store, Suppliers | 3 | ⚪ 선택 | 팩스번호 공급사의 사업장 팩스번호. |
| 평점 | rating | Community | Boards articles | 2 | ⚪ 선택 | 평점 |
| 표시 | display_position, sequence_no | Product, Promotion | Categories products, Commonevents | 3 | ⚪ 선택 | 표시 위치 top_detail: 상품상세정보 위 side_image: 상품이미지 옆 DEFAULT top_detail |
| 표시기간 | icon_exposure_begin_datetime, icon_exposure_end_datetime, show_end_date, show_start_date, use_icon_exposure_term, use_show_date | Product | Bundleproducts, Products, Products decorationimages, Products icons | 6 | ⚪ 선택 | 표시기간 사용 여부 Youtube shopping 이용 시에는 미제공 T : 사용함 F : 사용안함 |
| 표시대상 | exposure_group_list | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 표시대상 회원 등급 Youtube shopping 이용 시에는 미제공 |
| 표시여부 | use_display | Community | Boards | 2 | ⚪ 선택 | 표시여부 T : 표시함 F : 표시안함 |
| 표시제한 | exposure_limit_type | Product | Bundleproducts, Products | 4 | ⚪ 선택 | 표시제한 범위 Youtube shopping 이용 시에는 미제공 A : 모두에게 표시 M : 회원에게만 표시 DEFAULT A |
| 품목 | image, items, variants | Order, Product | Orders paymentamount, Products, Products variants | 4 | ⚪ 선택 | 품목 리소스 상품당 품목정보를 100개까지 조회할 수 있음. 조회시 Embed 파라메터를 사용하여 조회할 수 있다. |
| 품목 번호 | item_no | Order | Orders items | 1 | ⚪ 선택 | 품주 아이디 품목별 주문번호의 아이디 |
| 품목별 | payment_amount | Order | Orders items, Orders paymentamount, Reservations | 3 | ⚪ 선택 | 품목별 결제금액 쇼핑몰설정 > 주문설정 > 주문 후 설정 > 입금/환불/반품처리 설정 > 취소/교환/반품 접수 시 할인/적립 금액 설정 : 할인금액 자동계산(설정한 이후 접수된 주문부터 적용) 위 옵션을 설정하지 않은 경우 값이 null로 반환됩니다. |
| 품목수 | item_count | Salesreport | Reports hourlysales | 1 | ⚪ 선택 | 품목수 |
| 품목코드 | variants_code | Salesreport | Reports productsales, Reports salesvolume | 3 | ⚪ 선택 | 품목코드 판매 수량을 검색할 품목 코드 조회시 상품번호(product_no)와 품목코드(variant_code) 둘 중에 하나는 반드시 포함하여야한다. |
| 품절상품진열 | soldout_product_display, soldout_sort_type | Category | Categories, Mains | 4 | ⚪ 선택 | 품절상품진열 품절 상품을 상품 분류의 맨 앞 또는 맨 뒤에 진열할 것인지 여부 상품의 품절 여부는 List all products를 통해 sold_out 파라메터로 알 수 있다. B : 품절상품 맨 뒤로 N : 품절상품 상관없음 |
| 품절여부 | sold_out | Product | Bundleproducts, Categories products, Products | 3 | ⚪ 선택 | 품절여부 해당 상품이 품절되었는지 여부. 해당 상품이 재고를 사용하고 있고 모든 품목의 재고가 0이 되면 품절로 표시된다. T : 품절 F : 품절아님 |
| 품절표시 | soldout_message | Product | Products | 2 | ⚪ 선택 | 품절표시 문구 |
| 품절표시여부 | display_soldout | Product | Products variants, Products variants inventories | 4 | ⚪ 선택 | 품절표시여부 재고가 다 판매되었을 경우 해당 품목을 품절로 표시할 것인지 여부. 품절로 표시되면 주문을 할 수 없다. 모든 품목이 품절이 될 경우 해당 상품에 품절 아이콘이 표시된다. "표시안함" 선택시 재고가 다 판매되어도 주문이 가능하며 재고가 마이너스(-)로 표기된다. T : 품절표시 사용 F : 품절표시 사용안함 |
| 품주 | items | Order | Cancellationrequests, Exchangerequests, Orders, Orders migrations, Orders shipments, Refunds, Returnrequests | 13 | ⚪ 선택 | 품주 리소스 조회시 Embed 파라메터를 사용하여 조회할 수 있다. |
| 품주코드 | items | Order | Cancellation, Exchange, Orders cancellation, Orders exchange, Orders return, Orders shortagecancellation, Return | 14 | ⚪ 선택 | 품주코드 |
| 하위분류 | display_sub_category_detail, include_sub_category, sub_category_product_display | Category, Product, Store | Bundleproducts, Categories, Products, Products setting | 5 | ⚪ 선택 | 하위분류 상품진열 현재 상품 분류 하위 분류에 진열된 상품들까지 포함하여 진열할 것인지 여부 T : 진열함 F : 진열안함 |
| 한 | display_lines_desktop, display_lines_mobile | Order | Orderform properties | 2 | ⚪ 선택 | 한 줄에 표시할 옵션 개수 (모바일) input_type를 "R", "C"로 선택 하였을때만 입력 가능 |
| 할인 | allow_using_coupons_with_discounts, discount_limit_begin_date, discount_limit_end_date, discount_limit_information, discount_limit_reset_date, discount_limit_reset_period, discount_limit_reset_week, discount_value, discount_value_unit, discount_values | Customer, Promotion, Store | Coupons setting, Customergroups, Customergroups setting, Discountcodes, Subscription shipments setting | 8 | ⚪ 선택 | 할인 제한설정 멀티쇼핑몰에서 등급별 할인 혜택 제한 사용 시 등급 별로 적용되는 할인 혜택 제한 설정 및 최대 할인 한도 정보. 멀티쇼핑몰에서 등급별 할인 혜택 제한을 사용하지 않거나, buy_benefits(구매 시 할인/적립 혜택)이 F(혜택없음) 또는 M(적립금 지급)일 경우 null로 반환 discount_limit_type(할인 혜택 제한 설정) - A : 제한없음 - B : 할인금액 제한 - C : 할인횟수 제한 discount_amount_limit(최대 할인금액 한도) : discount_limit_type이 B가 아닐 경우 null number_of_discount_limit(최대 할인횟수 한도) : discount_limit_type이 C가 아닐 경우 null로 반환. |
| 할인수단 | discount_method | Order | Orders | 1 | ⚪ 선택 | 할인수단 ,(콤마)로 여러 건을 검색할 수 있다. point : 적립금 credit : 예치금 coupon : 쿠폰 market_discount : 마켓할인 discount_code : 할인코드 |
| 할인율 | discount_rate | Promotion | Coupons, Serialcoupons | 4 | ⚪ 선택 | 할인율 |
| 할인코드 | available_product_type, discount_code, discount_code_name, discount_code_no | Order, Promotion | Discountcodes, Orders | 5 | ⚪ 선택 | 할인코드 적용범위 할인코드의 적용범위가 A(전체상품) 일 경우 할인코드적용 상품(available_product) 및 할인코드적용 분류(available_category) 는 입력 필요 없음 할인코드의 적용범위가 P(특정상품) 일 경우 할인코드적용 상품(available_product) 은 필수 입력 할인코드의 적용범위가 C(특정분류) 일 경우 할인코드적용 분류(available_category)는 필수 입력 A : 전체상품 P : 특정상품 C : 특정분류 DEFAULT A |
| 항목 | properties, property | Customer, Product | Categories properties, Customers properties, Mains properties, Products properties | 11 | ⚪ 선택 | 항목 속성 |
| 해시태그 | hash_tags, use_hashtag | Category | Autodisplay | 2 | ⚪ 선택 | 해시태그 사용여부 T: 사용함 F: 사용안함 |
| 해외 | foreign, international_shipping_fee_criteria, sub_payment_method_code, sub_payment_method_name | Collection, Order, Shipping | Orders, Origin, Shipping | 5 | ⚪ 선택 | 해외 배송비 기준 설정 B : 쇼핑몰 자체 배송비 E : 자동 책정 배송비(EMS) |
| 해외통관용 | clearance_category, clearance_category_eng, clearance_category_info, clearance_category_kor | Order, Product | Bundleproducts, Orders items, Products | 3 | ⚪ 선택 | 해외통관용 상품구분 영문명 해외 통관시 통관용 상품 구분 정보로 사용하는 정보. 국문명 입력시 입력한 구분명이 자동으로 번역된 항목. 번역된 영문명이 해외송장 상품명에 포함되어 전송됨. |
| 해외통관코드 | clearance_category_code | Order, Product | Bundleproducts, Orders items, Products | 5 | ⚪ 선택 | 해외통관코드 배송정보(shipping_scope)가 C(해외배송)일 경우 필수 입력 shipping_calculation이 A(자동계산)일 경우 필수 입력 아님 clearance_category_code |
| 현금영수증 | cash_bill_no, cashreceipt_no | Order | Cashreceipt, Cashreceipt cancellation | 4 | ⚪ 선택 | 현금영수증 일련 번호 |
| 현재 | actual_order_amount, status_code, status_text | Order | Orders, Orders items | 2 | ⚪ 선택 | 현재 주문 금액 실결제금액 중 coupon_shipping_fee_amount는 할인 금액 자동 계산을 사용할 때만 품목별로 배송비 배분이 가능하기 때문에 할인 금액 자동 계산 기능을 사용할 때만 노출됨 |
| 혜택 | auto_reward, benefit_division, benefit_end_date, benefit_percent, benefit_percentage, benefit_percentage_max_price, benefit_percentage_round_unit, benefit_price, benefit_start_date, benefit_title, benefit_type, benefit_value, benefits, benefits_paymethod, coupon_no, discount_max_price, period_type, platform_types, point_amount, use_benefit_period, use_coupon, use_point | Customer, Order, Product, Promotion | Benefits, Bundleproducts, Coupons, Customerevents, Customergroups, Customers coupons, Discountcodes, Orders, Orders benefits, Products, Serialcoupons | 20 | ⚪ 선택 | 혜택 구분 쿠폰으로 받는 혜택의 종류 구분 ,(콤마)로 여러 건을 검색할 수 있다. A : 할인금액 B : 할인율 C : 적립금액 D : 적립율 E : 기본배송비 할인(전액할인) I : 기본배송비 할인(할인율) H : 기본배송비 할인(할인금액) J : 전체배송비 할인(전액할인) F : 즉시적립 G : 예치금 |
| 혜택명 | benefit_name | Order, Promotion | Benefits, Orders benefits | 3 | ⚪ 선택 | 혜택명 |
| 혜택번호 | benefit_no | Order, Promotion | Benefits, Orders benefits | 3 | ⚪ 선택 | 혜택번호 혜택이 생성된 경우 부여되는 고유 번호 |
| 혜택코드 | benefit_code | Order | Orders benefits | 1 | ⚪ 선택 | 혜택코드 |
| 화면 | display_location, top_image_url, use_top_image | Application, Community, Design | Boards, Scripttags, Themes pages | 6 | ⚪ 선택 | 화면 경로 스크립트를 표시할 "화면 경로". 화면 경로는 화면의 페이지 경로가 아니라 쇼핑몰의 각 페이지에 부여된 특정한 역할을 의미함. (예 : 상품분류(product_list)에 스크립트를 삽입할 경우 쇼핑몰에서 상품분류로 사용되는 모든 페이지에 스크립트가 노출됨) 화면의 역할은 해당 페이지에 사용된 모듈에 따라 자동으로 부여됨. 임의의 페이지에 상품분류 모듈을 추가하면 해당 페이지는 "상품분류" 역할로 인식된다. 쇼핑몰 관리자 화면의 [쇼핑몰 설정 > 사이트 설정 > '사이트 환경 설정 > 쇼핑몰 환경 설정 > 화면경로 > 화면경로 설정']에서 각 페이지에 부여된 화면 역할을 조회하고 설정할 수 있음. "all" 일 경우 전체 페이지에 스크립트가 적용됨. display_location_code ,(콤마)로 여러 건을 검색할 수 있다. |
| 회사소개 | about_us_contents, company_introduction | Store, Supply | Store, Suppliers | 3 | ⚪ 선택 | 회사소개 쇼핑몰에 대한 간략한 소개 표시. 쇼핑몰의 회사 소개 화면에 표시된다. |
| 후불 | cod_fees, defer_commission | Order | Cancellation, Exchange, Refunds, Return | 4 | ⚪ 선택 | 후불 결제 수수료 |
| 14세 | junior_purchase_block | Store | Orderform setting | 2 | ⚪ 낮음 | 14세 미만 구매 차단 buy_limit_type를 A(모두 구매 가능)으로 선택하였을때만 설정 가능 T : 사용함 F : 사용안함 |
| 14세미만 | minimum_age_restriction | Store | Customers setting | 2 | ⚪ 낮음 | 14세미만 가입제한 M:인증 후 이용 T:인증없이 바로 이용 F:가입 불가 |
| 19세미만 | adult_age_restriction | Store | Customers setting | 1 | ⚪ 낮음 | 19세미만 가입제한 T:사용함 F:사용안함 |
| 1회구매 | one_time_purchase | Store | Subscription shipments setting | 2 | ⚪ 낮음 | 1회구매 제공여부 T : 제공함 F : 제공안함 DEFAULT T |
| additional_coupon_no | additional_coupon_no | Store | Coupons setting | 1 | ⚪ 낮음 |  |
| available | available | Store | Users | 1 | ⚪ 낮음 | 사용여부 T : 사용함 F : 사용안함 |
| background_image_type | background_image_type | Store | Coupons setting | 2 | ⚪ 낮음 | 기본 쿠폰 배경 이미지 1:TYPE1 2:TYPE2 3:TYPE3 4:TYPE4 5:TYPE5 |
| base_domain | base_domain | Store | Shops, Store | 2 | ⚪ 낮음 | 기본제공 도메인 쇼핑몰 생성시 자동으로 생성되는 기본제공 도메인 정보. 해당 도메인을 통해 쇼핑몰에 접근할 수 있다. |
| basic_name | basic_name | Store | Orders status | 1 | ⚪ 낮음 | 기본 표기 주문상태명 |
| basket_button_size | basket_button_size | Store | Kakaopay setting | 1 | ⚪ 낮음 |  |
| client_id | client_id | Store | Socials apple | 1 | ⚪ 낮음 | client id |
| custom_name | custom_name | Store | Orders status | 2 | ⚪ 낮음 | 사용자 정의 주문상태명 |
| default | default | Store | Shops | 1 | ⚪ 낮음 | 기본샵 여부 기본샵 여부 구분 T : 기본샵 F : 기본샵 아님 |
| default_sender | default_sender | Store | Sms setting | 2 | ⚪ 낮음 | 기본 발신번호 |
| discount_values | discount_values | Store | Subscription shipments setting | 1 | ⚪ 낮음 |  |
| download_image_type | download_image_type | Store | Coupons setting | 2 | ⚪ 낮음 | 기본 쿠폰 다운로드 이미지 1:TYPE1 2:TYPE2 3:TYPE3 4:TYPE4 5:TYPE5 |
| expiration_notice_date_setting | expiration_notice_date_setting | Store | Coupons setting | 1 | ⚪ 낮음 |  |
| footer_tag | footer_tag | Store | Seo setting | 2 | ⚪ 낮음 | Body HTML(PC) |
| gender | gender | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 해당 회원의 성별 |
| header_tag | header_tag | Store | Seo setting | 2 | ⚪ 낮음 | Head HTML(PC) |
| javascript_key | javascript_key | Store | Socials kakaosync | 2 | ⚪ 낮음 | JavaScript 키 |
| key_id | key_id | Store | Socials apple | 1 | ⚪ 낮음 | Key ID |
| language_name | language_name | Store | Shops | 1 | ⚪ 낮음 | 기본 언어명 멀티쇼핑몰의 기본 언어명 |
| max_coupon_count | max_coupon_count | Store | Coupons setting | 1 | ⚪ 낮음 |  |
| mobile_robots_text | mobile_robots_text | Store | Seo setting | 2 | ⚪ 낮음 | 검색로봇 접근 제어(모바일) |
| og_board | og_board | Store | Seo setting | 1 | ⚪ 낮음 |  |
| og_category | og_category | Store | Seo setting | 1 | ⚪ 낮음 |  |
| og_main | og_main | Store | Seo setting | 1 | ⚪ 낮음 |  |
| og_product | og_product | Store | Seo setting | 1 | ⚪ 낮음 |  |
| optimum_discount_price_text | optimum_discount_price_text | Store | Categories properties setting, Mains properties setting, Products properties setting | 3 | ⚪ 낮음 |  |
| order_info | order_info | Store | Orderform setting | 1 | ⚪ 낮음 |  |
| print_type | print_type | Store | Orderform setting | 1 | ⚪ 낮음 |  |
| product_detail_button_size | product_detail_button_size | Store | Kakaopay setting | 1 | ⚪ 낮음 |  |
| product_discount_price_text | product_discount_price_text | Store | Categories properties setting, Mains properties setting, Products properties setting | 3 | ⚪ 낮음 |  |
| product_image_size | product_image_size | Store | Images setting | 1 | ⚪ 낮음 |  |
| product_tax_type_text | product_tax_type_text | Store | Categories properties setting, Mains properties setting, Products properties setting | 3 | ⚪ 낮음 |  |
| recover_coupon_setting | recover_coupon_setting | Store | Coupons setting | 1 | ⚪ 낮음 |  |
| rest_api_key | rest_api_key | Store | Socials kakaosync | 2 | ⚪ 낮음 | REST API 키 |
| return_url | return_url | Application | Appstore orders | 2 | ⚪ 낮음 | Return Url 사용자가 결제 후 이동해야하는 페이지. 결제 완료 페이지 주소를 입력한다. |
| robots_text | robots_text | Store | Seo setting | 2 | ⚪ 낮음 | 검색로봇 접근 제어(PC) |
| script의 | script_no | Application | Scripttags | 2 | ⚪ 낮음 | script의 고유번호 스크립트의 고유 번호 검색 |
| send_case | send_case | Store | Automessages arguments | 1 | ⚪ 낮음 | 사용 가능 발송 상황 |
| shipping_info | shipping_info | Store | Orderform setting | 1 | ⚪ 낮음 |  |
| since_log_id | since_log_id | Application | Databridge logs, Webhooks logs | 2 | ⚪ 낮음 | 해당 로그 ID 이후 검색 |
| skin_translation | skin_translation | Translation | Translations themes | 1 | ⚪ 낮음 |  |
| stock_recover_individual | stock_recover_individual | Store | Orders setting | 1 | ⚪ 낮음 |  |
| team_id | team_id | Store | Socials apple | 1 | ⚪ 낮음 | Team ID |
| trace_id | trace_id | Application | Databridge logs, Webhooks logs | 2 | ⚪ 낮음 | Trace ID |
| translations | translations | Translation | Translations categories, Translations products, Translations store | 3 | ⚪ 낮음 |  |
| trigger_settings | trigger_settings | Application | Recipes | 1 | ⚪ 낮음 |  |
| use | use | Store | Information, Privacy boards, Privacy join, Privacy orders, Restocknotification setting | 10 | ⚪ 낮음 | 사용 여부 T: 사용함 F: 사용안함 |
| use_account | use_account | Store | Store accounts | 1 | ⚪ 낮음 | 사용여부 T : 사용함 F : 사용안함 |
| use_push | use_push | Store | Automessages setting | 1 | ⚪ 낮음 | PUSH 사용 여부 T: 사용함 F: 사용안함 |
| use_sms | use_sms | Store | Automessages setting, Sms setting | 3 | ⚪ 낮음 | SMS 사용 여부 T: 사용함 F: 사용안함 |
| 가상계좌 | auto_cancel_virtual_account_period | Store | Orders setting | 2 | ⚪ 낮음 | 가상계좌 자동취소 기간 Youtube shopping 이용 시에는 미제공 |
| 가입경로 | join_path | Notification, Privacy | Customersprivacy, Recipientgroups | 4 | ⚪ 낮음 | 가입경로 Youtube shopping 이용 시에는 미제공 P : PC M : 모바일 |
| 가입기준 | join_standard | Store | Customers setting | 2 | ⚪ 낮음 | 가입기준 id:아이디 email:이메일 |
| 가입비 | membership_fee_type | Store | Paymentgateway | 2 | ⚪ 낮음 | 가입비 분류 PRE : 선불 PAD : 후불 FREE : 무료 |
| 가입일 | created_start_date | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 가입일 기준 검색시 검색 시작일 Youtube shopping 이용 시에는 미제공 search_type이 created_date 일 경우 가입일 기준의 검색 시작일. 해당 가입일 이후에 가입한 회원을 검색할 수 있다. |
| 개인정보보호 | privacy_officer_department, privacy_officer_email, privacy_officer_name, privacy_officer_phone, privacy_officer_position | Store | Store | 1 | ⚪ 낮음 | 개인정보보호 책임자 이메일 쇼핑몰 화면에 표시되는 개인정보보호 책임자의 이메일 주소. |
| 개인정보처리방침 | privacy_all | Store | Policy | 2 | ⚪ 낮음 | 개인정보처리방침 전체내용 |
| 결혼기념일 | wedding_anniversary | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 결혼기념일 해당 회원의 결혼기념일 |
| 계약일 | contract_date | Store | Financials paymentgateway | 1 | ⚪ 낮음 | PG 계약일 |
| 계정 | invitation_type | Notification | Customers invitation | 1 | ⚪ 낮음 | 계정 활성화 초대 수단 |
| 공유 이미지 | sns_share_image | Store | Seo setting | 2 | ⚪ 낮음 | SNS 공유 이미지 |
| 관심분야 | interest | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 관심분야 해당 회원의 관심사 |
| 관심상품 | wishlist_registration | Store | Products setting | 1 | ⚪ 낮음 | 관심상품 등록 기능 T : 사용함 F : 사용안함 |
| 구글 | google_search_console, use_google_search_console | Store | Seo setting | 2 | ⚪ 낮음 | 구글 서치 콘솔 사용여부 T : 사용함 F : 사용안함 |
| 구매자 | claim_request, claim_request_auto_accept, claim_request_button_date_type, claim_request_button_exposure, claim_request_button_period, claim_request_type | Store | Orders setting | 2 | ⚪ 낮음 | 구매자 취소/교환/반품 신청버튼 노출 범위 설정 Youtube shopping 이용 시에는 미제공 cancel_N10 : 취소신청 상품준비중 cancel_N20 : 취소신청 배송준비중 cancel_N22 : 취소신청 배송보류 cancel_N21 : 취소신청 배송대기 exchange_N00 : 교환신청 입금전 exchange_N10 : 교환신청 상품준비중 exchange_N20 : 교환신청 배송준비중 exchange_N22 : 교환신청 배송보류 exchange_N21 : 교환신청 배송대기 exchange_N30 : 교환신청 배송중 exchange_N40 : 교환신청 배송완료 return_N30 : 반품신청 배송중 return_N40 : 반품신청 배송완료 |
| 국적 | nationality | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 국적 해당 회원이 "외국인 회원"일 경우, 해당 회원의 국적 |
| 그룹 | group_code | Design | Icons | 2 | ⚪ 낮음 | 그룹 코드 A : 상품 아이콘 B : 게시판 아이콘 C : 카드 아이콘 E : 이벤트 아이콘 |
| 금융제휴여부 | status | Store | Financials paymentgateway | 1 | ⚪ 낮음 | 금융제휴여부 T:제휴함 F: 제휴안함 |
| 기준 | standard_currency_code, standard_currency_symbol | Store | Currency | 1 | ⚪ 낮음 | 기준 화폐 심볼 해당 쇼핑몰의 기본쇼핑몰에서 사용하는 화폐의 화폐 기호. 기준 화폐란 일반적으로 쇼핑몰 운영자가 속한 국가에서 통용되는 화폐를 의미한다. |
| 나이 | age_max, age_min | Notification | Recipientgroups | 2 | ⚪ 낮음 | 나이 검색 최소값 |
| 단문(SMS) | sms_count | Notification | Sms balance | 1 | ⚪ 낮음 | 단문(SMS) 발송 가능 건수 |
| 단위 | unit_system | Store | Shops | 1 | ⚪ 낮음 | 단위 체계 metric : 메트릭 체계 imperial : 야드파운드법 |
| 담긴 | cart_item_direct_purchase | Store | Carts setting | 2 | ⚪ 낮음 | 담긴 상품 확인 및 구매 가능여부 T: 사용함 F: 사용안함 |
| 담당자명 | manager_name | Notification | Sms receivers | 2 | ⚪ 낮음 | 담당자명 |
| 대상 | target | Store | Redirects | 2 | ⚪ 낮음 | 대상 위치 |
| 대표도메인 | primary_domain | Store | Shops, Store | 2 | ⚪ 낮음 | 대표도메인 쇼핑몰에 연결한 대표도메인. 대표도메인을 연결하였을 경우에만 노출된다. |
| 대표디자인 | published_in | Design | Themes | 1 | ⚪ 낮음 | 대표디자인 설정 멀티쇼핑몰 번호 |
| 도메인 | preview_domain | Design | Themes | 1 | ⚪ 낮음 | 도메인 조회 |
| 동의서 | display, no | Store | Privacy boards, Privacy join, Privacy orders | 6 | ⚪ 낮음 | 동의서 표시 화면 JOIN: 회원가입 SIMPLE_ORDER_JOIN: 주문서 간단 회원가입 SHOPPING_PAY_EASY_JOIN: 쇼핑페이 간편가입 |
| 동의서명 | name | Store | Privacy boards, Privacy join, Privacy orders | 3 | ⚪ 낮음 | 동의서명 |
| 드롭쉬핑 | name, use | Store | Store dropshipping | 2 | ⚪ 낮음 | 드롭쉬핑 계정연동 여부 T : 연동함 F : 연동안함 |
| 디자인 | design_purchase_no, skin_code, skin_lock, skin_no, skin_thumbnail_url, skin_translation, type, usage_type | Design, Translation | Icons, Themes, Themes pages, Translations themes | 10 | ⚪ 낮음 | 디자인 용도 구분 S : PC 기본스킨 C : PC 복사된 스킨 I : PC 상속된 스킨 M : 모바일 기본스킨/상속된 스킨 N : 모바일 복사된 스킨 |
| 디자인명 | skin_name | Design | Themes | 1 | ⚪ 낮음 | 디자인명 |
| 디자인센터 | design_product_code | Design | Themes | 1 | ⚪ 낮음 | 디자인센터 상품 코드 |
| 레시피 | recipe_code, recipe_name | Application | Recipes | 2 | ⚪ 낮음 | 레시피 코드 |
| 로그 | log_id, log_type | Application | Databridge logs, Webhooks logs | 3 | ⚪ 낮음 | 로그 종류 G : 일반 발송 R : 재발송 T : 테스트 발송 |
| 리다이렉트 | id, path | Store | Redirects | 2 | ⚪ 낮음 | 리다이렉트 아이디 |
| 매매보호 | purchase_protection_amount | Store | Payment setting | 1 | ⚪ 낮음 | 매매보호 적용 결제금액 설정 |
| 메뉴 | menu_access_authority, menu_no, mode, path | Store | Menus, Users | 3 | ⚪ 낮음 | 메뉴 모드 new_pro: PC 어드민 mobile_admin : 모바일 어드민 DEFAULT new_pro |
| 메뉴명 | name | Store | Menus | 1 | ⚪ 낮음 | 메뉴명 |
| 메시지 | string_length | Store | Automessages arguments | 1 | ⚪ 낮음 | 메시지 표시 최대 글자수 글자수 : 설정된 글자수 만큼 표시 가변 : 글자수 제한 없이 모두 표시 |
| 메인 | og_main | Store | Seo setting | 2 | ⚪ 낮음 | 메인 화면 설정 |
| 메일 | type | Notification | Automails | 2 | ⚪ 낮음 | 메일 항목 automails_typecode |
| 모드 | mode | Store | Activitylogs | 2 | ⚪ 낮음 | 모드 P : PC 어드민 M : 모바일 어드민 S : (구)스마트모드 |
| 모바일) | mobile_footer_tag, mobile_header_tag | Store | Seo setting | 2 | ⚪ 낮음 | Head HTML(모바일) |
| 무료 | unsubscribe_phone | Store | Sms setting | 2 | ⚪ 낮음 | 무료 수신거부 전화번호 |
| 무이자 | installments | Store | Payment freeinstallments | 1 | ⚪ 낮음 | 무이자 할부 정보 목록 |
| 무통장입금 | auto_cancel_cash_period, auto_cancel_cash_unit | Store | Orders setting | 2 | ⚪ 낮음 | 무통장입금 자동취소 단위 Youtube shopping 이용 시에는 미제공 D : 일단위 T : 시간단위 |
| 발송그룹 | group_description, group_member_count, group_no | Notification | Recipientgroups | 3 | ⚪ 낮음 | 발송그룹 회원 수 |
| 발송그룹명 | group_name | Notification | Recipientgroups | 2 | ⚪ 낮음 | 발송그룹명 |
| 발송방법 (자동) L | send_method_automatic | Store | Sms setting | 2 | ⚪ 낮음 | SMS 발송방법 (자동) L: 장문발송(3건차감) S: 단문 분할발송 N: 단문발송 |
| 발송방법 S | send_method | Store | Sms setting | 2 | ⚪ 낮음 | SMS 발송방법 S: 단문 분할발송 L: 장문발송(3건 차감) |
| 발신자 | sender, sender_no | Notification | Sms, Sms senders | 2 | ⚪ 낮음 | 발신자 아이디 발신자의 고유한 일련번호 |
| 발신전용 | notification_only_email | Store | Store | 1 | ⚪ 낮음 | 발신전용 이메일 고객과 운영자에게 자동메일 발송시 보내는 사람 메일주소 |
| 발음표기 | name_phonetic | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 발음표기 이름 (일본어) 해당 회원의 발음 표기 이름(일본어) |
| 버전 | version, version_expiration_date | Application | Apps | 2 | ⚪ 낮음 | 버전 만료일 |
| 버튼 | available_product, available_product_list, button_show_method, button_show_target, is_button_show | Store | Restocknotification setting | 2 | ⚪ 낮음 | 버튼 노출 상품 A:전체상품 P:특정상품 E:제외상품 |
| 번역 | translations | Translation | Translations categories, Translations products, Translations store, Translations themes | 7 | ⚪ 낮음 | 번역 정보 |
| 번호 | no | Notification | Sms receivers | 1 | ⚪ 낮음 | 번호 |
| 법인명 | corporate_name | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 법인명 해당 회원의 법인명 |
| 변수 | description, sample | Store | Automessages arguments | 1 | ⚪ 낮음 | 변수 설명 |
| 변수명 | name | Store | Automessages arguments | 1 | ⚪ 낮음 | 변수명 |
| 비밀번호 | password_recovery | Store | Customers setting | 1 | ⚪ 낮음 | 비밀번호 찾기 방법 설정 T:임시 비밀번호 전송 N:비밀번호 즉시변경 |
| 비즈니스 | business_country | Store | Store | 1 | ⚪ 낮음 | 비즈니스 국가 |
| 빠른 | use_direct_pay | Store | Payment setting | 2 | ⚪ 낮음 | 빠른 결제 수단 사용여부 T : 사용함 F : 사용안함 |
| 사업자 | business_country_code, company_type | Privacy, Store | Customersprivacy, Shops | 2 | ⚪ 낮음 | 사업자 구분 해당 회원의 회원타입이 사업자일경우 p : 개인사업자 c : 법인사업자 |
| 사은품기능 | use_gift | Store | Benefits setting | 2 | ⚪ 낮음 | 사은품기능 사용여부 T : 사용함 F : 사용안함 |
| 사은품제공 | gift_calculation_scope, gift_calculation_type | Store | Benefits setting | 2 | ⚪ 낮음 | 사은품제공 계산방식 total_order : 총 주문금액 기준 actual_payment : 실결제금액 기준 |
| 사이트 | site_connect | Store | Shops | 1 | ⚪ 낮음 | 사이트 접속설정 |
| 사이트맵 | use_sitemap_auto_update | Store | Seo setting | 2 | ⚪ 낮음 | 사이트맵 사용여부 T : 사용함 F : 사용안함 |
| 상품/주문서 | allow_using_product_and_order_coupons | Store | Coupons setting | 2 | ⚪ 낮음 | 상품/주문서 동시사용 T:사용함 F:사용안함 |
| 상품이미지 | image_effect, image_effect_detail | Store | Products setting | 1 | ⚪ 낮음 | 상품이미지 효과 설정 T : 사용함 F : 사용안함 |
| 상품정렬조건 | sorting_options | Store | Products display setting | 2 | ⚪ 낮음 | 상품정렬조건 new_product : 신상품 product_name : 상품명 low_price : 낮은가격 high_price : 높은가격 manufacture : 제조사 popular_product : 인기상품 review : 사용후기 hit_count : 조회수 like_count : 좋아요 |
| 상품준비중 | use_product_prepare_status | Store | Orders setting | 2 | ⚪ 낮음 | 상품준비중 주문상태 사용여부 상품준비중 주문상태 사용 설정에 따라서 아래 설정의 '상품준비중' 기능이 제어됨 - 배송지 변경 버튼 노출 범위 설정: '상품준비중' - 구매자 취소/교환/반품 신청버튼 노출 범위 설정: '상품준비중' T : 사용함 F : 사용안함 |
| 생년월일 | use_update_birthday | Store | Customers setting | 2 | ⚪ 낮음 | 생년월일 수정 T:허용함 F:허용안함 |
| 생일 | birthday | Privacy | Customersprivacy | 2 | ⚪ 낮음 | 생일 Youtube shopping 이용 시에는 미제공 |
| 설정할 | period | Store | Carts setting | 2 | ⚪ 낮음 | 설정할 저장기간 장바구니 저장기간은 1,2,3,4,5,6,7,8,9,10,14,30일 중 설정 가능 |
| 세팅일 | setting_date | Store | Financials paymentgateway | 1 | ⚪ 낮음 | PG 세팅일 |
| 소비자가 | strikethrough_retail_price | Store | Categories properties setting, Mains properties setting, Products properties setting | 6 | ⚪ 낮음 | 소비자가 취소선 표시 T : 사용함 F : 사용안함 |
| 소스 | source | Design | Themes pages | 2 | ⚪ 낮음 | 소스 코드 |
| 수신거부자 | exclude_unsubscriber | Notification, Store | Sms, Sms setting | 3 | ⚪ 낮음 | 수신거부자 제외 발송 여부 수신거부자를 제외하고 발송할지 여부를 설정할 수 있음. T : 제외 F : 포함 DEFAULT T |
| 수신동의 | agree_point, agree_restriction_period | Store | Points setting | 2 | ⚪ 낮음 | 수신동의 변경 불가 기간 1:1개월 3:3개월 6:6개월 12:1년 |
| 수신자 | recipient_type, recipients | Notification | Sms, Sms receivers | 3 | ⚪ 낮음 | 수신자 구분 ALL:전체 S:공급사 A:운영자 |
| 스크립트 | created_end_date, created_start_date, updated_end_date, updated_start_date | Application | Scripttags | 1 | ⚪ 낮음 | 스크립트 설치일 검색 시작일 스크립트 설치 날짜가 해당 날짜 이후인 스크립트 검색 검색 종료일과 같이 사용해야함. |
| 스크립트를 설치한 Client의 ID | client_id | Application | Scripttags | 1 | ⚪ 낮음 | Client ID 스크립트를 설치한 Client의 ID |
| 스킨 | skin_no | Application | Scripttags | 2 | ⚪ 낮음 | 스킨 번호 스크립트를 적용할 스킨 번호 ,(콤마)로 여러 건을 검색할 수 있다. |
| 실시간 | scopes | Application | Webhooks setting | 1 | ⚪ 낮음 | 실시간 정보제공 권한 |
| 심사일자 | review_date | Store | Paymentgateway | 1 | ⚪ 낮음 | 심사일자 |
| 아이디저장 | save_member_id | Store | Customers setting | 1 | ⚪ 낮음 | 아이디저장 T:사용함 F:사용안함 |
| 안내 | type | Store | Information | 2 | ⚪ 낮음 | 안내 유형 information_type |
| 애플 | use_apple_login, use_certification | Store | Socials apple | 2 | ⚪ 낮음 | 애플 로그인 본인인증 T : 사용함 F : 사용안함 |
| 애플 개발자 센터의 App ID Prefix | team_id | Store | Socials apple | 1 | ⚪ 낮음 | Team ID 애플 개발자 센터의 App ID Prefix |
| 애플 개발자 센터의 Key ID | key_id | Store | Socials apple | 1 | ⚪ 낮음 | Key ID 애플 개발자 센터의 Key ID |
| 애플 개발자 센터의 Service ID 생성 시 설정한 | client_id | Store | Socials apple | 1 | ⚪ 낮음 | Client ID 애플 개발자 센터의 Service ID 생성 시 설정한 Identifier |
| 어드민 | admin_language | Store | Users | 1 | ⚪ 낮음 | 어드민 언어 ko_KR : 한국어 en_US : 영어 ja_JP : 일본어 |
| 언어 | language_code | Design, Store, Translation | Shops, Themes, Translations categories, Translations products, Translations store, Translations themes | 6 | ⚪ 낮음 | 언어 코드 번역 정보의 언어 코드에 해당되는 번역 정보를 검색 언어별로 번역된 정보에서 검색하고자 하는 언어를 선택하면, 해당 언어에 대한 번역 내용을 확인할 수 있습니다. ,(콤마)로 여러 건을 검색할 수 있다. |
| 업무처리 | process_no | Store | Activitylogs | 2 | ⚪ 낮음 | 업무처리 넘버 |
| 없는 | missing_page_redirect_url, mobile_missing_page_redirect_url, mobile_use_missing_page_redirect, use_missing_page_redirect | Store | Seo setting | 2 | ⚪ 낮음 | 없는 페이지 연결 리다이렉션 여부(모바일) T : 사용함 F : 사용안함 |
| 에디터 | editor_type | Design | Themes | 1 | ⚪ 낮음 | 에디터 타입 H : 스마트 디자인 (HTML) D : 에디봇 디자인 (Drag & Drop) W : 심플 디자인 (WYSIWYG) E : 스마트디자인Easy C : 콘텐츠스튜디오(Contents Studio) |
| 에스크로(가상계좌) | use_escrow_virtual_account | Store | Payment setting | 2 | ⚪ 낮음 | 에스크로(가상계좌) 사용여부 T : 사용함 F : 사용안함 |
| 에스크로(계좌이체) | use_escrow_account_transfer | Store | Payment setting | 2 | ⚪ 낮음 | 에스크로(계좌이체) 사용여부 T : 사용함 F : 사용안함 |
| 연동사(ECP/독립몰)에서 | pixel_code | Store | Kakaopay setting | 2 | ⚪ 낮음 | 연동사(ECP/독립몰)에서 이미 사용중인 카카오 광고 픽셀 ID |
| 연동중인 | sns_list | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 연동중인 SNS |
| 영문이름 | name_english | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 영문이름 해당 회원의 영문 이름 |
| 예약주문 | reservation_custom_name, reservation_order | Store | Orderform setting, Orders status | 4 | ⚪ 낮음 | 예약주문 T : 사용함 F : 사용안함 |
| 외국인 | foreigner_type | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 외국인 인증방법 해당 외국인 회원의 인증방법 f : 외국인등록번호 p : 여권번호 d : 국제운전면허증 |
| 운영자 | admin_type, nick_name, use_admin, user_id, user_name | Notification, Privacy, Store | Automails, Customersprivacy, Sms receivers, Users | 8 | ⚪ 낮음 | 운영자 구분 대표운영자인지 부운영자인지의 구분 P : 대표운영자 A : 부운영자 |
| 운영자명 | user_name | Notification | Sms receivers | 2 | ⚪ 낮음 | 운영자명 |
| 원본 | src | Application | Scripttags | 2 | ⚪ 낮음 | 원본 script 경로 설치할 스크립트의 원본 경로(절대 경로) |
| 월간 | monthly_sales_stats | Store | Dashboard | 1 | ⚪ 낮음 | 월간 매출 현황 월간 단위의 매출 현황 정보 |
| 웹훅 | reception_status, success | Application | Databridge logs, Webhooks logs, Webhooks setting | 6 | ⚪ 낮음 | 웹훅 발송 성공 여부 T : 성공 F : 실패 |
| 유튜브쇼핑 | youtube_shops_logo | Store | Store | 1 | ⚪ 낮음 | 유튜브쇼핑 로고 이미지 |
| 응답 | response_body, response_http_code | Application | Databridge logs, Webhooks logs | 2 | ⚪ 낮음 | 응답 http code |
| 이름 inicis | payment_gateway_name | Store | Financials paymentgateway | 1 | ⚪ 낮음 | PG 이름 inicis : 이니시스 kcp : KCP allat : 올앳 ksnet : KSNET dacom : 토스페이먼츠 allthegate : 올더게이트 settlebank : 세틀뱅크 smartro : 스마트로 kicc : 한국정보통신 mobilians : 모빌리언스 danal : 다날 |
| 이용가능한 | available_shop_no | Store | Paymentgateway paymentmethods | 2 | ⚪ 낮음 | 이용가능한 멀티쇼핑몰 번호 |
| 이전 | previous_version | Application | Apps | 1 | ⚪ 낮음 | 이전 버전 |
| 인기 | popular_search_keywords | Store | Products setting | 1 | ⚪ 낮음 | 인기검색어 |
| 인쇄버튼 | print_type | Store | Orderform setting | 2 | ⚪ 낮음 | 인쇄버튼 타입 |
| 일일 | daily_sales_stats | Store | Dashboard | 1 | ⚪ 낮음 | 일일 현황 정보 일 단위의 매출 현황 정보 |
| 입점시 | button_authorization_key, shop_key | Store | Kakaopay setting | 2 | ⚪ 낮음 | 입점시 부여 받는 판매점의 고유 식별자 |
| 자동번역 | use_translation | Store | Shops | 1 | ⚪ 낮음 | 자동번역 |
| 장문(LMS) | lms_count | Notification | Sms balance | 1 | ⚪ 낮음 | 장문(LMS) 발송 가능 건수 |
| 장바구니 | add_action_type, basket_product_no, icon_display, storage_period, wishlist_display | Personal, Store | Carts, Carts setting | 3 | ⚪ 낮음 | 장바구니 담기 이후 액션 타입 M: 장바구니 페이지 바로 이동 S: 장바구니 페이지 이동 유무 선택 |
| 장바구니에 | discount_display | Store | Carts setting | 2 | ⚪ 낮음 | 장바구니에 할인 금액 표시 T: 사용함 F: 사용안함 |
| 장바구니에서 | cart_item_option_change | Store | Carts setting | 2 | ⚪ 낮음 | 장바구니에서 상품 옵션 변경가능 하도록 제공 여부 T: 사용함 F: 사용안함 |
| 저장 | save_type | Store | Information, Policy, Privacy boards, Privacy join, Privacy orders | 5 | ⚪ 낮음 | 저장 방식 S: 표준 약관 적용 C: 사용자 정의 약관 적용 DEFAULT S |
| 전송일시 | requested_time | Application | Databridge logs, Webhooks logs | 2 | ⚪ 낮음 | 전송일시 |
| 접근 제한 | ip_access_restriction | Store | Users | 1 | ⚪ 낮음 | IP 접근 제한 |
| 접근제한 IP 접근제한의 | ip_restriction_type | Store | Users | 1 | ⚪ 낮음 | IP 접근제한 IP 접근제한의 사용여부 A : 사용함 F : 사용안함 |
| 정기과금 | automatic_payment | Application | Appstore orders, Appstore payments | 3 | ⚪ 낮음 | 정기과금 여부 T : 사용함 F : 사용안함 DEFAULT F |
| 정산입금 | bank_account_name, bank_account_no, bank_code | Store | Financials paymentgateway | 1 | ⚪ 낮음 | 정산입금 은행코드 은행 코드 조회하기 |
| 제3자 | thirdparty_agree, thirdparty_agree_date | Privacy, Store | Customersprivacy, Kakaopay setting, Socials kakaosync | 5 | ⚪ 낮음 | 제3자 제공 동의 여부 Youtube shopping 이용 시에는 미제공 T : 동의함 F : 동의안함 |
| 주간 | weekly_sales_stats | Store | Dashboard | 1 | ⚪ 낮음 | 주간 매출 현황 주간 단위의 매출 현황 정보 |
| 주문명 | order_name | Application | Appstore orders | 2 | ⚪ 낮음 | 주문명 앱스토어 주문의 주문 이름. 주문 생성시 지정이 가능하며, 사용자가 결제시 해당 결제의 내용이 무엇인지 알 수 있는 내용이어야 함. |
| 중국/대만 | china_taiwan_id_input | Store | Orderform setting | 2 | ⚪ 낮음 | 중국/대만 신분증 ID 입력 T : 사용함 F : 사용안함 |
| 중량 | weight_unit | Store | Shops | 1 | ⚪ 낮음 | 중량 단위 kg : 킬로그램 g : 그램 lb : 파운드 oz : 온스 |
| 지역코드 | residence | Privacy | Customersprivacy | 2 | ⚪ 낮음 | 지역코드 Youtube shopping 이용 시에는 미제공 해당 회원의 주거지역 ,(콤마)로 여러 건을 검색할 수 있다. |
| 직업 | job | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 직업 해당 회원의 직업 |
| 직종 | job_class | Privacy | Customersprivacy | 1 | ⚪ 낮음 | 직종 해당 회원의 직종 |
| 참조 | reference_currency_code, reference_currency_name | Store | Shops | 1 | ⚪ 낮음 | 참조 화폐 코드 멀티쇼핑몰의 참조 화폐 코드 South Korean Won (KRW) United States Dollar (USD) Japanese Yen (JPY) Chinese Yuan (CNY) |
| 채널 | channel | Store | Shops | 1 | ⚪ 낮음 | 채널 |
| 처리자 | manager_id, manager_type | Store | Activitylogs | 2 | ⚪ 낮음 | 처리자 타입 P : 대표운영자 A : 부운영자 S : 공급사 |
| 청약철회방침 | required_withdrawal, use_withdrawal, withdrawal | Store | Policy | 2 | ⚪ 낮음 | 청약철회방침 사용자 동의 필수 여부 T : 필수 F : 선택 |
| 최적할인가 | optimum_discount_price_text | Store | Categories properties setting, Mains properties setting, Products properties setting | 6 | ⚪ 낮음 | 최적할인가 할인금액 표시문구 |
| 추천인아이디 | recommend_id | Privacy | Customersprivacy | 2 | ⚪ 낮음 | 추천인아이디 Youtube shopping 이용 시에는 미제공 |
| 카카오 | kakao_senderkey | Store | Kakaoalimtalk profile | 1 | ⚪ 낮음 | 카카오 채널 발신 프로필 키 |
| 카카오싱크 | use_kakaosync | Store | Socials kakaosync | 1 | ⚪ 낮음 | 카카오싱크 사용여부 T : 사용함 F : 사용안함 |
| 카카오알림톡 | use_kakaoalimtalk | Store | Automessages setting, Kakaoalimtalk setting | 3 | ⚪ 낮음 | 카카오알림톡 사용 여부 T: 사용함 F: 사용안함 |
| 큐 | queue_code | Notification | Sms | 1 | ⚪ 낮음 | 큐 코드 |
| 크롤러 접근 제어 | llms_text | Store | Seo setting | 2 | ⚪ 낮음 | AI 크롤러 접근 제어 |
| 클라이언트 | client_id, client_secret | Store | Socials naverlogin | 2 | ⚪ 낮음 | 클라이언트 시크릿 키 |
| 탈퇴사유 | unregistration_reason | Store | Customers setting | 1 | ⚪ 낮음 | 탈퇴사유 T:사용함 F:사용안함 |
| 통신 | mail_order_sales_registration | Store | Store | 1 | ⚪ 낮음 | 통신 판매업 신고 통신판매업 신고가 되었는지 신고 여부 T : 신고함 F : 신고안함 |
| 통신판매신고 | mail_order_sales_registration_number | Store | Store | 1 | ⚪ 낮음 | 통신판매신고 번호 |
| 통신판매업 | missing_report_reason, missing_report_reason_type | Store | Store | 1 | ⚪ 낮음 | 통신판매업 미신고 사유 상세 내용 통신판매업 미신고 사유가 "기타"일 경우 상세 사유. |
| 트리거 | trigger_settings | Application | Recipes | 1 | ⚪ 낮음 | 트리거 설정 |
| 트위터 | use_twitter_card | Store | Seo setting | 2 | ⚪ 낮음 | 트위터 카드 사용여부 T : 사용함 F : 사용안함 |
| 파비콘 | favicon | Store | Seo setting | 2 | ⚪ 낮음 | 파비콘 |
| 파일/디렉토리 | path | Design | Themes pages | 1 | ⚪ 낮음 | 파일/디렉토리 경로 |
| 파일명 | auth_key_file_name | Store | Socials apple | 1 | ⚪ 낮음 | Auth Key 파일명 |
| 파일명 App ID의 Key파일로 | auth_key_file_name | Store | Socials apple | 1 | ⚪ 낮음 | Auth Key 파일명 App ID의 Key파일로 .p8파일만 가능 |
| 판매 | category_tags, sales_product_categories | Store | Store | 1 | ⚪ 낮음 | 판매 상품 카테고리 회원가입 및 쇼핑몰 생성 직후 입력하는 판매 상품 카테고리의 정보를 조회할 수 있습니다. (2023년 4월 이후 가입한 몰에 한하여 조회할 수 있습니다.) Undecided : 아직 결정하지 못했어요. Apparel : 패션의류 FashionAccessories : 패션잡화 LuxuryGoods : 수입명품 BrandApparel : 브랜드의류 BrandAccessories : 브랜드잡화 Food_Beverage : 식품 Lifestyle_HealthCare : 생활/건강 Furniture_HomeDecor : 가구/인테리어 Beauty_PersonalCare : 화장품/미용 Maternity_BabyProducts : 출산/육아 Digital_HomeAppliances : 디지털/가전 CarAccessories : 자동차 Rentals : 렌탈 서비스 Sports_Leisure : 스포츠/레저 CD_DVD : 음반/DVD Books : 도서 Travels_Ser |
| 판매자 | seller_id, seller_skin_code | Design | Themes | 1 | ⚪ 낮음 | 판매자 디자인센터 아이디 |
| 팝업 | popup_menu | Store | Products setting | 1 | ⚪ 낮음 | 팝업 메뉴 T : 사용함 F : 사용안함 |
| 페이센터 | shop_id | Store | Naverpay setting | 2 | ⚪ 낮음 | 페이센터 ID |
| 표준시간대 | date_format, time_format, timezone_name | Store | Shops | 1 | ⚪ 낮음 | 표준시간대 날짜 표시형식 년/월/일 : YYYY-MM-DD 월/일/년 : MM-DD-YYYY 일/월/년 : DD-MM-YYYY |
| 표준시간대(타임존) | timezone | Store | Shops | 1 | ⚪ 낮음 | 표준시간대(타임존) |
| 푸시 | send_method_push | Store | Automessages setting | 2 | ⚪ 낮음 | 푸시 수신 대상에게 푸시 우선 발송 여부 Youtube shopping 이용 시에는 미제공 T : 우선 발송함 F : 우선 발송 안함 |
| 품절 | display_soldout_gifts | Store | Benefits setting | 2 | ⚪ 낮음 | 품절 사은품 표시여부 grayed : 표시하되 선택불가 disabled : 표시하지 않음 |
| 품절된 | sold_out_products_count | Store | Dashboard | 1 | ⚪ 낮음 | 품절된 상품 수 품절된 상품의 수. 재고관리기능과 품절기능이 활성화 되어있을 경우 집계에 포함됨. |
| 피드 | use_rss | Store | Seo setting | 2 | ⚪ 낮음 | RSS 피드 사용여부 T : 사용함 F : 사용안함 |
| 필수/선택 | required | Store | Privacy join | 2 | ⚪ 낮음 | 필수/선택 여부 T : 필수 F : 선택 |
| 하위 | integrity | Application | Scripttags | 2 | ⚪ 낮음 | 하위 리소스 무결성 스크립트 위변조를 방지하기위한 무결성 검증용 해시. (sha384, sha512 해시 알고리즘 지원) Integrity 해시 생성방법 참고 |
| 확장 | extension_type | Application | Apps | 2 | ⚪ 낮음 | 확장 타입 section : 섹션(쇼핑몰 프론트에 html 삽입이 필요한 앱 타입) embedded : 임베디드(쇼핑몰 프론트에 임베디드되어 자동으로 구동되는 앱 타입) |
| 활성화 | active | Application, Store | Recipes, Shops | 2 | ⚪ 낮음 | 활성화 여부 멀티쇼핑몰 활성화 여부 T : 활성화 F : 비활성화 |
| 활성화 여부 | is_https_active | Store | Shops | 1 | ⚪ 낮음 | HTTPS 활성화 여부 T : 활성화 F : 비활성화 |
| 회사약도 | company_map_url | Store | Store | 1 | ⚪ 낮음 | 회사약도 쇼핑몰에 대한 간략한 약도 표시. 쇼핑몰의 회사 소개 화면에 표시된다. |
