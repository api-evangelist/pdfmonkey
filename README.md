# PDFMonkey (pdfmonkey)

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
