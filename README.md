# Gladly (gladly)

Gladly is a San Francisco–based people-centered customer service AI platform. The Gladly **Hero** agent workspace unifies voice, chat, SMS, email, and social into a single channel-agnostic conversation per Customer, while **Gladly Sidekick AI** handles routine resolutions, drafts agent replies, and hands off to human agents with full context. Brands integrate via the REST API, the Chat SDK (Web/iOS/Android), the Help Center widget, the embedded App Platform, webhooks, and a brand-hosted Lookup API.

**URL:** [Visit APIs.yml](https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

Customer Service, CX, Contact Center, AI Customer Service, Conversations, Sidekick AI, Hero, Voice, Chat, SMS, Email, Help Center, Webhooks, Knowledge Base

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Notable Customers

JetBlue, Allbirds, Crate & Barrel, Warby Parker, Ulta Beauty, Nordstrom, TUMI, UGG, Tory Burch, Breeze Airways, Kuhl.

## APIs

### Gladly REST API

Unified REST API for the people-centered customer service platform. Exposes Customers, Conversations, Messages, Tasks, Answers (knowledge base), Topics, Teams, Inboxes, Audiences, Business Hours, Communications (outbound SMS/email), Webhooks, Events, Export jobs, Reports, Agents, Organization, Public Answers (Help Center), Proactive Conversations, and User Identity (JWT for authenticated chat). HTTP Basic auth with an agent email + API token. Default 10 requests per second per organization. Mounted at `https://{organization}.gladly.com/api/v1`.

**Human URL:** [https://developer.gladly.com/rest/](https://developer.gladly.com/rest/)

- [Documentation](https://developer.gladly.com/rest/)
- [Getting Started — Developer Tutorials](https://help.gladly.com/developer-tutorials/docs)
- [OpenAPI](openapi/gladly-rest-api-openapi.yml)
- JSON Schema: [Customer](json-schema/gladly-customer-schema.json) · [Conversation](json-schema/gladly-conversation-schema.json) · [Task](json-schema/gladly-task-schema.json) · [Answer](json-schema/gladly-answer-schema.json) · [Webhook](json-schema/gladly-webhook-schema.json)
- JSON Structure: [Customer](json-structure/gladly-customer-structure.json) · [Conversation](json-structure/gladly-conversation-structure.json) · [Task](json-structure/gladly-task-structure.json) · [Answer](json-structure/gladly-answer-structure.json) · [Webhook](json-structure/gladly-webhook-structure.json)
- JSON-LD: [gladly-context.jsonld](json-ld/gladly-context.jsonld)
- Examples: [Create Customer](examples/gladly-customer-create-example.json) · [List Conversations](examples/gladly-conversation-list-example.json) · [Create Task](examples/gladly-task-create-example.json) · [Create Webhook](examples/gladly-webhook-create-example.json)

### Gladly Lookup API

Brand-hosted endpoint Gladly calls outbound to enrich a conversation with first-party customer data. Lets brands keep customer system-of-record data in their own services while still presenting a unified profile inside the Hero agent workspace and to Sidekick AI.

- [Sample Source — lookup-practice](https://github.com/gladly/lookup-practice)

### Gladly Chat SDK (Web)

JavaScript chat widget loaded from `https://cdn.gladly.com/chat-sdk/widget.js`. Exposes `Gladly.init`, `show`, `close`, `setUser`, `startConversation`, `navigate`, `applyCampaign`, `getAvailability` plus a full event system (availability, conversation lifecycle, messages, campaigns). JWT-authenticated user identity via the User Identity REST endpoint.

- [Documentation](https://developer.gladly.com/chat/)

### Gladly Sidekick iOS SDK

Swift SDK (v1.2.5, iOS 11+) for embedding the Gladly Sidekick chat experience in iOS apps.

- [Documentation](https://developer.gladly.com/ios-sdk/)
- [Source — sidekick-ios-sdk](https://github.com/gladly/sidekick-ios-sdk)

### Gladly Sidekick Android SDK

Kotlin SDK (Android API 29+) for embedding the Gladly Sidekick chat experience in Android apps.

- [Documentation](https://developer.gladly.com/android-sdk/)
- [Source — sidekick-android-sdk](https://github.com/gladly/sidekick-android-sdk)

### Gladly Help Center

Embeddable widget that builds an FAQ / help page on a brand's website powered by Public Answers. CSS-customizable via the `.gladlyHC` class hierarchy.

- [Documentation](https://developer.gladly.com/help-center/)

### Gladly App Platform

Framework for building embedded apps inside the Gladly Hero workspace. Apps surface third-party data (orders, loyalty, returns, CDP profiles) alongside the customer timeline. Authored as JavaScript/Groovy bundles and managed via `app-platform-appcfg-cli`.

- [Documentation](https://help.gladly.com/developer-tutorials/docs)
- [Sample Source — app-platform-examples](https://github.com/gladly/app-platform-examples)
- [CLI — app-platform-appcfg-cli](https://github.com/gladly/app-platform-appcfg-cli)

### Gladly Webhooks

Event-driven push channel delivering conversation, message, task, customer, and agent-state events to brand-supplied HTTPS endpoints. Managed through the Webhooks REST endpoints with retry and logging.

- [Sample Source — webhook-examples](https://github.com/gladly/webhook-examples)
- [Webhook JSON Schema](json-schema/gladly-webhook-schema.json)

## Solutions

- **Gladly Hero** — People-centered agent workspace for voice, chat, SMS, email, and social.
- **Gladly Sidekick AI** — AI customer service agent (approx. $0.60 per AI-resolved conversation).
- **Gladly Voice AI** — Voice-channel AI assistant priced per minute.
- **Gladly Help Center** — Embedded self-service experience powered by Public Answers.
- **Gladly App Platform** — Embedded apps and connectors inside the Hero workspace.

## Pricing

| Plan | Price | Notes |
|---|---|---|
| Hero | $180 / agent / month | 10-agent minimum, billed annually |
| Superhero | $210 / agent / month | 45-agent minimum, billed annually |
| Sidekick AI | $0.60 / AI-resolved conversation | Stacks on Hero or Superhero |
| Voice AI add-on | $0.06216 / minute | Inbound Voice AI |
| Toll-free voice (inbound) | $0.02794 / minute | Per-minute charge |
| SMS | $0.00273 – $0.00637 / message | Varies by number type |
| Enterprise / Custom | Contact sales | SSO, audit logs, dedicated CSM, SLAs |

Reconciled in [`plans/gladly-plans-pricing.yml`](plans/gladly-plans-pricing.yml) and aligned to FOCUS / FinOps in [`finops/gladly-finops.yml`](finops/gladly-finops.yml).

## Rate Limits

Default REST API: **10 requests per second per organization** across all HTTP methods. The Reporting API has a separate dedicated tier. Exceeded limits return **HTTP 429** with `Ratelimit-Limit-Second` / `Ratelimit-Remaining-Second` response headers. Full machine-readable definition in [`rate-limits/gladly-rate-limits.yml`](rate-limits/gladly-rate-limits.yml).

## Integrations

Native and Marketplace integrations span e-commerce (Shopify, BigCommerce, Magento, Spree, Swell), subscriptions (Recharge, Recurly, Ordergroove, Skio), returns (AfterShip, Loop, ReturnLogic, Narvar, Corso, Shiphero, Shipped Suite), CDP/ELT (Segment, Fivetran, HighTouch), loyalty (Smile.io, LoyaltyLion, Zinrelo), marketing (Klaviyo, Attentive, Emplifi, Optimizely/Zaius), reviews (TurnTo), workforce management (Assembled, Playvox, Calabrio, MaestroQA), surveys (Medallia, Qualtrics, Delighted, Simplesat), AI partners (Ada, Netomi, Siena, KODIF.ai), agent capacity (Simplr, HiOperator, AgentsOnly), and event routing (AWS EventBridge). Full list in [`apis.yml`](apis.yml) under `Integrations`.

## GitHub

Public repos at [github.com/gladly](https://github.com/gladly):

| Repo | Purpose | Language |
|---|---|---|
| [rest-api-examples](https://github.com/gladly/rest-api-examples) | Node.js examples for the REST API | JavaScript |
| [sidekick-ios-sdk](https://github.com/gladly/sidekick-ios-sdk) | iOS chat SDK | Swift |
| [sidekick-android-sdk](https://github.com/gladly/sidekick-android-sdk) | Android chat SDK | Kotlin |
| [app-platform-examples](https://github.com/gladly/app-platform-examples) | App Platform sample apps | Groovy |
| [app-platform-appcfg-cli](https://github.com/gladly/app-platform-appcfg-cli) | App Platform CLI | Shell |
| [webhook-examples](https://github.com/gladly/webhook-examples) | Webhook receiver samples | JavaScript |
| [help-center-examples](https://github.com/gladly/help-center-examples) | Help Center embed samples | HTML |
| [lookup-practice](https://github.com/gladly/lookup-practice) | Lookup API practice resources | JavaScript |
| [gladly-getting-started](https://github.com/gladly/gladly-getting-started) | App Platform tutorial assets | Groovy |
| [gladapp-examples](https://github.com/gladly/gladapp-examples) | Additional app samples | JavaScript |

## Authentication

HTTP Basic — username is the API user's email, password is the API token. The API user requires the **API User** permission inside the Gladly organization. All requests must be HTTPS. Production base URL is `https://{organization}.gladly.com/api/v1`; the QA / sandbox is `https://{organization}.gladly.qa/api/v1`.

## Naftiko Capabilities

21 Naftiko capability files in [`capabilities/`](capabilities/), one per business surface (Agents, Answer Management, Audiences, Business Hours, Communications, Conversations, Customers, Events, Export, Freeform Topics, Inboxes, Organization, Payloads, Proactive Conversations, Public Answer, Reports, Tasks, Teams, Topics, User Identity, Webhooks). Each exposes both a REST adapter and an MCP tool surface.

## Governance Artifacts

- **Spectral rules:** [`rules/gladly-rules.yml`](rules/gladly-rules.yml)
- **Vocabulary:** [`vocabulary/gladly-vocabulary.yml`](vocabulary/gladly-vocabulary.yml)
- **JSON-LD context:** [`json-ld/gladly-context.jsonld`](json-ld/gladly-context.jsonld)
