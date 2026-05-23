# UDS Core Schema — MVP ERP/Dashboard
- MVP 속성 수: **79개**
- 범위: 주문/주문상품/배송/클레임/상품/재고/정산/고객·수령자/CS
- 비즈니스 라벨은 한국어, DB 컬럼은 English `snake_case`입니다.
- 채널 매핑 대상은 Coupang, Cafe24, Naver Smart Store, Gmarket/Auction, SSG Mall 5개로 제한합니다.

## 주문 — `orders`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 채널 | `channel` | text | 판매 채널 식별자 |
| 1 | core_required | 채널 주문 ID | `channel_order_id` | text | 채널 원주문/주문번호 |
| 1 | core_required | 주문일시 | `ordered_at` | datetime | 고객이 주문을 생성한 시각 |
| 1 | recommended | 결제일시 | `paid_at` | datetime | 결제 완료 시각 |
| 1 | core_required | 주문 상태 | `order_status` | text | 채널 주문 단위 상태 |
| 2 | recommended | 결제 수단 | `payment_method` | text | 카드/간편결제/무통장 등 결제 수단 |
| 2 | recommended | 통화 | `currency_code` | text | 거래 통화 코드 |
| 1 | core_required | 주문 금액 | `order_amount` | numeric | 주문 단위 총 상품/주문 금액 |
| 2 | recommended | 할인 금액 | `discount_amount` | numeric | 채널/쿠폰/판매자 할인 합계 |
| 1 | core_required | 결제 금액 | `paid_amount` | numeric | 실제 결제 금액 |
| 2 | recommended | 판매자 ID | `seller_id` | text | 채널 판매자/벤더/몰 식별자 |
| 1 | core_required | 원본 수집 시각 | `source_collected_at` | datetime | 원천 API/파일 수집 시각 |

## 주문상품 — `order_items`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 채널 주문상품 ID | `channel_order_item_id` | text | 채널의 상품주문/주문상세/품목 식별자 |
| 1 | core_required | 상품 ID | `channel_product_id` | text | 채널 상품번호 |
| 2 | recommended | 옵션 ID | `channel_option_id` | text | 채널 옵션/SKU 식별자 |
| 1 | core_required | 상품명 | `product_name` | text | 주문 시점 상품명 |
| 2 | recommended | 옵션명 | `option_name` | text | 주문 옵션명/옵션 조합 |
| 2 | recommended | 판매자 SKU | `seller_sku` | text | 판매자 관리 SKU/자체상품코드 |
| 1 | core_required | 수량 | `quantity` | integer | 주문/판매 수량 |
| 1 | core_required | 판매 단가 | `unit_price` | numeric | 품목 단위 판매가 |
| 1 | core_required | 품목 총액 | `item_amount` | numeric | 수량 반영 품목 총액 |
| 2 | recommended | 품목 할인액 | `item_discount_amount` | numeric | 품목에 배부된 할인액 |
| 1 | core_required | 품목 상태 | `item_status` | text | 상품주문/품목 처리 상태 |
| 2 | recommended | 발주확인일시 | `order_confirmed_at` | datetime | 판매자 발주/주문 확인 시각 |
| 2 | recommended | 구매확정일시 | `purchase_confirmed_at` | datetime | 구매확정/정산 기준 시각 |
| 3 | phase_2 | 세금 포함 여부 | `tax_included` | boolean | 가격에 세금 포함 여부 |
| 3 | phase_2 | 과세 금액 | `taxable_amount` | numeric | 부가세 과세 대상 금액 |
| 3 | phase_2 | 상품 유형 | `product_type` | text | 일반/배송/여행/e쿠폰 등 상품 유형 |
| 3 | phase_2 | 클레임 가능 여부 | `claimable` | boolean | 취소/반품/교환 가능 여부 |
| 1 | core_required | 행 해시 | `row_hash` | text | 정규화 행 변경 감지용 해시 |

## 배송 — `shipments`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 배송 ID | `channel_shipment_id` | text | 배송/출고/박스 식별자 |
| 2 | recommended | 택배사 코드 | `carrier_code` | text | 택배사 코드 |
| 2 | recommended | 택배사명 | `carrier_name` | text | 택배사명 |
| 1 | core_required | 운송장 번호 | `tracking_number` | text | 송장/추적 번호 |
| 1 | core_required | 배송 상태 | `shipment_status` | text | 출고/배송 진행 상태 |
| 2 | recommended | 배송비 | `shipping_fee` | numeric | 고객/판매자 배송비 |
| 2 | recommended | 배송 메시지 | `shipping_message` | text | 고객 배송 요청사항 |
| 2 | recommended | 출고 예정일 | `expected_ship_at` | datetime | 출고/발송 예정 시각 |
| 2 | recommended | 출고일시 | `shipped_at` | datetime | 판매자가 발송 처리한 시각 |
| 3 | phase_2 | 배송완료일시 | `delivered_at` | datetime | 배송완료 시각 |

