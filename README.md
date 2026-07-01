# Messente (messente)

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
