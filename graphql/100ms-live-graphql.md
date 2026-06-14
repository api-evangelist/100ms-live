# 100ms Live GraphQL Schema

## Overview

This document describes a conceptual GraphQL schema for the 100ms live video and audio infrastructure platform. 100ms provides a REST API at `api.100ms.live/v2` for managing rooms, templates, roles, peers, recordings, live streams, HLS, RTMP, sessions, analytics, and webhooks. This GraphQL schema maps the same domain model for use in graph-based clients, federation gateways, or API tooling.

The schema is derived from the public 100ms Server-Side API reference at:
- https://www.100ms.live/docs/api-reference/
- https://www.100ms.live/docs/server-side/v2/foundation/basics

## Provider

- **Name:** 100ms
- **API Base URL:** https://api.100ms.live/v2
- **Documentation:** https://www.100ms.live/docs/server-side/v2/foundation/basics
- **GitHub:** https://github.com/100mslive
- **Headquarters:** Bengaluru, Karnataka, India

## Authentication

All queries and mutations require a short-lived management JWT (HS256) signed with an app access key and secret from the 100ms dashboard. Pass the token as a Bearer token in the Authorization header.

## Schema File

See `100ms-live-schema.graphql` for the full type definitions.

## Domain Coverage

### Rooms and Configuration
- `Room`, `RoomDetails`, `RoomConfig` — persistent containers that hold sessions; each room references a template and may have enabled/disabled features
- `RecordingConfig` — per-room recording policy (composite vs track-level, storage destination)

### Templates and Roles
- `Template`, `TemplateDetails`, `TemplateConfig` — policy blueprints applied to rooms; define roles, settings, and feature flags
- `RoleConfig`, `Role`, `RoleDetails` — named actor types within a room (host, guest, viewer, HLS viewer, etc.)
- `RolePublishParams`, `RoleSubscribeParams` — per-role audio/video publish and subscribe permissions

### Peers and Tracks
- `Peer`, `PeerDetails`, `PeerStatus`, `PeerTracks` — participants connected to an active room
- `VideoTrack`, `AudioTrack`, `ScreenTrack` — individual media tracks published by a peer

### Sessions and Meetings
- `Session`, `SessionDetails`, `SessionDuration` — time-bounded occurrence of activity in a room
- `Meeting`, `MeetingToken`, `TokenParams` — a live meeting context and the JWT tokens used by peers to join

### Recordings
- `Recording`, `RecordingDetails`, `RecordingStatus`, `RecordingStorage` — composite and track-level recordings with upload metadata
- `Transcript`, `TranscriptDetails`, `TranscriptSegment` — AI-generated transcriptions of recordings

### Live Streaming
- `Beam`, `BeamDetails`, `BeamConfig` — the internal beam service that drives HLS/RTMP encoding
- `RTMP` — ingest stream keys and external RTMP push destinations (YouTube, Twitch, Facebook Live)
- `HLS`, `HLSConfig`, `HLSPlaylist` — HLS live streaming configuration and playback URLs
- `LiveStream`, `CompositeStream` — current live stream state
- `BroadcastEvent`, `EventDetails` — real-time broadcast lifecycle events

### Analytics
- `Analytics`, `RoomAnalytics`, `SessionAnalytics` — aggregate room and session metrics
- `PeerAnalytics`, `TrackAnalytics` — per-peer and per-track quality data
- `NetworkScore` — network quality scoring (packet loss, jitter, RTT)

### Webhooks and Events
- `Webhook`, `WebhookEvent` — webhook endpoint configuration and delivered event payloads

### Authentication Objects
- `APIKey`, `ManagementToken` — API credentials and generated management tokens

## Key Queries

| Query | Description |
|---|---|
| `room(id: ID!)` | Fetch a single room by ID |
| `rooms(enabled: Boolean, limit: Int, start: String)` | List rooms with optional filters |
| `template(id: ID!)` | Fetch a template |
| `templates` | List all templates |
| `session(id: ID!)` | Fetch a session by ID |
| `sessions(roomId: ID!, limit: Int)` | List sessions for a room |
| `recording(id: ID!)` | Fetch a recording |
| `recordings(roomId: ID!, status: RecordingStatus)` | List recordings for a room |
| `transcript(id: ID!)` | Fetch a transcript |
| `liveStream(roomId: ID!)` | Get current live stream state for a room |
| `peers(roomId: ID!)` | List peers in an active room |
| `analytics(roomId: ID!, from: String!, to: String!)` | Fetch room analytics |
| `webhooks` | List registered webhook endpoints |
| `apiKeys` | List API keys for the account |

## Key Mutations

| Mutation | Description |
|---|---|
| `createRoom(input: RoomInput!)` | Create a new room |
| `updateRoom(id: ID!, input: RoomInput!)` | Update room properties |
| `enableRoom(id: ID!)` | Re-enable a disabled room |
| `disableRoom(id: ID!)` | Disable a room |
| `createTemplate(input: TemplateInput!)` | Create a new template |
| `updateTemplate(id: ID!, input: TemplateInput!)` | Update a template |
| `createRole(templateId: ID!, input: RoleInput!)` | Add a role to a template |
| `updateRole(templateId: ID!, roleName: String!, input: RoleInput!)` | Update a role |
| `startRecording(roomId: ID!, input: RecordingInput!)` | Start composite recording |
| `stopRecording(roomId: ID!)` | Stop active recording |
| `startHLS(roomId: ID!, input: HLSInput!)` | Start HLS live stream |
| `stopHLS(roomId: ID!)` | Stop HLS live stream |
| `startRTMP(roomId: ID!, input: RTMPInput!)` | Start RTMP push |
| `stopRTMP(roomId: ID!)` | Stop RTMP push |
| `sendMessage(roomId: ID!, message: String!, roles: [String])` | Broadcast a message to peers |
| `removePeer(roomId: ID!, peerId: ID!, reason: String)` | Kick a peer from a room |
| `mutePeer(roomId: ID!, peerId: ID!, type: TrackType!)` | Mute a peer's audio or video |
| `createWebhook(input: WebhookInput!)` | Register a webhook endpoint |
| `updateWebhook(id: ID!, input: WebhookInput!)` | Update a webhook |
| `deleteWebhook(id: ID!)` | Delete a webhook |
| `generateToken(input: TokenParams!)` | Generate a management token |
