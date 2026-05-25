# 100ms (100ms-live)

100ms is a live video and audio infrastructure company headquartered in Bengaluru, India. The platform provides SDKs for Web, iOS, Android, React Native, and Flutter plus a unified Server-Side REST API (`api.100ms.live/v2`) for video conferencing, interactive HLS live streaming, RTMP ingest and egress, composite recording, real-time messaging, polls, whiteboard, and AI-powered live transcription. 100ms was acquired by Disney+ Hotstar (JioHotstar / JioCinema) in late 2022 and continues to operate as a commercial SaaS — the same infrastructure powers some of the largest live cricket audiences in the world.

**URL:** [Visit APIs.yml URL](https://raw.githubusercontent.com/api-evangelist/100ms-live/refs/heads/main/apis.yml)

## Type
- **x-type:** company

## Headquarters
- Bengaluru, Karnataka, India

## Acquirer
- Disney+ Hotstar (JioHotstar), 2022

## Tags
- Live Video, Live Streaming, Video Conferencing, WebRTC, HLS, RTMP, Recording, Real-time Messaging, Live Infrastructure, India

## APIs
- **100ms Server-Side API** (`https://api.100ms.live/v2`) — single REST control plane for Rooms, Sessions, Active Rooms (in-session control), Policy / Templates / Roles, Recordings, Recording Assets, Live Streams (HLS), External Streams (RTMP push), Stream Keys (RTMP-in), Room Codes, Polls, and Analytics.

## OpenAPI specs (in `openapi/`)
- `100ms-live-server-side-api-openapi.yml`

Source: https://www.100ms.live/docs/server-side/v2/foundation/basics

## JSON Schema (in `json-schema/`)
- `100ms-live-room-schema.json`
- `100ms-live-recording-schema.json`
- `100ms-live-webhook-event-schema.json`

## JSON Structure (in `json-structure/`)
- `100ms-live-room-structure.json`

## JSON-LD (in `json-ld/`)
- `100ms-live-context.jsonld`

## Examples (in `examples/`)
- `100ms-live-create-room-example.json`
- `100ms-live-start-live-stream-example.json`
- `100ms-live-webhook-session-open-example.json`

## Naftiko capabilities (in `capabilities/`)
- `rooms.yaml`
- `active-rooms.yaml`
- `recordings.yaml`
- `live-streams.yaml`
- `external-streams.yaml`
- `policy-templates.yaml`
- `room-codes.yaml`
- `analytics.yaml`

## Spectral rules (in `rules/`)
- `100ms-live-rules.yml`

## Vocabulary (in `vocabulary/`)
- `100ms-live-vocabulary.yml`

## Commercial artifacts
- [Plans](plans/100ms-live-plans-pricing.yml) — Build (free, 10k minutes/mo), Growth, Enterprise
- [RateLimits](rate-limits/100ms-live-rate-limits.yml) — concurrency caps (1k standard rooms, 10k+ large rooms)
- [FinOps](finops/100ms-live-finops.yml) — FOCUS-aligned per-minute meters

## SDKs (open source on GitHub)
- [Web SDKs](https://github.com/100mslive/web-sdks) — JavaScript / React, Prebuilt UI, hooks
- [iOS SDK](https://github.com/100mslive/100ms-ios-sdk) — Swift
- [Android SDK](https://github.com/100mslive/100ms-android) — Kotlin
- [React Native SDK](https://github.com/100mslive/100ms-react-native)
- [Flutter SDK](https://github.com/100mslive/100ms-flutter)
- [Server SDK (Node.js)](https://github.com/100mslive/server-sdks)
- [100ms Examples](https://github.com/100mslive/100ms-examples)

## Common Properties
- [Portal](https://www.100ms.live/)
- [Documentation](https://www.100ms.live/docs/)
- [Dashboard](https://dashboard.100ms.live/)
- [Sign up](https://dashboard.100ms.live/register)
- [Pricing](https://www.100ms.live/pricing)
- [GitHub](https://github.com/100mslive)
- [Status](https://status.100ms.live/)
- [Blog](https://www.100ms.live/blog)
- [Postman setup](https://www.100ms.live/docs/server-side/v2/how-to-guides/set-up-postman)

## Timestamps
- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
