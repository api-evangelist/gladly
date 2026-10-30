# Gladly

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

Gladly is a San Francisco–based people-centered customer service AI platform. The Gladly Hero agent workspace unifies voice, chat, SMS, email, and social into a single, channel-agnostic conversation per Customer, while Gladly Sidekick AI handles routine resolutions, drafts replies, and hands off to humans with full context. Brands integrate via the REST API, the Chat SDK (Web/iOS/Android), the Help Center widget, the embedded App Platform, webhooks, and a brand-hosted Lookup API. Customers include JetBlue, Allbirds, Crate & Barrel, Warby Parker, Ulta, Nordstrom, TUMI, UGG, Tory Burch, and Breeze Airways.

**Areas:** Customer Service · Customer Experience · Contact Center · AI Customer Service · Conversations · Sidekick AI · Hero · Voice · Chat · SMS · Email · Help Center

## Gladly on APIs.io

Everything profiled for Gladly is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/gladly/](https://apis.io/providers/gladly/)** — or go straight to one of the APIs or properties below.

### APIs (28)

- [Gladly Lookup API](https://apis.io/apis/gladly/gladly-lookup-api/) — Brand-hosted "Lookup" endpoint that Gladly calls outbound to enrich a conversation with first-party customer data. Lets brands keep system-of-record…
- [Gladly Chat SDK](https://apis.io/apis/gladly/gladly-chat-sdk/) — JavaScript chat widget loaded from the Gladly CDN. Exposes `Gladly.init`, `show`, `close`, `setUser`, `startConversation`, `navigate`, `applyCampaign`,…
- [Gladly Sidekick iOS SDK](https://apis.io/apis/gladly/gladly-sidekick-ios-sdk/) — Swift SDK (v1.2.5, iOS 11+) for embedding the Gladly Sidekick chat experience in iOS apps. Ships `Gladly`, `GladlySettings`, `GladlyUser`,…
- [Gladly Sidekick Android SDK](https://apis.io/apis/gladly/gladly-sidekick-android-sdk/) — Kotlin SDK (Android Q / API 29+) for embedding the Gladly Sidekick chat experience in Android apps. Provides `Gladly.initialize`, `setUser`, `showChat`,…
- [Gladly Help Center](https://apis.io/apis/gladly/gladly-help-center/) — Embeddable Help Center widget that builds an FAQ/help page on a brand's website powered by Public Answers from Gladly's Answers knowledge base. Exposes a…
- [Gladly App Platform](https://apis.io/apis/gladly/gladly-app-platform/) — Framework for building embedded "Apps" inside the Gladly Hero agent workspace. Apps surface third-party data (orders, loyalty, returns, CDP profiles)…
- [Gladly Webhooks](https://apis.io/apis/gladly/gladly-webhooks/) — Event-driven push channel that delivers Gladly platform events (conversation created/updated/closed, message created, task created/updated/closed, customer…
- [Gladly Agents API](https://apis.io/apis/gladly/gladly-agents-api/) — An **Agent** represents the user profile of a person who helps customers in Gladly. The API allows you to lookup Agents who participated in conversations…
- [Gladly Answer Management API](https://apis.io/apis/gladly/gladly-answer-management-api/) — The **Answer Management API** allows you to create, update, and delete Answers in Gladly. To create an Answer with content, two calls would be needed. One…
- [Gladly Audiences API](https://apis.io/apis/gladly/gladly-audiences-api/) — An **Audience** represents a brand (or segment) specially for a multi-brand company. They are used to categorize Answers, Help Centers and Chats for the…
- [Gladly Business Hours API](https://apis.io/apis/gladly/gladly-business-hours-api/) — **Business Hours** define the operating schedule for your organization. They determine when your organization is available to handle customer communications…
- [Gladly Communications API](https://apis.io/apis/gladly/gladly-communications-api/) — Communications API enables you to programmatically send messages to your customers. These messages are non-routable and non-searchable. ### Agent View…
- [Gladly Conversations API](https://apis.io/apis/gladly/gladly-conversations-api/) — ## Conversation A **Conversation** in Gladly contains the timeline of activity for a customer including communications to and from your organization along…
- [Gladly Customers API](https://apis.io/apis/gladly/gladly-customers-api/) — A **Customer** in Gladly represents information about a customer of your organization including their profile, contact information, notes, and transactions.…
- [Gladly Events API](https://apis.io/apis/gladly/gladly-events-api/) — An **Event** is something that has happened in Gladly. The Events API allows you to extract event details from the past 24 hours.
- [Gladly Export API](https://apis.io/apis/gladly/gladly-export-api/) — Export API is a simple, comprehensive, file-based data export. You can export the lifetime of your customers' conversations in Gladly to a central data…
- [Gladly Freeform Topics API](https://apis.io/apis/gladly/gladly-freeform-topics-api/) — Freeform Topics allow you to associate granular data like Order Number to a Conversation. This data can be accessed for analysis via APIs, Webhooks, and AWS…
- [Gladly Inboxes API](https://apis.io/apis/gladly/gladly-inboxes-api/) — An **Inbox** receives customer communications in Gladly. The communications route to the inbox according to channel and destination endpoint configuration.…
- [Gladly Organization API](https://apis.io/apis/gladly/gladly-organization-api/) — An **Organization** contains metadata about your company that Gladly is configured with.
- [Gladly Payloads API](https://apis.io/apis/gladly/gladly-payloads-api/) — The Payloads API from Gladly — 1 operation(s) for payloads.
- [Gladly Proactive Conversations API](https://apis.io/apis/gladly/gladly-proactive-conversations-api/) — A proactive conversation consists of a **campaign** and **recipients**. This APIs intended use-case would be to provide status updates to a customer and not…
- [Gladly Public Answer API](https://apis.io/apis/gladly/gladly-public-answer-api/) — A **Public Answer** in Gladly represents a consumer-facing Answer. The Public Answers API allows you to search and retrieve Public Answers (created directly…
- [Gladly Reports API](https://apis.io/apis/gladly/gladly-reports-api/) — A **Report** in Gladly contains metrics that you need to run the contact center. Reports API allows you to access Gladly's reports programatically.
- [Gladly Tasks API](https://apis.io/apis/gladly/gladly-tasks-api/) — A task is a way to create and do internal follow-up work for a customer within Gladly. Tasks have a due date, an assignee, a description of what is needed…
- [Gladly Teams API](https://apis.io/apis/gladly/gladly-teams-api/) — A **Team** represents a group of Agents. They may handle particular **Inboxes** or types of work within Gladly.
- [Gladly Topics API](https://apis.io/apis/gladly/gladly-topics-api/) — A **Topic** is a way of labeling a conversation in Gladly for specific business purposes. For example, an agent may apply the topic "Return" to a…
- [Gladly User Identity API](https://apis.io/apis/gladly/gladly-user-identity-api/) — The User Identity API from Gladly — 1 operation(s) for user identity.
- [Gladly Webhooks API](https://apis.io/apis/gladly/gladly-webhooks-api/) — A **Webhook** is a way to send notifications about Gladly events as a POST request to the endpoint of your choice.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Gladly Agentic Access](https://apis.io/agentic-access/gladly/gladly-agentic-access/)

#### JSON Schema (5)

The data models the API reads and writes.

- [Gladly Answer](https://apis.io/schemas/gladly/gladly-answer/)
- [Gladly Conversation](https://apis.io/schemas/gladly/gladly-conversation/)
- [Gladly Customer](https://apis.io/schemas/gladly/gladly-customer/)
- [Gladly Task](https://apis.io/schemas/gladly/gladly-task/)
- [Gladly Webhook](https://apis.io/schemas/gladly/gladly-webhook/)

#### JSON Structure (5)

Data models expressed in JSON Structure.

- [Gladly Answer Structure](https://apis.io/json-structure/gladly/gladly-answer-structure/)
- [Gladly Conversation Structure](https://apis.io/json-structure/gladly/gladly-conversation-structure/)
- [Gladly Customer Structure](https://apis.io/json-structure/gladly/gladly-customer-structure/)
- [Gladly Task Structure](https://apis.io/json-structure/gladly/gladly-task-structure/)
- [Gladly Webhook Structure](https://apis.io/json-structure/gladly/gladly-webhook-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Gladly Context](https://apis.io/jsonld/gladly/gladly-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Gladly Domain Vocabulary](https://apis.io/vocabularies/gladly/gladly-vocabulary/)

#### Examples (4)

Example requests and responses.

- [Gladly Conversation List Example](https://apis.io/examples/gladly/gladly-conversation-list-example/)
- [Gladly Customer Create Example](https://apis.io/examples/gladly/gladly-customer-create-example/)
- [Gladly Task Create Example](https://apis.io/examples/gladly/gladly-task-create-example/)
- [Gladly Webhook Create Example](https://apis.io/examples/gladly/gladly-webhook-create-example/)

#### Collections (43)

Postman and Open Collection request collections.

- [Gladly Agents API](https://apis.io/collections/gladly/open-gladly-agents-api/)
- [Gladly Agents Answer Management API](https://apis.io/collections/gladly/open-gladly-answer-management-api/)
- [Gladly Agents Audiences API](https://apis.io/collections/gladly/open-gladly-audiences-api/)
- [Gladly Agents Business Hours API](https://apis.io/collections/gladly/open-gladly-business-hours-api/)
- [Gladly Agents Communications API](https://apis.io/collections/gladly/open-gladly-communications-api/)
- [Gladly Agents Conversations API](https://apis.io/collections/gladly/open-gladly-conversations-api/)
- [Gladly Agents Customers API](https://apis.io/collections/gladly/open-gladly-customers-api/)
- [Gladly Agents Events API](https://apis.io/collections/gladly/open-gladly-events-api/)
- [Gladly Agents Export API](https://apis.io/collections/gladly/open-gladly-export-api/)
- [Gladly Agents Freeform Topics API](https://apis.io/collections/gladly/open-gladly-freeform-topics-api/)
- [Gladly Agents Inboxes API](https://apis.io/collections/gladly/open-gladly-inboxes-api/)
- [Gladly Agents Organization API](https://apis.io/collections/gladly/open-gladly-organization-api/)
- [Gladly Agents Payloads API](https://apis.io/collections/gladly/open-gladly-payloads-api/)
- [Gladly Agents Proactive Conversations API](https://apis.io/collections/gladly/open-gladly-proactive-conversations-api/)
- [Gladly Agents Public Answer API](https://apis.io/collections/gladly/open-gladly-public-answer-api/)
- [Gladly Agents Reports API](https://apis.io/collections/gladly/open-gladly-reports-api/)
- [Gladly API](https://apis.io/collections/gladly/open-gladly-rest-api/)
- [Gladly Agents Tasks API](https://apis.io/collections/gladly/open-gladly-tasks-api/)
- [Gladly Agents Teams API](https://apis.io/collections/gladly/open-gladly-teams-api/)
- [Gladly Agents Topics API](https://apis.io/collections/gladly/open-gladly-topics-api/)
- [Gladly Agents User Identity API](https://apis.io/collections/gladly/open-gladly-user-identity-api/)
- [Gladly Agents Webhooks API](https://apis.io/collections/gladly/open-gladly-webhooks-api/)
- [Gladly Agents API](https://apis.io/collections/gladly/postman-gladly-agents-api/)
- [Gladly Agents Answer Management API](https://apis.io/collections/gladly/postman-gladly-answer-management-api/)
- [Gladly Agents Audiences API](https://apis.io/collections/gladly/postman-gladly-audiences-api/)
- …and 18 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Gladly — jsonschema rules](https://apis.io/rules/gladly/gladly-jsonschema-spectral-rules/)
- [Gladly API Rules](https://apis.io/rules/gladly/gladly-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Gladly Authentication](https://apis.io/security/gladly/gladly-authentication/)
- [Gladly Domain Security](https://apis.io/security/gladly/gladly-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Gladly Plans Pricing](https://apis.io/plans/gladly/gladly-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Gladly Rate Limits](https://apis.io/rate-limits/gladly/gladly-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Gladly Finops](https://apis.io/finops/gladly/gladly-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://gladly.com)
- [Documentation](https://developer.gladly.com/)
- [Getting started](https://help.gladly.com/developer-tutorials/docs)
- [API reference](https://developer.gladly.com/rest/)
- [Pricing](https://www.gladly.ai/pricing/)
- [Support](https://help.gladly.com/)
- [Blog](https://www.gladly.ai/blog/)
- [Terms of service](https://www.gladly.ai/terms-of-service/)
- [Privacy policy](https://www.gladly.ai/privacy-policy/)
- [GitHub](https://github.com/gladly)

## API Evangelist rating

**Kin Score 54.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 64.6 |
| Contract governance | 27.3 |
| Operational transparency | 10.5 |
| Developer ergonomics | 82.1 |
| Access clarity | 47.4 |

**Agent readiness 35.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | verified |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 20.8** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/gladly/](https://apis.io/providers/gladly/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Gladly: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/gladly/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
