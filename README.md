# Twenty (twenty)

Twenty is an open-source CRM platform built as a modern alternative to Salesforce, designed for teams that need flexibility, data ownership, and a contemporary developer experience. It provides REST and GraphQL APIs covering core CRM operations such as managing companies, people, opportunities, notes, tasks, and fully customizable objects. Developers can extend Twenty with custom objects, server-side logic, UI components, and AI agents as TypeScript packages, all surfaced through the same API surface. The platform is available as a cloud service or as a self-hosted deployment via Docker Compose, giving teams full control over their data residency and infrastructure.

APIs.json: https://raw.githubusercontent.com/api-evangelist/twenty/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=twenty-api-evangelist&utm_content=repo

## Tags

- CRM
- Open Source
- REST
- GraphQL
- Webhooks
- Self-Hosted
- Companies
- People
- Opportunities
- Workflows
- AI Agents
- Custom Objects

## APIs

| API | Description |
|-----|-------------|
| Twenty Core API | REST and GraphQL endpoints for CRUD operations on all CRM records including companies, people, opportunities, notes, tasks, and custom objects. Supports batch operations up to 60 records per request. |
| Twenty Metadata API | REST and GraphQL endpoints for programmatic schema management — create, update, and delete custom objects, fields, and relations within a workspace. |

## Plans / Rate Limits / FinOps

| Resource | Location |
|----------|----------|
| Plans and Pricing | [plans/twenty-plans-pricing.yml](plans/twenty-plans-pricing.yml) |
| Rate Limits | [rate-limits/twenty-rate-limits.yml](rate-limits/twenty-rate-limits.yml) |
| FinOps | [finops/twenty-finops.yml](finops/twenty-finops.yml) |

### Pricing Summary

| Plan | Price |
|------|-------|
| Self-Hosted | Free (infrastructure costs borne by operator) |
| Pro | $9 / user / month ($6.75 annually) |
| Organization | $19 / user / month ($14.25 annually) |

### Rate Limit Summary

| Plan | API Calls/Minute | Batch Records/Request |
|------|------------------|-----------------------|
| Pro | 50 | 60 |
| Organization | 100 | 60 |
| Self-Hosted | Configurable | 60 |

## Timestamps

- Created: 2026-06-12
- Modified: 2026-06-12

## Common

| Type | URL |
|------|-----|
| Website | https://twenty.com |
| Documentation | https://docs.twenty.com/developers/introduction |
| GitHub Org | https://github.com/twentyhq |
| LinkedIn | https://www.linkedin.com/company/twenty |
| Blog / Releases | https://twenty.com/releases |
| Pricing | https://twenty.com/pricing |
| X (Twitter) | https://x.com/twentycrm |

## Maintainers

| Name | Email |
|------|-------|
| Kin Lane | kin@apievangelist.com |
