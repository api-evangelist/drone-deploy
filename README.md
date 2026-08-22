# DroneDeploy (drone-deploy)

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
