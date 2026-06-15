# Loops (loops-so)

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
