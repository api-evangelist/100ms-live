# 100ms (100ms-live)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/apis.yml)

## Tags

- Live Video
- Live Streaming
- Video Conferencing
- WebRTC
- HLS
- RTMP
- Recording
- Real-time Messaging
- Live Infrastructure
- India

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### 100ms Server-Side API

The 100ms Server-Side API is the unified REST control plane for the 100ms live video platform. It manages rooms (the persistent containers for a live session), templates and roles (policy), active rooms and peers (in-session control like kick/mute/message), recordings (composite and per-track), live streams (HLS output and RTMP ingest stream keys), external streams (push to YouTube/Twitch/Facebook Live), recording assets, room codes, polls, sessions, and an analytics API for querying webhook events, track events, recording events, error events, and peer quality stats. Authentication uses a short-lived management JWT (HS256) signed with an app access key + secret pair issued from the dashboard.

- **Human URL:** [https://www.100ms.live/docs/server-side/v2/foundation/basics](https://www.100ms.live/docs/server-side/v2/foundation/basics)
- **Base URL:** `https://api.100ms.live/v2`

#### Tags

- Rooms
- Sessions
- Recordings
- Live Streams
- RTMP
- HLS
- Webhooks
- Polls
- Templates
- Analytics

#### Properties

- [Documentation](https://www.100ms.live/docs/server-side/v2/foundation/basics)
- [Documentation](https://www.100ms.live/docs/server-side/v2/foundation/authentication-and-tokens)
- [OpenAPI](openapi/100ms-live-server-side-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/100ms-live-server-side-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/100ms-live-server-side-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman](https://www.100ms.live/docs/server-side/v2/how-to-guides/set-up-postman) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [SDK](https://github.com/100mslive/server-sdks)

## Common Properties

- [Portal](https://www.100ms.live/)
- [Documentation](https://www.100ms.live/docs/)
- [Sign Up](https://dashboard.100ms.live/register)
- [Dashboard](https://dashboard.100ms.live/)
- [Pricing](https://www.100ms.live/pricing)
- [Git Hub](https://github.com/100mslive)
- [Status Page](https://status.100ms.live/)
- [Blog](https://www.100ms.live/blog)
- [Postman](https://www.100ms.live/docs/server-side/v2/how-to-guides/set-up-postman) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Twitter](https://twitter.com/100mslive)
- [LinkedIn](https://www.linkedin.com/company/100mslive/)
- [SDK](https://github.com/100mslive/web-sdks)
- [SDK](https://github.com/100mslive/100ms-ios-sdk)
- [SDK](https://github.com/100mslive/100ms-android)
- [SDK](https://github.com/100mslive/100ms-react-native)
- [SDK](https://github.com/100mslive/100ms-flutter)
- [SDK](https://github.com/100mslive/server-sdks)
- [Samples](https://github.com/100mslive/100ms-examples)
- [Plans](plans/100ms-live-plans-pricing.yml)
- [Rate Limits](rate-limits/100ms-live-rate-limits.yml)
- [Fin Ops](finops/100ms-live-finops.yml)
- [JSON Schema](json-schema/100ms-live-room-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/100ms-live-recording-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/100ms-live-webhook-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/100ms-live-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/100ms-live-vocabulary.yml)
- [Spectral Rules](rules/100ms-live-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
