# Contentsquare (contentsquare)

Contentsquare is a digital experience analytics platform that captures every user interaction on web and mobile properties to surface friction points, conversion blockers, and behavioral insights via session replay, heatmaps, journey analysis, and zone-based analytics. The platform helps product, marketing, and UX teams optimize digital experiences with AI-driven recommendations. Contentsquare offers Data Export and Enrichment REST APIs authenticated via OAuth 2.0 client credentials with dynamic regional base URLs returned at authentication time.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/contentsquare/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Digital Experience Analytics
- Product Analytics
- Session Replay
- Heatmaps
- Customer Experience
- Conversion Optimization
- User Behavior

## Timestamps

- **Created:** 2026-05-11
- **Modified:** 2026-05-11

## APIs

### Contentsquare Data Export API

REST API for exporting Contentsquare metrics and raw analytics data. Authentication uses OAuth 2.0 client_credentials flow against https://api.contentsquare.com/v1/oauth/token, which returns a JWT access token valid for one hour plus a dynamic regional base URL (for example https://api.eu-west-1.production.contentsquare.com).

- **Human URL:** [https://docs.contentsquare.com/en/api/export/](https://docs.contentsquare.com/en/api/export/)
- **Base URL:** `https://api.eu-west-1.production.contentsquare.com`

#### Tags

- Digital Experience Analytics
- Data Export
- Metrics
- OAuth

#### Properties

- [Documentation](https://docs.contentsquare.com/en/api/export/)
- [Authentication](https://docs.contentsquare.com/en/api/export/authentication/)
- [Postman Collection](collections/contentsquare.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contentsquare.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Contentsquare Enrichment API

REST API for sending enrichment data batches into Contentsquare, enabling teams to merge first-party data with captured session data. Uses the same OAuth 2.0 client credentials authentication and dynamic regional base URLs as the Data Export API.

- **Human URL:** [https://docs.contentsquare.com/en/api/enrichment/](https://docs.contentsquare.com/en/api/enrichment/)
- **Base URL:** `https://enrichment-api.eu-west-1.production.contentsquare.com`

#### Tags

- Digital Experience Analytics
- Data Enrichment
- OAuth

#### Properties

- [Documentation](https://docs.contentsquare.com/en/api/enrichment/)
- [Sending  Batches](https://docs.contentsquare.com/en/api/enrichment/sending-enrichment-data-batches-cs/)
- [Postman Collection](collections/contentsquare.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/contentsquare.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/contentsquare)
- [LinkedIn](https://www.linkedin.com/company/contentsquare)
- [Website](https://contentsquare.com)
- [Documentation](https://docs.contentsquare.com/en/)
- [Pricing](https://contentsquare.com/pricing/)
- [Sign Up](https://contentsquare.com/request-demo/)
- [L L Ms Txt](https://docs.contentsquare.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
