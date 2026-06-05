# DroneDeploy (drone-deploy)

DroneDeploy is the unified reality-capture platform for construction, agriculture, mining, energy, oil & gas, and inspection workflows. Founded in 2013 and headquartered in San Francisco, DroneDeploy combines aerial drone mapping, ground 360 capture, robotics (DJI Dock, Boston Dynamics Spot), and vision-language AI (Progress AI, Safety AI, Earthworks AI) into a single platform that operates across 3M+ sites in 180 countries and has processed 2.8B+ images. Developers integrate via a GraphQL API at https://www.dronedeploy.com/graphql, an Apps Platform with OAuth2 templates that embed third-party apps into the DroneDeploy web application, and a 40+ partner App Market spanning construction (Procore, Autodesk Construction Cloud, PlanGrid), GIS (ArcGIS, Mapbox), cloud storage (S3, Google Drive, OneDrive, Box, Azure), and agriculture (Climate FieldView).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/drone-deploy/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/drone-deploy/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Drones
- Reality Capture
- Mapping
- Photogrammetry
- 3D Models
- Orthomosaic
- LiDAR
- Construction
- Agriculture
- AI
- Aerial
- Robotics

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### DroneDeploy GraphQL API

DroneDeploy's GraphQL API is the primary programmatic interface for the DroneDeploy reality-capture platform. A single POST endpoint at https://www.dronedeploy.com/graphql exposes a strongly-typed schema rooted at the `viewer` object that gives the authenticated user access to organizations, plans (MapPlan and other Plan variants), exports, layers, geometry, and processing status. Forward, cursor-based pagination via Relay-style edges/nodes/pageInfo. Authenticated with `Authorization Bearer` API keys obtained from DroneDeploy Support or via a Developer Partner / Enterprise account.

- **Human URL:** [https://developer-docs.dronedeploy.com/api/introduction](https://developer-docs.dronedeploy.com/api/introduction)
- **Base URL:** `https://www.dronedeploy.com/graphql`

#### Tags

- Drones
- Reality Capture
- Mapping
- GraphQL
- Plans
- Exports

#### Properties

- [Documentation](https://developer-docs.dronedeploy.com/api/introduction)
- [Authentication](https://developer-docs.dronedeploy.com/api/authentication)
- [Documentation](https://developer-docs.dronedeploy.com/api/pagination)
- [Sandbox](https://www.dronedeploy.com/graphiql/)
- [OpenAPI](openapi/drone-deploy-graphql-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/drone-deploy-graphql-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/drone-deploy-graphql-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/drone-deploy-plan-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/drone-deploy-export-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/drone-deploy-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### DroneDeploy Apps Platform

The DroneDeploy Apps Platform lets third parties build embedded apps and serverless "functions" that run inside the DroneDeploy web application and the DroneDeploy App Market. Apps consume the GraphQL API on behalf of the signed-in user, can register OAuth2 flows via the oauth-function-template, and are surfaced in the App Market across construction, agriculture, mining, utilities, and renewable energy verticals.

- **Human URL:** [https://developer-docs.dronedeploy.com/introduction/overview](https://developer-docs.dronedeploy.com/introduction/overview)

#### Tags

- Apps
- Marketplace
- OAuth
- Extensions

#### Properties

- [Documentation](https://developer-docs.dronedeploy.com/introduction/overview)
- [App Market](https://www.dronedeploy.com/product/market)
- [Code Repository](https://github.com/dronedeploy/app-examples)
- [Code Repository](https://github.com/dronedeploy/oauth-function-template)
- [SDK](https://github.com/dronedeploy/function-wrapper)
- [Postman Collection](collections/drone-deploy-graphql-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/drone-deploy-graphql-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DroneDeploy Flight Log Parser

Open-source JavaScript/TypeScript library for parsing DroneDeploy flight log files (the .csv/.json telemetry files emitted by the DroneDeploy Flight App). MIT-licensed, maintained on GitHub.

- **Human URL:** [https://github.com/dronedeploy/flight-log-parser](https://github.com/dronedeploy/flight-log-parser)

#### Tags

- SDK
- Flight Logs
- Telemetry

#### Properties

- [Code Repository](https://github.com/dronedeploy/flight-log-parser)
- [SDK](https://www.npmjs.com/package/flight-log-parser)
- [Postman Collection](collections/drone-deploy-graphql-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/drone-deploy-graphql-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.dronedeploy.com)
- [Documentation](https://developer-docs.dronedeploy.com/)
- [Documentation](https://developer-docs.dronedeploy.com/dronedeploy-apps)
- [Documentation](https://developer-docs.dronedeploy.com/api/introduction)
- [Sandbox](https://www.dronedeploy.com/graphiql/)
- [Status Page](https://status.dronedeploy.com)
- [Sign Up](https://www.dronedeploy.com/get-started)
- [Login](https://www.dronedeploy.com/app2/auth/signin)
- [Support](https://help.dronedeploy.com/hc/en-us)
- [Terms of Service](https://www.dronedeploy.com/legal/master-services-agreement)
- [Privacy Policy](https://www.dronedeploy.com/legal/privacy)
- [Blog](https://www.dronedeploy.com/blog)
- [Careers](https://www.dronedeploy.com/about/careers)
- [About Us](https://www.dronedeploy.com/about)
- [GitHub Organization](https://github.com/dronedeploy)
- [App Market](https://www.dronedeploy.com/product/market)
- [LinkedIn](https://www.linkedin.com/company/dronedeploy)
- [X (Twitter)](https://twitter.com/dronedeploy)
- [YouTube](https://www.youtube.com/c/DroneDeploy)
- [Plans](https://www.dronedeploy.com/pricing)
- [Trial](https://www.dronedeploy.com/get-started)
- [Plans](plans/drone-deploy-plans-pricing.yml)
- [Rate Limits](rate-limits/drone-deploy-rate-limits.yml)
- [Fin Ops](finops/drone-deploy-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
