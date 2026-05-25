# Cafe24 UDS attribute

Source: https://developers.cafe24.com/docs/api/admin/#orders

Scope: Cafe24 Admin API `Orders` resource — `Orders property list`.

GET API: `GET /api/v2/admin/orders` / `GET /api/v2/admin/orders/{order_id}`

Total attributes: **83**

## 한국어 라벨 목록

- 멀티쇼핑몰 번호
- 화폐단위
- 주문번호
- 마켓 구분값
- 마켓 주문 번호
- 회원아이디
- 회원 이메일
- 회원인증여부
- 결제자명
- 은행코드
- 입금자 은행명
- 결제수단 코드
- 결제수단명
- PG 이름
- 해외 결제수단명
- 해외 결제수단코드
- 카드 거래 아이디
- 결제 여부
- 취소 여부
- 주문일
- 최초 주문여부
- 결제일
- 모바일 구분
- 에스크로 사용여부
- 주문시 회원등급
- 최초 주문 금액
- 현재 주문 금액
- 계좌번호
- 예금주
- 마켓 판매자 아이디
- 최종 결제 금액
- 주문취소일
- 주문경로 텍스트
- 주문경로
- 후불결제 입금확인 가능 여부
- 결제 수수료
- 후불결제여부
- 관리자 입력 금액
- 추가 배송비
- 해외배송 보험료
- 해외배송 부가금액
- 배송 유형
- 배송 유형명
- 배송상태
- 희망배송일
- 희망배송시간
- 희망배송사 코드
- 희망배송사 명
- 반품승인일시
- 총 공급가액
- 네이버포인트
- 주문서 추가항목
- 매장수령여부
- 간편결제 결제사 이름
- 여신상태
- 정기결제 여부
- 품주 리소스
- 수령자정보 리소스
- 주문자정보 리소스
- 배송비 정보
- 지역별 배송비 정보
- 반품상세 리소스
- 취소상세 리소스
- 교환상세 리소스
- 멀티 배송지 여부
- 결제 화폐 환율 정보
- 최초 결제수단 코드
- 네이버페이 PG 결제 정보
- 가격에 세금 포함
- 세금 상세 정보
- 주문 서비스 유형
- 주문 서비스 데이터
- 배송지 정보 표기 여부
- 연동 된 SNS 제공코드
- 연동 된 SNS명
- 주문시 회원등급
- 혜택 리소스
- 쿠폰 리소스
- 환불상세 리소스
- 주문상태
- 품주코드
- 구매확정 여부
- 적립금 회수

## Cafe24 attribute 목록

- `shop_no`
- `currency`
- `order_id`
- `market_id`
- `market_order_no`
- `member_id`
- `member_email`
- `member_authentication`
- `billing_name`
- `bank_code`
- `bank_code_name`
- `payment_method`
- `payment_method_name`
- `payment_gateway_names`
- `sub_payment_method_name`
- `sub_payment_method_code`
- `transaction_ids`
- `paid`
- `canceled`
- `order_date`
- `first_order`
- `payment_date`
- `order_from_mobile`
- `use_escrow`
- `group_no_when_ordering`
- `initial_order_amount`
- `actual_order_amount`
- `bank_account_no`
- `bank_account_owner_name`
- `market_seller_id`
- `payment_amount`
- `cancel_date`
- `order_place_name`
- `order_place_id`
- `payment_confirmation`
- `commission`
- `postpay`
- `admin_additional_amount`
- `additional_shipping_fee`
- `international_shipping_insurance`
- `additional_handling_fee`
- `shipping_type`
- `shipping_type_text`
- `shipping_status`
- `wished_delivery_date`
- `wished_delivery_time`
- `wished_carrier_id`
- `wished_carrier_name`
- `return_confirmed_date`
- `total_supply_price`
- `naver_point`
- `additional_order_info_list`
- `store_pickup`
- `easypay_name`
- `loan_status`
- `subscription`
- `items`
- `receivers`
- `buyer`
- `shipping_fee_detail`
- `regional_surcharge_detail`
- `return`
- `cancellation`
- `exchange`
- `multiple_addresses`
- `exchange_rate`
- `first_payment_methods`
- `naverpay_payment_information`
- `include_tax`
- `tax_detail`
- `service_type`
- `service_data`
- `show_shipping_address`
- `social_member_code`
- `social_name`
- `customer_group_no_when_ordering`
- `benefits`
- `coupons`
- `refunds`
- `process_status`
- `order_item_code`
- `purchase_confirmation`
- `collect_points`

## Attribute dictionary

