# Kakao Shopping / KakaoTalk Gift Future Channel API Note

## Status

Kakao Shopping Open API exists. KakaoTalk Gift (`선물하기`) access is permissioned and must be granted to approved sellers.

## Known details

- Order list API family includes `/v2/shopping/orders` for modified-time order search.
- Auth pattern uses Kakao app/admin keys, including headers such as:
  - `Authorization: KakaoAK {admin_app_key}`
  - `Target-Authorization: KakaoAK {seller_app_key}`
  - `channel-ids: 1` for 선물하기; `101` for 톡스토어.

## Connector implications

- Feasible only if Barudak has Kakao Gift API permission.
- Modified-time polling is suitable for incremental sync if access is granted.
- Confirm claim, shipping, settlement, and CS endpoint coverage before schema extension.
