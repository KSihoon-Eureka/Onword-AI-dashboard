# Gmarket/Auction ESM UDS Attribute Dictionary

접근권한 리서치 결론: Gmarket/Auction ESM Trading API는 일반적인 “클라이언트 API 키만 받아서 바로 연결” 모델이 아닙니다. 셀링툴사는 자사 사업자 기준으로 G마켓/옥션 판매자 회원 가입 + ESM+ 마스터 ID 생성이 필요하고, API 범위/ESM 마스터 ID/서비스 URL/최근 3개월 매출/API 개발기간/셀링툴 소개자료/현재 이용 중인 G마켓·옥션 판매자 수를 포함해 etapihelp@gmail.com으로 사용 신청해야 합니다. 승인은 내부 리소스와 안정성 기준에 따라 거절될 수 있습니다. 인증 JWT의 kid도 “셀링툴사의 ESM+ 마스터 ID”를 넣으라고 명시되어 있어, 우리 SaaS도 별도 접근승인을 받아야 한다고 보는 것이 맞습니다.

## Universal Total Table — 전체 Gmarket/Auction 고유 UDS 속성

자동 추출 기준: ESM Trading API sitemap 196개 문서 / 원본 필드 occurrence 4044개 / 의미 기준 UDS 속성 2114개. UDS 필요도: ✅ 핵심 UDS=1732개, 🟡 후보=34개. 요청대로 Universal Total Table만 생성했습니다.