| # | 한국어 라벨 | Cafe24 attribute | Description |
|---:|---|---|---|
| 1 | 멀티쇼핑몰 번호 | `shop_no` | 멀티쇼핑몰 번호 멀티쇼핑몰 구분을 위해 사용하는 멀티쇼핑몰 번호. |
| 2 | 화폐단위 | `currency` | 화폐단위 해당 멀티쇼핑몰의 화폐단위 |
| 3 | 주문번호 | `order_id` | 주문번호 |
| 4 | 마켓 구분값 | `market_id` | 마켓 구분값 가격 비교 사이트를 통하여 마켓 등에서 상품 구매 시 해당 사이트를 구분하기 위한 ID |
| 5 | 마켓 주문 번호 | `market_order_no` | 마켓 주문 번호 |
| 6 | 회원아이디 | `member_id` | 회원아이디 |
| 7 | 회원 이메일 | `member_email` | 회원 이메일 |
| 8 | 회원인증여부 | `member_authentication` | 회원인증여부 회원 인증여부. 인증여부에 따라 3가지로 회원타입이 나눠짐. T : 승인 B : 특별관리회원 J : 14세미만회원 |
| 9 | 결제자명 | `billing_name` | 결제자명 입금자 이름. 주문자 혹은 수령자 이름과는 다를 수 있음. |
| 10 | 은행코드 | `bank_code` | 은행코드 bank_code |
| 11 | 입금자 은행명 | `bank_code_name` | 입금자 은행명 |
| 12 | 결제수단 코드 | `payment_method` | 결제수단 코드 주문자가 이용한 결제수단의 코드 cash : 무통장 card : 신용카드 cell : 휴대폰 tcash : 계좌이체 icash : 가상계좌 prepaid : 선불금 credit : 예치금 point : 적립금 pointfy : 통합포인트 cvs : 편의점 cod : 후불 coupon : 쿠폰 market_discount : 마켓할인 giftcard : 제휴상품권 pointcard : 제휴포인트 etc : 기타 |
| 13 | 결제수단명 | `payment_method_name` | 결제수단명 주문자가 이용한 결제수단의 이름 |
| 14 | PG 이름 | `payment_gateway_names` | PG 이름 |
| 15 | 해외 결제수단명 | `sub_payment_method_name` | 해외 결제수단명 |
| 16 | 해외 결제수단코드 | `sub_payment_method_code` | 해외 결제수단코드 sub_payment_method_code |
| 17 | 카드 거래 아이디 | `transaction_ids` | 카드 거래 아이디 |
| 18 | 결제 여부 | `paid` | 결제 여부 결제가 완료되었는지 여부 T : 결제 F : 미결제 M : 부분 결제 |
| 19 | 취소 여부 | `canceled` | 취소 여부 T : 취소 F : 미취소 M : 부분 취소 |
| 20 | 주문일 | `order_date` | 주문일 |
| 21 | 최초 주문여부 | `first_order` | 최초 주문여부 해당 주문이 최초 주문인지 여부 T : 최초 주문 F : 최초 주문 아님 |
| 22 | 결제일 | `payment_date` | 결제일 |
| 23 | 모바일 구분 | `order_from_mobile` | 모바일 구분 주문이 모바일에서 이루어졌는지 여부 T : 모바일 주문 F : 모바일 주문 아님 |
| 24 | 에스크로 사용여부 | `use_escrow` | 에스크로 사용여부 에스크로를 사용했는지 여부 T : 에스크로 사용 F : 에스크로 미사용 |
| 25 | 주문시 회원등급 | `group_no_when_ordering` | 주문시 회원등급 |
| 26 | 최초 주문 금액 | `initial_order_amount` | 최초 주문 금액 |
| 27 | 현재 주문 금액 | `actual_order_amount` | 현재 주문 금액 실결제금액 중 coupon_shipping_fee_amount는 할인 금액 자동 계산을 사용할 때만 품목별로 배송비 배분이 가능하기 때문에 할인 금액 자동 계산 기능을 사용할 때만 노출됨 |
| 28 | 계좌번호 | `bank_account_no` | 계좌번호 해당 주문건에 대한 쇼핑몰의 계좌번호 |
| 29 | 예금주 | `bank_account_owner_name` | 예금주 |
| 30 | 마켓 판매자 아이디 | `market_seller_id` | 마켓 판매자 아이디 |
| 31 | 최종 결제 금액 | `payment_amount` | 최종 결제 금액 |
| 32 | 주문취소일 | `cancel_date` | 주문취소일 |
| 33 | 주문경로 텍스트 | `order_place_name` | 주문경로 텍스트 |
| 34 | 주문경로 | `order_place_id` | 주문경로 |
| 35 | 후불결제 입금확인 가능 여부 | `payment_confirmation` | 후불결제 입금확인 가능 여부 T : 입금확인 F : 입금미확인 |
| 36 | 결제 수수료 | `commission` | 결제 수수료 |
| 37 | 후불결제여부 | `postpay` | 후불결제여부 T : 후불결제 F : 후불결제 아님 |
| 38 | 관리자 입력 금액 | `admin_additional_amount` | 관리자 입력 금액 |
| 39 | 추가 배송비 | `additional_shipping_fee` | 추가 배송비 |
| 40 | 해외배송 보험료 | `international_shipping_insurance` | 해외배송 보험료 |
| 41 | 해외배송 부가금액 | `additional_handling_fee` | 해외배송 부가금액 |
| 42 | 배송 유형 | `shipping_type` | 배송 유형 배송 유형. 국내배송인지 해외배송인지 여부 A : 국내 B : 해외 |
| 43 | 배송 유형명 | `shipping_type_text` | 배송 유형명 배송 유형. 국내배송인지 해외배송인지 여부 |
| 44 | 배송상태 | `shipping_status` | 배송상태 F : 배송전 M : 배송중 T : 배송완료 W : 배송보류 X : 발주전 |
| 45 | 희망배송일 | `wished_delivery_date` | 희망배송일 |
| 46 | 희망배송시간 | `wished_delivery_time` | 희망배송시간 |
| 47 | 희망배송사 코드 | `wished_carrier_id` | 희망배송사 코드 |
| 48 | 희망배송사 명 | `wished_carrier_name` | 희망배송사 명 |
| 49 | 반품승인일시 | `return_confirmed_date` | 반품승인일시 |
| 50 | 총 공급가액 | `total_supply_price` | 총 공급가액 |
| 51 | 네이버포인트 | `naver_point` | 네이버포인트 |
| 52 | 주문서 추가항목 | `additional_order_info_list` | 주문서 추가항목 |
| 53 | 매장수령여부 | `store_pickup` | 매장수령여부 T : 매장수령 F : 매장수령 아님 |
| 54 | 간편결제 결제사 이름 | `easypay_name` | 간편결제 결제사 이름 |
| 55 | 여신상태 | `loan_status` | 여신상태 OK : GOOD NG : NOT GOOD ER : ERROR |
| 56 | 정기결제 여부 | `subscription` | 정기결제 여부 T : 정기결제 F : 정기결제 아님 |
| 57 | 품주 리소스 | `items` | 품주 리소스 조회시 Embed 파라메터를 사용하여 조회할 수 있다. |
| 58 | 수령자정보 리소스 | `receivers` | 수령자정보 리소스 조회시 Embed 파라메터를 사용하여 조회할 수 있다. |
| 59 | 주문자정보 리소스 | `buyer` | 주문자정보 리소스 |
| 60 | 배송비 정보 | `shipping_fee_detail` | 배송비 정보 |
| 61 | 지역별 배송비 정보 | `regional_surcharge_detail` | 지역별 배송비 정보 |
| 62 | 반품상세 리소스 | `return` | 반품상세 리소스 |
| 63 | 취소상세 리소스 | `cancellation` | 취소상세 리소스 |
| 64 | 교환상세 리소스 | `exchange` | 교환상세 리소스 |
| 65 | 멀티 배송지 여부 | `multiple_addresses` | 멀티 배송지 여부 T : 멀티 배송지 주문 F : 멀티 배송지 주문 아님 |
| 66 | 결제 화폐 환율 정보 | `exchange_rate` | 결제 화폐 환율 정보 |
| 67 | 최초 결제수단 코드 | `first_payment_methods` | 최초 결제수단 코드 cash : 무통장 card : 신용카드 cell : 휴대폰 tcash : 계좌이체 icash : 가상계좌 prepaid : 선불금 credit : 예치금 point : 적립금 pointfy : 통합포인트 cvs : 편의점 cod : 후불 giftcard : 제휴상품권 pointcard : 제휴포인트 etc : 기타 |
| 68 | 네이버페이 PG 결제 정보 | `naverpay_payment_information` | 네이버페이 PG 결제 정보 P : PG결제 N : 네이버결제 |
| 69 | 가격에 세금 포함 | `include_tax` | 가격에 세금 포함 T: 세금포함 F: 세금제외 |
| 70 | 세금 상세 정보 | `tax_detail` | 세금 상세 정보 |
| 71 | 주문 서비스 유형 | `service_type` | 주문 서비스 유형 rental : 렌탈주문 |
| 72 | 주문 서비스 데이터 | `service_data` | 주문 서비스 데이터 |
| 73 | 배송지 정보 표기 여부 | `show_shipping_address` | 배송지 정보 표기 여부 T: 배송지 정보 표기 F: 배송지 정보 가림 |
| 74 | 연동 된 SNS 제공코드 | `social_member_code` | 연동 된 SNS 제공코드 |
| 75 | 연동 된 SNS명 | `social_name` | 연동 된 SNS명 |
| 76 | 주문시 회원등급 | `customer_group_no_when_ordering` | 주문시 회원등급 주문 당시의 회원등급 |
| 77 | 혜택 리소스 | `benefits` | 혜택 리소스 |
| 78 | 쿠폰 리소스 | `coupons` | 쿠폰 리소스 |
| 79 | 환불상세 리소스 | `refunds` | 환불상세 리소스 |
| 80 | 주문상태 | `process_status` | 주문상태 prepare : 배송준비중 prepareproduct : 상품준비중 hold : 배송보류 unhold : 배송보류해제 |
| 81 | 품주코드 | `order_item_code` | 품주코드 |
| 82 | 구매확정 여부 | `purchase_confirmation` | 구매확정 여부 |
| 83 | 적립금 회수 | `collect_points` | 적립금 회수 |

