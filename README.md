# Messente (messente)

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

Messente is an Estonian CPaaS provider of global messaging and user verification services. A single Omnimessage endpoint sends SMS, Viber, WhatsApp, and Telegram with an automatic fallback chain, backed by contacts and groups in the Phonebook, phone number (HLR) lookup, PIN-based number verification / 2FA, delivery reports, and messaging statistics over an HTTP Basic authenticated REST API at api.messente.com/v1.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/messente/refs/heads/main/apis.yml)

## Tags

- CPaaS
- Messaging
- SMS
- Viber
- WhatsApp
- Verification
- 2FA

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Messente Omnimessage API

The unified Omnimessage endpoint sends a message across SMS, Viber, WhatsApp, and Telegram as an ordered fallback chain, attempting each channel in priority order until delivery succeeds, and supports cancelling scheduled messages.

- **Human URL:** [https://messente.com/documentation/omnichannel-api](https://messente.com/documentation/omnichannel-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Omnimessage
- Messaging
- Fallback

#### Properties

- [Documentation](https://messente.com/documentation/omnichannel-api)
- [API Reference](https://messente.com/documentation)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente SMS API

Global SMS delivery via the Omnimessage endpoint with sender ID, GSM/Unicode autoconvert, validity periods, and bulk sending to many recipients in a single request.

- **Human URL:** [https://messente.com/documentation/omnichannel-api](https://messente.com/documentation/omnichannel-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- SMS
- Text Messaging
- Bulk

#### Properties

- [Documentation](https://messente.com/documentation/omnichannel-api)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente Contacts API

Create, read, update, and delete contacts in the Messente Phonebook under /phonebook/contacts, manage their group memberships, and maintain a phone number blacklist to suppress unwanted messages.

- **Human URL:** [https://messente.com/documentation/phonebook-api](https://messente.com/documentation/phonebook-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Contacts
- Phonebook
- CRM

#### Properties

- [Documentation](https://messente.com/documentation/phonebook-api)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente Groups API

Manage contact groups under /phonebook/groups for segmentation and targeted bulk messaging, including creating, updating, listing, and deleting groups and adding or removing contacts from them.

- **Human URL:** [https://messente.com/documentation/phonebook-api](https://messente.com/documentation/phonebook-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Groups
- Phonebook
- Segmentation

#### Properties

- [Documentation](https://messente.com/documentation/phonebook-api)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente Number Lookup API

Synchronous HLR lookup at /hlr/sync returns network, roaming, and portability information for phone numbers, plus PIN-based number verification (2FA) at /verify/start and /verify/pin for confirming a user controls a number.

- **Human URL:** [https://messente.com/documentation/phone-number-lookup-api](https://messente.com/documentation/phone-number-lookup-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Number Lookup
- HLR
- Number Verification

#### Properties

- [Documentation](https://messente.com/documentation/phone-number-lookup-api)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente Statistics API

Request messaging statistics reports by country and destination network (MCC/MNC) over a date range at /statistics/reports, reporting sent, delivered, and failed message counts.

- **Human URL:** [https://messente.com/documentation/statistics-api](https://messente.com/documentation/statistics-api)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Statistics
- Reporting
- Analytics

#### Properties

- [Documentation](https://messente.com/documentation/statistics-api)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Messente Delivery Reports API

Retrieve per-channel delivery status for a sent Omnimessage at /omnimessage/{omnimessageId}/status, or receive asynchronous status pushes to a configured delivery report callback (webhook) URL.

- **Human URL:** [https://messente.com/documentation/omnichannel-api/delivery-report](https://messente.com/documentation/omnichannel-api/delivery-report)
- **Base URL:** `https://api.messente.com/v1`

#### Tags

- Delivery Reports
- Webhooks
- Status

#### Properties

- [Documentation](https://messente.com/documentation/omnichannel-api/delivery-report)
- [OpenAPI](openapi/messente-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/messente.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/messente.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/messente)
- [LinkedIn](https://www.linkedin.com/company/messente)
- [Website](https://messente.com/)
- [Documentation](https://messente.com/documentation)
- [Plans](plans/messente-plans-pricing.yml)
- [Rate Limits](rate-limits/messente-rate-limits.yml)
- [Fin Ops](finops/messente-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
