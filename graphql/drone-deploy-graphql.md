# DroneDeploy GraphQL API

DroneDeploy's GraphQL API is the primary programmatic interface for the DroneDeploy reality-capture platform. A single POST endpoint at https://www.dronedeploy.com/graphql exposes a strongly-typed schema rooted at the `viewer` object that gives the authenticated user access to organizations, plans (MapPlan and other Plan variants), exports, layers, geometry, and processing status. Forward, cursor-based pagination via Relay-style edges/nodes/pageInfo. Authenticated with `Authorization Bearer` API keys obtained from DroneDeploy Support or via a Developer Partner / Enterprise account.

**Endpoint:** https://www.dronedeploy.com/graphql

**Documentation:** https://developer-docs.dronedeploy.com/api/introduction

**References:**

- Documentation: https://developer-docs.dronedeploy.com/api/introduction
- Authentication: https://developer-docs.dronedeploy.com/api/authentication
- Documentation: https://developer-docs.dronedeploy.com/api/pagination
