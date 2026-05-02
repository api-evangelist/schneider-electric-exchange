# Schneider Electric Exchange

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
