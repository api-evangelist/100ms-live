# 100ms (100ms-live)

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
