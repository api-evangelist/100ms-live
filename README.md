# 100ms

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

100ms is a live video and audio infrastructure company headquartered in Bengaluru, India that provides developer SDKs and a REST control plane for embedding video conferencing, interactive live streaming (HLS), RTMP ingest/egress, recording, real-time chat/messaging, polls, whiteboard, and AI-powered transcription into applications. The company was acquired by Disney+ Hotstar (JioCinema/JioHotstar) in 2023 and continues to operate as an independent commercial SaaS — the same infrastructure powering some of the largest live cricket audiences in the world (IPL on JioCinema/Hotstar). The platform exposes a single Server-Side REST API at api.100ms.live/v2 plus client SDKs for Web (JavaScript/React), iOS (Swift), Android (Kotlin), React Native, Flutter, and a Node.js server SDK, with public OpenAPI specs generated from the docs and a Postman collection.

**Areas:** Live Streaming · Video Conferencing · WebRTC · HLS · RTMP · Recording · Real-Time Messaging · Live Infrastructure · India

## 100ms on APIs.io

Everything profiled for 100ms is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/100ms-live/](https://apis.io/providers/100ms-live/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [100ms Active Rooms API](https://apis.io/apis/100ms-live/100ms-live-active-rooms-api/) — In-session control of running rooms and connected peers.
- [100ms Analytics API](https://apis.io/apis/100ms-live/100ms-live-analytics-api/) — Query webhook events, track events, recording events, errors, and peer quality.
- [100ms External Streams API](https://apis.io/apis/100ms-live/100ms-live-external-streams-api/) — Push the room feed to YouTube / Twitch / Facebook via RTMP.
- [100ms Live Streams API](https://apis.io/apis/100ms-live/100ms-live-live-streams-api/) — HLS live streams driven from a 100ms room.
- [100ms Policy API](https://apis.io/apis/100ms-live/100ms-live-policy-api/) — Templates, roles, and recording configuration.
- [100ms Polls API](https://apis.io/apis/100ms-live/100ms-live-polls-api/) — Real-time polls and quizzes inside a room.
- [100ms Recording Assets API](https://apis.io/apis/100ms-live/100ms-live-recording-assets-api/) — Output assets (mp4, mp3, transcript, chat) produced by recordings.
- [100ms Recordings API](https://apis.io/apis/100ms-live/100ms-live-recordings-api/) — Composite and track-level recordings of sessions.
- [100ms Room Codes API](https://apis.io/apis/100ms-live/100ms-live-room-codes-api/) — Short codes used by client apps to join a room.
- [100ms Rooms API](https://apis.io/apis/100ms-live/100ms-live-rooms-api/) — Persistent containers for a live session.
- [100ms Sessions API](https://apis.io/apis/100ms-live/100ms-live-sessions-api/) — Historical sessions inside a room.
- [100ms Stream Keys API](https://apis.io/apis/100ms-live/100ms-live-stream-keys-api/) — Per-room RTMP ingest stream keys.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/100ms-live/](https://apis.io/graphqls/100ms-live/100ms-live-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [100Ms Live Agentic Access](https://apis.io/agentic-access/100ms-live/100ms-live-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [100ms Recording](https://apis.io/schemas/100ms-live/100ms-live-recording/)
- [100ms Room](https://apis.io/schemas/100ms-live/100ms-live-room/)
- [100ms Webhook Event](https://apis.io/schemas/100ms-live/100ms-live-webhook-event/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [100Ms Live Room Structure](https://apis.io/json-structure/100ms-live/100ms-live-room-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [100Ms Live Context](https://apis.io/jsonld/100ms-live/100ms-live-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [100Ms Live Vocabulary](https://apis.io/vocabularies/100ms-live/100ms-live-vocabulary/)

#### Examples (3)

Example requests and responses.

- [100Ms Live Create Room Example](https://apis.io/examples/100ms-live/100ms-live-create-room-example/)
- [100Ms Live Start Live Stream Example](https://apis.io/examples/100ms-live/100ms-live-start-live-stream-example/)
- [100Ms Live Webhook Session Open Example](https://apis.io/examples/100ms-live/100ms-live-webhook-session-open-example/)

#### Collections (25)

Postman and Open Collection request collections.

- [100ms Server-Side Active Rooms API](https://apis.io/collections/100ms-live/open-100ms-live-active-rooms-api/)
- [100ms Server-Side Active Rooms Analytics API](https://apis.io/collections/100ms-live/open-100ms-live-analytics-api/)
- [100ms Server-Side Active Rooms External Streams API](https://apis.io/collections/100ms-live/open-100ms-live-external-streams-api/)
- [100ms Server-Side Active Rooms Live Streams API](https://apis.io/collections/100ms-live/open-100ms-live-live-streams-api/)
- [100ms Server-Side Active Rooms Policy API](https://apis.io/collections/100ms-live/open-100ms-live-policy-api/)
- [100ms Server-Side Active Rooms Polls API](https://apis.io/collections/100ms-live/open-100ms-live-polls-api/)
- [100ms Server-Side Active Rooms Recording Assets API](https://apis.io/collections/100ms-live/open-100ms-live-recording-assets-api/)
- [100ms Server-Side Active Rooms Recordings API](https://apis.io/collections/100ms-live/open-100ms-live-recordings-api/)
- [100ms Server-Side Active Rooms Room Codes API](https://apis.io/collections/100ms-live/open-100ms-live-room-codes-api/)
- [100ms Server-Side Active Rooms API](https://apis.io/collections/100ms-live/open-100ms-live-rooms-api/)
- [100ms Server-Side API](https://apis.io/collections/100ms-live/open-100ms-live-server-side-api/)
- [100ms Server-Side Active Rooms Sessions API](https://apis.io/collections/100ms-live/open-100ms-live-sessions-api/)
- [100ms Server-Side Active Rooms Stream Keys API](https://apis.io/collections/100ms-live/open-100ms-live-stream-keys-api/)
- [100ms Server-Side Active Rooms API](https://apis.io/collections/100ms-live/postman-100ms-live-active-rooms-api/)
- [100ms Server-Side Active Rooms Analytics API](https://apis.io/collections/100ms-live/postman-100ms-live-analytics-api/)
- [100ms Server-Side Active Rooms External Streams API](https://apis.io/collections/100ms-live/postman-100ms-live-external-streams-api/)
- [100ms Server-Side Active Rooms Live Streams API](https://apis.io/collections/100ms-live/postman-100ms-live-live-streams-api/)
- [100ms Server-Side Active Rooms Policy API](https://apis.io/collections/100ms-live/postman-100ms-live-policy-api/)
- [100ms Server-Side Active Rooms Polls API](https://apis.io/collections/100ms-live/postman-100ms-live-polls-api/)
- [100ms Server-Side Active Rooms Recording Assets API](https://apis.io/collections/100ms-live/postman-100ms-live-recording-assets-api/)
- [100ms Server-Side Active Rooms Recordings API](https://apis.io/collections/100ms-live/postman-100ms-live-recordings-api/)
- [100ms Server-Side Active Rooms Room Codes API](https://apis.io/collections/100ms-live/postman-100ms-live-room-codes-api/)
- [100ms Server-Side Active Rooms API](https://apis.io/collections/100ms-live/postman-100ms-live-rooms-api/)
- [100ms Server-Side Active Rooms Sessions API](https://apis.io/collections/100ms-live/postman-100ms-live-sessions-api/)
- [100ms Server-Side Active Rooms Stream Keys API](https://apis.io/collections/100ms-live/postman-100ms-live-stream-keys-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [100ms — jsonschema rules](https://apis.io/rules/100ms-live/100ms-live-jsonschema-spectral-rules/)
- [100ms API Rules](https://apis.io/rules/100ms-live/100ms-live-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [100Ms Live Authentication](https://apis.io/security/100ms-live/100ms-live-authentication/)
- [100Ms Live Domain Security](https://apis.io/security/100ms-live/100ms-live-domain-security/)
- [100Ms Live Trust Center](https://apis.io/security/100ms-live/100ms-live-trust-center/)
- [100Ms Live Vulnerability Disclosure](https://apis.io/security/100ms-live/100ms-live-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [100Ms Live Plans Pricing](https://apis.io/plans/100ms-live/100ms-live-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [100Ms Live Rate Limits](https://apis.io/rate-limits/100ms-live/100ms-live-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [100Ms Live Finops](https://apis.io/finops/100ms-live/100ms-live-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.100ms.live/)
- [Documentation](https://www.100ms.live/docs/)
- [Pricing](https://www.100ms.live/pricing)
- [Blog](https://www.100ms.live/blog)
- [Status](https://status.100ms.live/)

## API Evangelist rating

**Kin Score 49.5** — developing · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 54.4 |
| Contract governance | 27.3 |
| Operational transparency | 28.9 |
| Developer ergonomics | 54.8 |
| Access clarity | 39.5 |

**Agent readiness 19.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 27.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/100ms-live/](https://apis.io/providers/100ms-live/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for 100ms: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/100ms-live/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
