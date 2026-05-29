# positionstack

Forward and Reverse Batch Geocoding REST API by **positionstack** (an apilayer product, owned by Idera, Inc.). Convert addresses to coordinates and coordinates to addresses across 2+ billion global places, with optional enrichment modules for country, timezone, sun, and bounding box.

- **Website:** https://positionstack.com/
- **Documentation:** https://docs.apilayer.com/positionstack/docs/api-documentation
- **Status:** https://positionstack.com/api-status
- **GitHub:** https://github.com/apilayer/positionstack (archived reference repo)
- **APIs.yml:** [apis.yml](apis.yml)

## Type

- **x-type:** company
- **x-tier:** 3 (bulk-registered from public-apis, enriched 2026-05-29)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) - category: Geocoding

## APIs

### positionstack Geocoding API

REST API providing forward geocoding (address to coordinates), reverse geocoding (coordinates to address), and batch lookups with optional enrichment modules.

- **Base URL:** `https://api.positionstack.com/v1`
- **Auth:** `access_key` query parameter
- **Endpoints:** `GET /forward`, `GET /reverse`
- **Output formats:** JSON, XML, GeoJSON

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [openapi/positionstack-openapi.yml](openapi/positionstack-openapi.yml) |
| JSON Schema (Location) | [json-schema/positionstack-location-schema.json](json-schema/positionstack-location-schema.json) |
| JSON Schema (Error) | [json-schema/positionstack-error-schema.json](json-schema/positionstack-error-schema.json) |
| JSON Structure | [json-structure/positionstack-location-structure.json](json-structure/positionstack-location-structure.json) |
| JSON-LD Context | [json-ld/positionstack-context.jsonld](json-ld/positionstack-context.jsonld) |
| Spectral Rules | [rules/positionstack-rules.yml](rules/positionstack-rules.yml) |
| Vocabulary | [vocabulary/positionstack-vocabulary.yml](vocabulary/positionstack-vocabulary.yml) |
| Plans / Pricing | [plans/positionstack-plans-pricing.yml](plans/positionstack-plans-pricing.yml) |
| Rate Limits | [rate-limits/positionstack-rate-limits.yml](rate-limits/positionstack-rate-limits.yml) |
| FinOps | [finops/positionstack-finops.yml](finops/positionstack-finops.yml) |

### Examples

- [Forward geocode](examples/positionstack-forward-geocode-example.json)
- [Reverse geocode](examples/positionstack-reverse-geocode-example.json)
- [Batch forward](examples/positionstack-batch-forward-example.json)
- [Error envelope](examples/positionstack-error-example.json)

### Capabilities

- [Shared geocoding capability](capabilities/shared/positionstack-geocoding.yaml)
- [Address to coordinates](capabilities/address-to-coordinates.yaml)
- [Coordinates to address](capabilities/coordinates-to-address.yaml)
- [Bulk address cleansing](capabilities/bulk-address-cleansing.yaml)

## Plans

| Plan | Monthly | Yearly (eff. /mo) | Requests/mo | Overage |
|---|---|---|---|---|
| Free | $0 | - | 100 | n/a |
| Basic | $9.99 | $8.99 | 100,000 | $0.0003996/req |
| Professional | $49.99 | $43.99 | 1,000,000 | $0.00019996/req |
| Business | $99.99 | $84.99 | 3,000,000 | $0.00013332/req |
| Enterprise | Custom | - | Custom | Custom |

Batch endpoint requires Professional or above. Overage notifications at 75%, 90%, 100%.

## Tags

Geocoding, Reverse Geocoding, Maps, Location, Address Validation, apilayer, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Maintainers

- **Kin Lane** - kin@apievangelist.com
