# DroneDeploy (drone-deploy)

DroneDeploy is the unified reality-capture platform for construction, agriculture, mining, energy, oil and gas, and inspection workflows. Founded in 2013 and headquartered in San Francisco, DroneDeploy combines aerial drone mapping, ground 360 capture, robotics (DJI Dock, Boston Dynamics Spot), and vision-language AI (Progress AI, Safety AI, Earthworks AI) into a single platform that operates across 3M+ sites in 180 countries and has processed 2.8B+ images. Developers integrate via a GraphQL API at https://www.dronedeploy.com/graphql, an Apps Platform with OAuth2 templates that embed third-party apps inside the DroneDeploy web application, and a 40+ partner App Market.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/drone-deploy/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Drones, Reality Capture, Mapping, Photogrammetry, 3D Models, Orthomosaic, LiDAR, Construction, Agriculture, AI, Aerial, Robotics

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### DroneDeploy GraphQL API
Single POST endpoint at `https://www.dronedeploy.com/graphql` exposing a strongly-typed schema rooted at the `viewer` object. Provides organization, plans (`MapPlan` and other Plan variants), exports, layers, geometry, and processing status. Forward, Relay-style cursor pagination. Authentication is `Authorization: Bearer <api_key>`.

**Human URL:** [https://developer-docs.dronedeploy.com/api/introduction](https://developer-docs.dronedeploy.com/api/introduction)

- [Documentation - Introduction](https://developer-docs.dronedeploy.com/api/introduction)
- [Documentation - Authentication](https://developer-docs.dronedeploy.com/api/authentication)
- [Documentation - Pagination](https://developer-docs.dronedeploy.com/api/pagination)
- [Sandbox - GraphiQL Explorer](https://www.dronedeploy.com/graphiql/)
- [OpenAPI](openapi/drone-deploy-graphql-api-openapi.yml)
- [JSON Schema - Plan](json-schema/drone-deploy-plan-schema.json)
- [JSON Schema - Export](json-schema/drone-deploy-export-schema.json)
- [JSON-LD Context](json-ld/drone-deploy-context.jsonld)
- [Naftiko Capability - Viewer](capabilities/graphql-viewer.yaml)
- [Naftiko Capability - Plans](capabilities/graphql-plans.yaml)
- [Naftiko Capability - Exports](capabilities/graphql-exports.yaml)

### DroneDeploy Apps Platform
Embedded apps and serverless "functions" that run inside the DroneDeploy web application and the App Market. Apps consume the GraphQL API on behalf of the signed-in user; OAuth2 flows handled via the `oauth-function-template`.

**Human URL:** [https://developer-docs.dronedeploy.com/introduction/overview](https://developer-docs.dronedeploy.com/introduction/overview)

- [Apps Documentation](https://developer-docs.dronedeploy.com/dronedeploy-apps)
- [App Market](https://www.dronedeploy.com/product/market)
- [App Examples (GitHub)](https://github.com/dronedeploy/app-examples)
- [OAuth Function Template (GitHub)](https://github.com/dronedeploy/oauth-function-template)
- [Function Wrapper (GitHub)](https://github.com/dronedeploy/function-wrapper)

### DroneDeploy Flight Log Parser
Open-source JavaScript/TypeScript library for parsing DroneDeploy flight log files.

**Human URL:** [https://github.com/dronedeploy/flight-log-parser](https://github.com/dronedeploy/flight-log-parser)

## Pricing Snapshot

| Plan | Price | Image cap | Notes |
|---|---|---|---|
| Ag Lite | $1,908 / pilot / yr | 1,000 / map | Stand Count, Live Map |
| Flight & Analysis | $4,188 / pilot / yr | 3,000 / map | Email + live chat |
| Advanced Flight & Analysis | Custom | 10,000 / map | Cut/fill, thermal, vertical |
| DroneDeploy Unified | Custom | n/a | Aerial + Ground + Robotics + AI |

14-day free trial, no credit card required: https://www.dronedeploy.com/get-started

## Operational

- [Status](https://status.dronedeploy.com)
- [Help Center](https://help.dronedeploy.com/hc/en-us)
- [Master Services Agreement](https://www.dronedeploy.com/legal/master-services-agreement)
- [Privacy Policy](https://www.dronedeploy.com/legal/privacy)
- [Blog](https://www.dronedeploy.com/blog)
- [Careers](https://www.dronedeploy.com/about/careers)
- [GitHub Organization](https://github.com/dronedeploy)

## Generated artifacts

- [Plans & Pricing](plans/drone-deploy-plans-pricing.yml)
- [Rate Limits](rate-limits/drone-deploy-rate-limits.yml)
- [FinOps](finops/drone-deploy-finops.yml)
- [Vocabulary](vocabulary/drone-deploy-vocabulary.yml)
- [Spectral Rules](rules/drone-deploy-rules.yml)
- [Example - List Plans](examples/drone-deploy-list-plans-example.json)
- [Example - Create Export](examples/drone-deploy-create-export-example.json)

## Maintainers

- Kin Lane (info@apievangelist.com) - [apievangelist.com](https://apievangelist.com)
