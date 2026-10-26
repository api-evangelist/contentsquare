# Contentsquare (contentsquare)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
