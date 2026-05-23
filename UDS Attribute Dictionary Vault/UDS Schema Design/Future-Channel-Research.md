# Future Channel Research

Future channels researched for later connector work. They are **not** included in `UDS-Channel-Mapping.csv` because the MVP mapping is limited to the five already-extracted dictionaries.

## Summary

| Channel | Public/API availability | MVP recommendation |
|---|---|---|
| 11st | Official OpenAPI has order-service entry points, but detailed order docs/API use are seller/API-registration gated. | Keep as phase-2 API connector candidate; confirm seller OpenAPI key and order endpoint details before extraction. |
| LotteON | Official OpenAPI is available for sellers/partners; delivery/order-search endpoint details are publicly referenced. | Phase-2 API connector candidate after key/IP setup. |
| KakaoTalk Gift / Kakao Shopping | Kakao Shopping Open API exists; Gift channel access is permissioned/pre-approved. | Phase-2 if Barudak has Gift API permission; otherwise portal/MD-assisted onboarding. |
| CJ OnStyle | Standard API docs are publicly accessible enough to identify delivery/order endpoints and auth headers. | Phase-2 API connector candidate after vendor code/authentication key/IP allowlist. |
| GS SHOP | Partner portal shows API concept, but public order API docs were not found. | Do not create connector until partner docs/credentials are obtained; prepare portal/Excel fallback. |
| Kurly | No public seller order API docs found. | Treat as portal/EDI/Excel fallback until partner account inspection. |
| Zigzag | No public seller order API docs found. | Treat as partner-center export/internal-XHR fallback until seller account inspection. |

## Notes saved

Detailed notes are saved only where official or credible API details were available:

- `future-channels/11st.md`
- `future-channels/LotteON.md`
- `future-channels/Kakao-Shopping-Gift.md`
- `future-channels/CJ-OnStyle.md`

No detailed note was created for GS SHOP, Kurly, or Zigzag because no API-usable public documentation was found in this pass.

## Caveat

Several Korean marketplace APIs are permissioned, seller-login-gated, or require MD/partner approval. Treat this research as connector triage, not a substitute for credentialed API validation.