## 클레임 — `claims`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 클레임 ID | `channel_claim_id` | text | 취소/반품/교환 클레임 식별자 |
| 1 | core_required | 클레임 유형 | `claim_type` | text | 취소/반품/교환/환불 유형 |
| 1 | core_required | 클레임 상태 | `claim_status` | text | 클레임 처리 상태 |
| 2 | recommended | 클레임 사유 코드 | `claim_reason_code` | text | 채널 클레임 사유 코드 |
| 2 | recommended | 클레임 사유 | `claim_reason` | text | 고객/관리자 클레임 사유 |
| 2 | recommended | 클레임 수량 | `claim_quantity` | integer | 취소/반품/교환 수량 |
| 2 | recommended | 클레임 접수일시 | `claim_requested_at` | datetime | 클레임 요청/접수 시각 |
| 2 | recommended | 환불 금액 | `refund_amount` | numeric | 환불/차감 금액 |

## 상품 — `products`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 마스터 상품 ID | `product_id` | text | 내부/UDS 상품 식별자 |
| 1 | core_required | 채널 상품 ID | `channel_product_id` | text | 채널 상품 식별자 |
| 1 | core_required | 상품명 | `product_name` | text | 현재 채널 상품명 |
| 2 | recommended | 브랜드명 | `brand_name` | text | 브랜드/제조사명 |
| 2 | recommended | 카테고리 ID | `category_id` | text | 채널 카테고리 식별자 |
| 2 | recommended | 카테고리명 | `category_name` | text | 채널 카테고리명 |
| 1 | core_required | 판매상태 | `product_status` | text | 판매중/품절/중지 등 상태 |
| 2 | recommended | 등록/수정일시 | `product_updated_at` | datetime | 상품 마지막 수정 시각 |

## 재고 — `inventory_snapshots`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 재고 스냅샷 ID | `inventory_snapshot_id` | text | 스냅샷 행 식별자 |
| 1 | core_required | 가용 재고 수량 | `available_quantity` | integer | 판매 가능한 재고 |
| 2 | recommended | 안전 재고 수량 | `safety_quantity` | integer | 안전재고/최소재고 |
| 2 | recommended | 재고 관리 여부 | `inventory_managed` | boolean | 재고 차감/관리 사용 여부 |
| 1 | core_required | 스냅샷 시각 | `snapshot_at` | datetime | 재고 값을 관측한 시각 |

## 정산 — `settlements`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 정산 ID | `channel_settlement_id` | text | 채널 정산 식별자 |
| 1 | core_required | 정산 기준일 | `settlement_date` | date | 정산/매출 기준일 |
| 2 | recommended | 정산 상태 | `settlement_status` | text | 예정/확정/보류 등 정산 상태 |
| 1 | core_required | 정산 대상 금액 | `settlement_gross_amount` | numeric | 매출/정산 대상 총액 |
| 2 | recommended | 수수료 금액 | `commission_amount` | numeric | 판매/결제/채널 수수료 |
| 1 | core_required | 정산 지급 금액 | `settlement_net_amount` | numeric | 차감 후 지급 예상/확정 금액 |

## 고객/수령자 — `customers_receivers`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 2 | recommended | 구매자 ID | `buyer_id` | text | 채널 구매자 식별자 |
| 2 | recommended | 구매자명 | `buyer_name` | text | 구매자명 |
| 2 | recommended | 구매자 연락처 | `buyer_phone` | text | 구매자 전화번호/휴대폰 |
| 1 | core_required | 수령자명 | `receiver_name` | text | 배송 수령자명 |
| 1 | core_required | 수령자 연락처 | `receiver_phone` | text | 수령자 전화번호/휴대폰 |
| 2 | recommended | 우편번호 | `receiver_zipcode` | text | 배송지 우편번호 |
| 2 | recommended | 주소 | `receiver_address` | text | 배송지 주소 |

## CS — `cs_threads`
| 우선순위 | 필요도 | 한국어 라벨 | DB 컬럼 | 타입 | 설명 |
|---:|---|---|---|---|---|
| 1 | core_required | 문의 ID | `channel_cs_id` | text | 상품문의/고객문의/쪽지 식별자 |
| 2 | recommended | 문의 유형 | `cs_type` | text | 상품 Q&A, 배송 문의, 클레임 문의 등 |
| 2 | recommended | 문의 제목 | `cs_subject` | text | 문의 제목 |
| 2 | recommended | 문의 내용 | `cs_content` | text | 문의/메시지 본문 |
| 2 | recommended | 답변 상태 | `cs_answer_status` | text | 미답변/답변완료 상태 |
