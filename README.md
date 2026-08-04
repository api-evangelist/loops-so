# Loops (loops-so)

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

Loops is a modern email platform purpose-built for software companies, combining product, marketing, and transactional email behind a single REST API and a single audience. Contacts, contact properties, mailing lists, events, segments, campaigns, email messages, themes, components, uploads, transactional sends, and dedicated sending IPs are all first-class API resources, with an OpenAPI 3.1 spec published at app.loops.so/openapi.yaml. Lifecycle workflows ("loops") use the Events API as their trigger, an HMAC-SHA256-signed webhook stream broadcasts every contact and email event for real-time integrations, and official SDKs ship for JavaScript, Nuxt, PHP, Ruby, and Go alongside an official Go-based CLI. Transactional email is included on every plan, team seats are unlimited, and a generous free tier covers 1,000 contacts and 4,000 sends per month — making Loops a Tier-1 developer-first email service for SaaS teams from waitlist to IPO.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Email
- Marketing Email
- Transactional Email
- Email Automation
- Email Campaigns
- Email Workflows
- Contacts
- Audience Management
- Events
- Webhooks
- SaaS
- Developer Tools

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Loops API

The Loops API is a single REST API exposing every Loops resource — contacts, contact properties, mailing lists, events, campaigns, email messages, themes, components, transactional sends, uploads, suppressions, and dedicated sending IPs. Base URL is https://app.loops.so/api/v1. Bearer-token authentication with API keys generated in Settings → API. Defaults to 10 requests/second per team with x-ratelimit-limit and x-ratelimit-remaining response headers; returns HTTP 429 when exceeded. OpenAPI 3.1 spec published at app.loops.so/openapi.yaml.

- **Human URL:** [https://loops.so/docs/api-reference/intro](https://loops.so/docs/api-reference/intro)

#### Tags

- Email
- Marketing
- Transactional
- Contacts
- Campaigns
- Events
- SaaS

#### Properties

- [Documentation](https://loops.so/docs/api-reference/intro)
- [OpenAPI](https://app.loops.so/openapi.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](https://app.loops.so/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/loops-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/loops.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/loops.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://loops.so)
- [Documentation](https://loops.so/docs)
- [Documentation](https://loops.so/docs/api-reference/intro)
- [OpenAPI](https://app.loops.so/openapi.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](https://app.loops.so/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Getting Started](https://loops.so/docs/quickstart)
- [Webhooks](https://loops.so/docs/webhooks)
- [Integrations](https://loops.so/docs/integrations)
- [Pricing](https://loops.so/pricing)
- [Blog](https://loops.so/blog)
- [Changelog](https://loops.so/changelog)
- [Terms of Service](https://loops.so/legal/terms)
- [Privacy Policy](https://loops.so/legal/privacy)
- [Security](https://loops.so/legal/security)
- [Sign Up](https://app.loops.so/register)
- [Sign In](https://app.loops.so/login)
- [Twitter](https://twitter.com/loops_so)
- [LinkedIn](https://www.linkedin.com/company/loops-so)
- [GitHub Organization](https://github.com/loops-so)
- [SDK](https://github.com/loops-so/loops-js)
- [SDK](https://github.com/loops-so/loops-nuxt)
- [SDK](https://github.com/loops-so/loops-php)
- [SDK](https://github.com/loops-so/loops-rb)
- [SDK](https://github.com/loops-so/loops-go)
- [Tool](https://github.com/loops-so/cli)
- [Tool](https://github.com/loops-so/homebrew-tap)
- [Tool](https://github.com/loops-so/skills)
- [Code Examples](https://github.com/loops-so/loops-nextjs)
- [Package](https://www.npmjs.com/package/loops)
- [Plans](https://loops.so/pricing)
- [Authentication](undefined)
- [Rate Limits](undefined)
- [Webhooks](undefined)
- [Integrations](undefined)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
