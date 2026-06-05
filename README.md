# Gladly (gladly)

Gladly is a San Francisco–based people-centered customer service AI platform. The Gladly Hero agent workspace unifies voice, chat, SMS, email, and social into a single, channel-agnostic conversation per Customer, while Gladly Sidekick AI handles routine resolutions, drafts replies, and hands off to humans with full context. Brands integrate via the REST API, the Chat SDK (Web/iOS/Android), the Help Center widget, the embedded App Platform, webhooks, and a brand-hosted Lookup API. Customers include JetBlue, Allbirds, Crate & Barrel, Warby Parker, Ulta, Nordstrom, TUMI, UGG, Tory Burch, and Breeze Airways.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gladly/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Customer Service
- CX
- Contact Center
- AI Customer Service
- Conversations
- Sidekick AI
- Hero
- Voice
- Chat
- SMS
- Email
- Help Center
- Webhooks
- Knowledge Base

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Gladly REST API

Gladly's unified REST API for the people-centered customer service platform. Exposes Customers, Conversations, Messages, Tasks, Answers (knowledge base), Topics, Teams, Inboxes, Audiences, Business Hours, Communications (outbound SMS/email), Webhooks, Events, Export jobs, Reports, Agents, Organization, Public Answers (Help Center), Proactive Conversations, and User Identity (JWT for authenticated chat). HTTP Basic auth with an agent email + API token. Default 10 req/sec per organization. Mounted at `https://{organization}.gladly.com/api/v1`.

