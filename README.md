# PDFMonkey (pdfmonkey)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

PDFMonkey is a document generation service that turns HTML + Liquid templates and a JSON data payload into PDF (or image) documents via a REST API. Templates are designed in a dashboard editor and generated on demand, asynchronously or synchronously, with webhooks and signed download URLs for delivery.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pdfmonkey/refs/heads/main/apis.yml)

## Tags

- PDF
- Document Generation
- Templates
- HTML to PDF
- Documents

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### PDFMonkey Documents API

Create, retrieve, update, and delete documents. A document is generated from a template plus a JSON payload, asynchronously by setting status to pending, or synchronously via the documents/sync endpoint, returning signed download URLs.

- **Human URL:** [https://docs.pdfmonkey.io/references/api/documents](https://docs.pdfmonkey.io/references/api/documents)
- **Base URL:** `https://api.pdfmonkey.io/api/v1`

#### Tags

- Documents
- PDF
- Generation

#### Properties

- [Documentation](https://docs.pdfmonkey.io/references/api/documents)
- [API Reference](https://docs.pdfmonkey.io/references/api)
- [OpenAPI](openapi/pdfmonkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfmonkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfmonkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PDFMonkey Document Cards API

Lightweight, paginated document representations that omit the heavy payload attribute. Used to poll generation status and retrieve download URLs efficiently, and to list documents with filtering by template, status, workspace, and update time.

- **Human URL:** [https://docs.pdfmonkey.io/references/api/documents](https://docs.pdfmonkey.io/references/api/documents)
- **Base URL:** `https://api.pdfmonkey.io/api/v1`

#### Tags

- Document Cards
- Status
- Listing

#### Properties

- [Documentation](https://docs.pdfmonkey.io/references/api/documents)
- [OpenAPI](openapi/pdfmonkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfmonkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfmonkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PDFMonkey Templates API

List, retrieve, create, update, and delete document templates. Templates hold published and draft HTML + Liquid bodies, SCSS styles, sample data, and printing settings. Lightweight document template cards support paginated listing.

- **Human URL:** [https://docs.pdfmonkey.io/references/api/templates](https://docs.pdfmonkey.io/references/api/templates)
- **Base URL:** `https://api.pdfmonkey.io/api/v1`

#### Tags

- Templates
- HTML
- Liquid

#### Properties

- [Documentation](https://docs.pdfmonkey.io/references/api/templates)
- [OpenAPI](openapi/pdfmonkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/pdfmonkey.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/pdfmonkey.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PDFMonkey Webhooks

Real-time notifications fired on documents.generation.success and documents.generation.failure. The webhook delivers a DocumentCard payload (no dynamic payload, logs, or checksum); use the meta field on creation to pass data through to handlers.

- **Human URL:** [https://docs.pdfmonkey.io/pdfmonkey-features/webhooks](https://docs.pdfmonkey.io/pdfmonkey-features/webhooks)
- **Base URL:** `https://api.pdfmonkey.io/api/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.pdfmonkey.io/pdfmonkey-features/webhooks)
- [OpenAPI](openapi/pdfmonkey-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/pdfmonkey)
- [LinkedIn](https://www.linkedin.com/company/pdfmonkey)
- [Website](https://www.pdfmonkey.io)
- [Documentation](https://docs.pdfmonkey.io)
- [Plans](plans/pdfmonkey-plans-pricing.yml)
- [Rate Limits](rate-limits/pdfmonkey-rate-limits.yml)
- [Fin Ops](finops/pdfmonkey-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
