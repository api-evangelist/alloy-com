# Alloy

Alloy is a New York-based identity decisioning platform that helps banks,
credit unions, and fintechs onboard, monitor, and protect customers across
KYC, KYB, AML, fraud, credit, and ongoing-monitoring use cases. The Alloy API
exposes the platform's evaluations, journey applications, entities, events,
documents, cases, investigations, lists, and webhooks for programmatic
identity decisioning and ongoing risk monitoring.

This repository is an API Evangelist catalog entry for Alloy and contains a
machine-readable [`apis.yml`](apis.yml), an [`OpenAPI`](openapi/alloy-openapi.yml)
spec assembled from Alloy's public developer reference, a set of Naftiko
capability definitions, and API Commons artifacts for plans, rate limits, and
FinOps.

## Provider

- Website: [https://www.alloy.com/](https://www.alloy.com/)
- Developer portal: [https://www.alloy.com/developer](https://www.alloy.com/developer)
- Documentation: [https://developer.alloy.com/public/docs](https://developer.alloy.com/public/docs)
- API reference: [https://developer.alloy.com/public/reference](https://developer.alloy.com/public/reference)
- Machine-readable docs index: [https://developer.alloy.com/llms.txt](https://developer.alloy.com/llms.txt)
- Status: [https://status.alloy.com/](https://status.alloy.com/)
- Help center: [https://help.alloy.com](https://help.alloy.com)
- Security: [https://www.alloy.com/security](https://www.alloy.com/security)
- GitHub organization: [https://github.com/UseAlloy](https://github.com/UseAlloy)

## API Surface

The Alloy API is a REST API served at two base URLs:

- Sandbox: `https://sandbox.alloy.co/v1`
- Production: `https://api.alloy.co/v1`

Authentication is supported via HTTP Basic with workflow or account-level API
keys, HMAC signing, and OAuth 2.0 bearer tokens (Client Credentials and
Password grants).

### Resource groups

- **Evaluations** - run, retrieve, update, and audit identity decisioning
  evaluations.
- **Journeys** - multi-step decisioning workflows, journey applications,
  batches, reviews, and rerun.
- **Entities** - person and business entities, merging, notes, feedback, and
  entity groups.
- **Bank Accounts** - account creation and lookup by token or external
  identifier.
- **Documents** - document upload, replacement, and per-entity attachment for
  document verification.
- **Events** - real-time monitoring events for entities, accounts,
  transactions, logins, and credentials.
- **Cases** - case management, evidences, and works.
- **Investigations** - investigation lifecycle with assignable agents,
  types, alerts, and reviews.
- **Lists and Custom Lists** - reference data with versioning and activation.
- **Published Attributes** - tenant-defined attributes for policy and models.
- **Portfolio Evaluations** - bulk re-evaluation across portfolios.
- **OAuth** - bearer token issuance and validation.

## Artifacts

| Artifact | Path |
|---|---|
| APIs.yml | [`apis.yml`](apis.yml) |
| Review | [`review.yml`](review.yml) |
| OpenAPI | [`openapi/alloy-openapi.yml`](openapi/alloy-openapi.yml) |
| Capabilities | [`capabilities/`](capabilities/) |
| Plans | [`plans/alloy-plans-pricing.yml`](plans/alloy-plans-pricing.yml) |
| Rate Limits | [`rate-limits/alloy-rate-limits.yml`](rate-limits/alloy-rate-limits.yml) |
| FinOps | [`finops/alloy-finops.yml`](finops/alloy-finops.yml) |

### Naftiko capabilities

- [`capabilities/alloy-evaluations.yaml`](capabilities/alloy-evaluations.yaml)
- [`capabilities/alloy-journeys.yaml`](capabilities/alloy-journeys.yaml)
- [`capabilities/alloy-entities.yaml`](capabilities/alloy-entities.yaml)
- [`capabilities/alloy-events.yaml`](capabilities/alloy-events.yaml)
- [`capabilities/alloy-cases.yaml`](capabilities/alloy-cases.yaml)
- [`capabilities/alloy-investigations.yaml`](capabilities/alloy-investigations.yaml)
- [`capabilities/alloy-documents.yaml`](capabilities/alloy-documents.yaml)
- [`capabilities/alloy-lists.yaml`](capabilities/alloy-lists.yaml)
- [`capabilities/alloy-oauth.yaml`](capabilities/alloy-oauth.yaml)

## Maintainers

- Kin Lane - kin@apievangelist.com - [API Evangelist](https://apievangelist.com)
