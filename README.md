# Schneider Electric Exchange

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

Schneider Electric Exchange is a developer platform providing APIs for EcoStruxure energy management, building automation, industrial IoT, and B2B partner commerce integrations. The Exchange platform enables distributors, system integrators, and developers to build applications with Schneider Electric's EcoStruxure platform and partner commerce ecosystem.

**Portal:** [https://exchange.se.com/develop](https://exchange.se.com/develop)

## EcoStruxure APIs

| API | Description |
|---|---|
| [EcoStruxure IT Expert API](https://community.se.com/t5/EcoStruxure-IT-Expert-API/tkb-p/ecostruxure-it-expert-api) | Data center infrastructure monitoring (devices, alarms, sensors) |
| [EcoStruxure Facility Expert Data API](https://shop.exchange.se.com/en-US/apps/76237/ecostruxure-facility-expert-data-api) | Building management time series and alarms |
| [EcoStruxure Energy Contextualized Data API](https://exchange.se.com/develop/products/ecostruxure-energy-contextualized-data-api) | Contextualized energy consumption data |
| [EcoStruxure Transformer Expert Data API](https://exchange.se.com/develop/products/684854/ecostruxure-transformer-expert-data-api) | Transformer health analytics and monitoring |

## Partner Commerce APIs

| API | Description |
|---|---|
| [Product Catalog](https://api-explorer.se.com/en/api/product-catalog-v2) | Technical product data with ETIM 10.0 classification |
| [Product Availability](https://api-explorer.se.com/en/api/product-availability-v2) | Delivery lead times by product and address |
| Net Price | List and partner net pricing by account |
| [Order Status](https://api-explorer.se.com/en/api/distributor-order-status-v1.0) | Order status and shipment tracking |
| [Distributor Quote](https://api-explorer.se.com/en/api/distributor-quote-v1) | Quote lines for distributor accounts |
| [Installed Product](https://api-explorer.se.com/en/api/Partner-Installed-Product-v1.0) | Warranty dates by serial number |
| [Digital Assets](https://api-explorer.se.com/en/api/product-digital-asset-v1) | Product images, 3D models, datasheets |

## Authentication

- **EcoStruxure APIs** — Subscription key (`Ocp-Apim-Subscription-Key` header), requires active EcoStruxure product subscription
- **Partner Commerce APIs** — OAuth 2.0 Client Credentials; client ID and secret obtained from local Schneider Electric contact

## Artifacts

### JSON Schema

- [ecostruxure-it-device-schema.json](json-schema/ecostruxure-it-device-schema.json) — EcoStruxure IT device resource schema
- [partner-product-schema.json](json-schema/partner-product-schema.json) — Partner product catalog schema

### JSON Structure

- [schneider-electric-exchange-api-structure.json](json-structure/schneider-electric-exchange-api-structure.json) — API platform structure

### JSON-LD

- [schneider-electric-exchange-context.jsonld](json-ld/schneider-electric-exchange-context.jsonld) — Linked data context for EcoStruxure vocabulary

### Examples

- [ecostruxure-it-get-devices-example.json](examples/ecostruxure-it-get-devices-example.json) — List devices from EcoStruxure IT Expert
- [partner-get-product-availability-example.json](examples/partner-get-product-availability-example.json) — Check product availability

### Vocabulary

- [schneider-electric-exchange-vocabulary.yml](vocabulary/schneider-electric-exchange-vocabulary.yml) — Domain vocabulary for EcoStruxure and partner APIs

## Maintainers

**Kin Lane** — kin@apievangelist.com
