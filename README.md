# Twenty (twenty)

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
