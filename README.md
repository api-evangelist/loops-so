# Loops (loops-so)
Loops is a modern email platform purpose-built for software companies, combining product, marketing, and transactional email behind a single REST API and a single audience. Contacts, contact properties, mailing lists, events, segments, campaigns, email messages, themes, components, uploads, transactional sends, and dedicated sending IPs are all first-class API resources, with an OpenAPI 3.1 spec published at app.loops.so/openapi.yaml. Lifecycle workflows ("loops") use the Events API as their trigger, an HMAC-SHA256-signed webhook stream broadcasts every contact and email event for real-time integrations, and official SDKs ship for JavaScript, Nuxt, PHP, Ruby, and Go alongside an official Go-based CLI. Transactional email is included on every plan, team seats are unlimited, and a generous free tier covers 1,000 contacts and 4,000 sends per month — making Loops a Tier-1 developer-first email service for SaaS teams from waitlist to IPO.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/loops-so/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Email, Marketing Email, Transactional Email, Email Automation, Email Campaigns, Email Workflows, Contacts, Audience Management, Events, Webhooks, SaaS, Developer Tools

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Loops API
Single REST API exposing every Loops resource — contacts, contact properties, mailing lists, events, campaigns, email messages, themes, components, transactional sends, uploads, suppressions, and dedicated sending IPs. Base URL `https://app.loops.so/api/v1`. Bearer-token authentication; 10 req/sec/team baseline rate limit with `x-ratelimit-*` response headers. OpenAPI 3.1 published at `app.loops.so/openapi.yaml`.

**Human URL:** [https://loops.so/docs/api-reference/intro](https://loops.so/docs/api-reference/intro)

- [Documentation](https://loops.so/docs/api-reference/intro)
- [OpenAPI (canonical)](https://app.loops.so/openapi.yaml)
- [OpenAPI (JSON)](https://app.loops.so/openapi.json)
- [OpenAPI (local)](openapi/loops-openapi.yml)

#### Resource map

| Tag | Endpoints |
|---|---|
| API Key | `GET /api-key` |
| Contacts | `POST /contacts/create`, `PUT /contacts/update`, `GET /contacts/find`, `POST /contacts/delete`, `GET /contacts/suppression`, `DELETE /contacts/suppression` |
| Contact Properties | `POST /contacts/properties`, `GET /contacts/properties` |
| Mailing Lists | `GET /lists` |
| Events | `POST /events/send` |
| Campaigns | `GET /campaigns`, `POST /campaigns`, `GET /campaigns/{id}`, `POST /campaigns/{id}` |
| Email Messages | `GET /campaigns/{id}/messages/{id}`, `POST /campaigns/{id}/messages/{id}` |
| Themes | `GET /themes`, `GET /themes/{id}` |
| Components | `GET /components`, `GET /components/{id}` |
| Transactional | `POST /transactional`, `GET /transactional` |
| Uploads | `POST /uploads`, `POST /uploads/complete` |
| Dedicated Sending IPs | `GET /dedicated-sending-ips` |

## Pricing

- **Free** — 1,000 subscribed contacts, 4,000 sends/month, all features, Loops branding at the bottom of emails
- **Paid** — removes send limits and Loops branding; never charged per seat or per send
- **Custom** — dedicated IPs and bespoke terms for high-volume senders

Transactional email is included at no extra charge on every plan.

## Webhooks

Configure a single webhook endpoint per account at Settings → Webhooks. Each event carries `Webhook-Id`, `Webhook-Timestamp`, and `Webhook-Signature` (HMAC-SHA256). Schema version `1.0.0`. 30 days of delivery history retained. Delivery is capped at 10 events/second.

Event categories:

- **Contact:** `contact.created`, `contact.unsubscribed`, `contact.deleted`, `contact.mailingList.subscribed`, `contact.mailingList.unsubscribed`
- **Sends:** `campaign.email.sent`, `loop.email.sent`, `transactional.email.sent`
- **Engagement:** `email.delivered`, `email.opened`, `email.clicked`, `email.softBounced`, `email.hardBounced`, `email.unsubscribed`, `email.resubscribed`, `email.spamReported`
- **Testing:** `testing.testEvent`

## SDKs and Tools

- [loops-js](https://github.com/loops-so/loops-js) — official TypeScript/JavaScript SDK ([npm](https://www.npmjs.com/package/loops))
- [loops-nuxt](https://github.com/loops-so/loops-nuxt) — official Nuxt module
- [loops-php](https://github.com/loops-so/loops-php) — official PHP SDK
- [loops-rb](https://github.com/loops-so/loops-rb) — official Ruby SDK
- [loops-go](https://github.com/loops-so/loops-go) — official Go SDK
- [cli](https://github.com/loops-so/cli) — official Loops CLI (Go) with [Homebrew tap](https://github.com/loops-so/homebrew-tap)
- [skills](https://github.com/loops-so/skills) — official Claude Code Skills for the Loops API and CLI
- [loops-nextjs](https://github.com/loops-so/loops-nextjs) — example Next.js app

## Integrations

25+ integrations across contact sync, authentication email, event ingestion, and template import:

**Payments & billing:** Stripe
**Authentication email:** Supabase, Clerk, Auth0, Auth.js, Better Auth
**Product analytics & CDPs:** PostHog, Segment, RudderStack, Fivetran
**CRM:** HubSpot, Salesforce, Attio, Clay
**No-code & automation:** Zapier, Make, Integrately, Bubble, Framer, Webflow
**Template import:** Emailify, Email Love
**Custom:** Incoming Webhooks for arbitrary HTTP payloads

## Maintainers

- **Kin Lane** — info@apievangelist.com — [apievangelist.com](https://apievangelist.com) — X: [@apievangelist](https://twitter.com/apievangelist)