- **Human URL:** [https://developer.gladly.com/rest/](https://developer.gladly.com/rest/)
- **Base URL:** `https://organization.gladly.com/api/v1`

#### Tags

- Customer Service
- CX
- Contact Center
- Conversations
- Customers
- Tasks
- Answers
- Webhooks

#### Properties

- [Documentation](https://developer.gladly.com/rest/)
- [API Reference](https://developer.gladly.com/rest/)
- [Getting Started](https://help.gladly.com/developer-tutorials/docs)
- [Authentication](https://developer.gladly.com/rest/)
- [OpenAPI](openapi/gladly-rest-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/gladly-customer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/gladly-conversation-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/gladly-task-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/gladly-answer-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/gladly-webhook-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/gladly-customer-structure.json)
- [JSON Structure](json-structure/gladly-conversation-structure.json)
- [JSON Structure](json-structure/gladly-task-structure.json)
- [JSON Structure](json-structure/gladly-answer-structure.json)
- [JSON Structure](json-structure/gladly-webhook-structure.json)
- [JSON-LD](json-ld/gladly-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/gladly-customer-create-example.json)
- [Example](examples/gladly-conversation-list-example.json)
- [Example](examples/gladly-task-create-example.json)
- [Example](examples/gladly-webhook-create-example.json)

### Gladly Lookup API

Brand-hosted "Lookup" endpoint that Gladly calls outbound to enrich a conversation with first-party customer data. Lets brands keep system-of-record customer data in their own services while presenting a unified profile inside the Gladly Hero agent workspace and to Sidekick AI.

- **Human URL:** [https://developer.gladly.com/rest/](https://developer.gladly.com/rest/)

#### Tags

- Customer Service
- Customer Data
- Webhooks
- Integrations

#### Properties

- [Documentation](https://developer.gladly.com/rest/)
- [Sample Source](https://github.com/gladly/lookup-practice)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly Chat SDK

JavaScript chat widget loaded from the Gladly CDN. Exposes `Gladly.init`, `show`, `close`, `setUser`, `startConversation`, `navigate`, `applyCampaign`, `getAvailability`, plus a full event system (availability, conversation lifecycle, messages, campaigns). Supports JWT-authenticated user identity issued by the User Identity REST endpoint.

- **Human URL:** [https://developer.gladly.com/chat/](https://developer.gladly.com/chat/)

#### Tags

- Customer Service
- Chat
- SDK
- Web

#### Properties

- [Documentation](https://developer.gladly.com/chat/)
- [SDK](https://cdn.gladly.com/chat-sdk/widget.js)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly Sidekick iOS SDK

Swift SDK (v1.2.5, iOS 11+) for embedding the Gladly Sidekick chat experience in iOS apps. Ships `Gladly`, `GladlySettings`, `GladlyUser`, `UIConfiguration`, `UIHeaderConfiguration`, and delegate protocols for chat display, notifications, and unread counts.

- **Human URL:** [https://developer.gladly.com/ios-sdk/](https://developer.gladly.com/ios-sdk/)

#### Tags

- Customer Service
- Chat
- SDK
- iOS
- Mobile

#### Properties

- [Documentation](https://developer.gladly.com/ios-sdk/)
- [Source Code](https://github.com/gladly/sidekick-ios-sdk)
- [SDK](https://github.com/gladly/sidekick-ios-sdk)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly Sidekick Android SDK

Kotlin SDK (Android Q / API 29+) for embedding the Gladly Sidekick chat experience in Android apps. Provides `Gladly.initialize`, `setUser`, `showChat`, `handleMessageReceived`, `getUnreadCount`, `registerPushToken`/`unregisterPushToken` plus EventInterface for events and errors.

- **Human URL:** [https://developer.gladly.com/android-sdk/](https://developer.gladly.com/android-sdk/)

#### Tags

- Customer Service
- Chat
- SDK
- Android
- Mobile

#### Properties

- [Documentation](https://developer.gladly.com/android-sdk/)
- [Source Code](https://github.com/gladly/sidekick-android-sdk)
- [SDK](https://github.com/gladly/sidekick-android-sdk)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly Help Center

Embeddable Help Center widget that builds an FAQ/help page on a brand's website powered by Public Answers from Gladly's Answers knowledge base. Exposes a `.gladlyHC` CSS class hierarchy for fully custom styling. SPA support is limited (Next.js not supported); best run from a single non-SPA HTML page.

- **Human URL:** [https://developer.gladly.com/help-center/](https://developer.gladly.com/help-center/)

#### Tags

- Customer Service
- Help Center
- Self-Service
- Web

#### Properties

- [Documentation](https://developer.gladly.com/help-center/)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly App Platform

Framework for building embedded "Apps" inside the Gladly Hero agent workspace. Apps surface third-party data (orders, loyalty, returns, CDP profiles) alongside the customer timeline. Authored as JavaScript/Groovy bundles and managed via the `app-platform-appcfg-cli`.

- **Human URL:** [https://help.gladly.com/developer-tutorials/docs](https://help.gladly.com/developer-tutorials/docs)

#### Tags

- Customer Service
- Apps
- Integrations
- Embedded

#### Properties

- [Documentation](https://help.gladly.com/developer-tutorials/docs)
- [Sample Source](https://github.com/gladly/app-platform-examples)
- [C L I](https://github.com/gladly/app-platform-appcfg-cli)
- [Sample Source](https://github.com/gladly/gladly-getting-started)
- [Sample Source](https://github.com/gladly/gladapp-examples)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Gladly Webhooks

Event-driven push channel that delivers Gladly platform events (conversation created/updated/closed, message created, task created/updated/closed, customer created/updated, agent state changes) to a brand-supplied HTTPS endpoint. Managed through the Webhooks REST endpoints. Includes retry policy and logging.

- **Human URL:** [https://developer.gladly.com/rest/](https://developer.gladly.com/rest/)

#### Tags

- Customer Service
- Webhooks
- Events

#### Properties

- [Documentation](https://developer.gladly.com/rest/)
- [Sample Source](https://github.com/gladly/webhook-examples)
- [JSON Schema](json-schema/gladly-webhook-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/gladly-webhook-create-example.json)
- [Postman Collection](collections/gladly-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gladly-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.gladly.ai/)
- [Documentation](https://developer.gladly.com/)
- [API Reference](https://developer.gladly.com/rest/)
- [Support](https://help.gladly.com/)
- [Getting Started](https://help.gladly.com/developer-tutorials/docs)
- [Rate Limits](https://help.gladly.com/developer-tutorials/docs/default-api-rate-limits)
- [Rate Limits](rate-limits/gladly-rate-limits.yml)
- [Pricing](https://www.gladly.ai/pricing/)
- [Plans](plans/gladly-plans-pricing.yml)
- [Fin Ops](finops/gladly-finops.yml)
- [Privacy Policy](https://www.gladly.ai/privacy-policy/)
- [Terms of Service](https://www.gladly.ai/terms-of-service/)
- [Blog](https://www.gladly.ai/blog/)
- [GitHub Organization](https://github.com/gladly)
- [LinkedIn](https://www.linkedin.com/company/gladly/)
- [Twitter](https://twitter.com/gladly)
- [YouTube](https://www.youtube.com/@gladlysoftware)
- [Spectral Rules](rules/gladly-rules.yml)
- [Vocabulary](vocabulary/gladly-vocabulary.yml)
- [JSON-LD](json-ld/gladly-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)
- [Customers](undefined)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
