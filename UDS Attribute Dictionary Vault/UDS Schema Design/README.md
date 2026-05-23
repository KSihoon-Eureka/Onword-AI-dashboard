# UDS Schema Design

MVP Unified Data Structure design for retail/ecommerce ERP dashboard ingestion.

## Outputs

- [UDS Core Schema](./UDS-Core-Schema.md) — human-readable relational MVP schema.
- [Channel Mapping CSV](./UDS-Channel-Mapping.csv) — one row per included channel, UDS attributes as columns.
- [Channel Mapping Markdown](./UDS-Channel-Mapping.md) — readable mapping explanation split by category.
- [Machine-readable JSON Schema](./uds_core_schema.json) — tables, fields, labels, DB columns, types, priority, descriptions.
- [Implementation Spec](./Implementation-Spec.md) — DB design, keys, upserts, raw payload strategy, normalization rules.
- [Future Channel Research](./Future-Channel-Research.md) — research summary for phase-2 channels.
- [Future channel notes](./future-channels/) — detailed notes only for channels with official/credible API details.

## Scope

Included in MVP mapping: Coupang, Cafe24, Naver Smart Store, Gmarket/Auction, SSG Mall.

Excluded from MVP mapping: 11st, LotteON, KakaoTalk Gift/Kakao Shopping, CJ OnStyle, GS SHOP, Kurly, Zigzag. These are captured as future-channel research only.

## Attribute count

The MVP schema contains **79 UDS attributes** across 9 relational tables/categories.
