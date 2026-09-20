# Awesome-Game-Live-Operations

Top Game LiveOps Platforms Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Live Service Management, Player Engagement, Remote Configuration & Real-Time Operations
Last updated: September 2026

This repository tracks notable SaaS platforms and open-source projects for Game Live Operations (LiveOps). These tools help game studios manage live services, deploy content updates without client patches, run in-game events, segment players, and maintain real-time multiplayer communication.

Examples include Unity Vivox, Unity Remote Config, Beamable, Pragma Platform, PlayFab LiveOps, AccelByte, LootLocker, OneSignal, Airship, and Leanplum (the category leaders).

Open-source emphasis: This section is heavily expanded with every major active project for self-hosting, custom live service pipelines, and transparent player data handling — ideal for indie studios, mid-sized developers, and teams that need full control over their live game infrastructure without per-player SaaS pricing.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

How to Contribute

Disclaimer

SaaS/Hosted Platforms

Unity Vivox
Unity's managed voice and text chat service for multiplayer games. Provides 2D and 3D positional voice channels, direct message text, channel rosters with speaking indicators, mute controls, and concurrency monitoring.

Unity Remote Config
Cloud service for tuning and customizing games without client updates. Supports feature flagging, staged rollouts, kill switches, start/end dates, real-time player segmentation, and A/B testing.

Beamable
Open-core LiveOps platform for Unity and Unreal. Provides player data management, live events, content creation, custom cloud code (C# microservices), and a marketplace of plug-in components. Backed by AWS with over 30 million players served -
11
.

Pragma Platform
Cross-platform identity and player account backend. Unified API for Steam, Epic, PlayStation, Xbox, Discord, and more. Features rate-limited logins, account bans, GDPR-compliant PII handling, and playtest management.

PlayFab LiveOps
Microsoft's complete backend platform for games. LiveOps capabilities include player segmentation, A/B experimentation, title data management, push notifications, cheat prevention, CloudScript server logic, and task scheduling for events and messaging.

AccelByte
Fully managed, modular backend for online and multiplayer games. Services span identity, cloud save, achievements, leaderboards, store/catalog, wallets, social features, chat, matchmaking, and sessions. Provides SDKs for Unreal, Unity, and web.

LootLocker
Game backend platform with open-source SDKs for Unity and Unreal. Features guest, platform, and white-label authentication, player progression, inventories, and cross-platform saves.

OneSignal
Push notification and customer engagement platform. Widely used for re-engagement campaigns, event announcements, and player messaging across mobile and web.

Airship
Customer engagement platform with push notifications, in-app messaging, and automation. Used by game studios for player retention and live event promotion.

Leanplum
Mobile engagement and marketing automation platform (now part of CleverTap). Provides player segmentation, A/B testing, and personalized messaging for live games.

Open-Source GitHub Projects

Nakama
The most mature open-source game backend server. Provides user accounts, chat, social features, matchmaker, real-time multiplayer, and leaderboards. Battle-tested at scale and actively maintained by Heroic Labs. Official AWS GameLift partner with deep integration -
17
. License: Apache 2.0.

Satori
Open-source LiveOps server for games, designed to work alongside Nakama. Features activity scheduling on an Event Calendar, player Audiences for segmentation, Feature Flags, and Experiments for A/B testing. Provides SDKs for Unity, Unreal, and server-side languages -
13
.

Namazu Elements
Self-hosted backend runtime for connected games with REST/WebSocket APIs. Built-in game backend services (auth, matchmaking, leaderboards, inventory) and extensibility via Custom Elements written in any JVM language. Includes a built-in LiveOps CMS for configuring quests, events, and items without code deployments. OpenAPI-first with generated client SDKs. License: MPL-2.0 (moved from AGPLv3 in v3.8) -
7
-
11
.

Globio
Serverless game backend built on Cloudflare's edge network. Ten services including GlobalDoc (edge database), GlobalSync (real-time multiplayer), GlobalVault (cloud saves), GlobalPulse (live configuration/feature flags), Globio ID (cross-platform auth), and GlobalBrain (edge AI inference). Firebase-compatible APIs for migration -
5
.

Open Game Backend (OpenGB)
Open-source backend engine designed as a response to PlayFab and Unity Gaming Services rigidity. Modular architecture where auth, tokens, rate limiting, and game logic are all forkable modules. Built on PostgreSQL with type-safe client SDKs and OpenAPI spec generation. Supports Deno, NodeJS, and Cloudflare Workers -
12
.

Asobi
Open-source game backend built on Erlang/OTP and the Nova ecosystem. Features authentication, player management, real-time multiplayer with WebSocket transport, matchmaking, leaderboards, virtual economy, social features, tournaments, cloud saves, and background jobs. Can be scripted in Lua via Docker or Erlang for full control -
3
.

CrateBytes
Open-source, self-hosted backend solution for games positioned as an alternative to AccelByte. Built with Svelte. Early-stage but active -
6
.

4Players ODIN
Reliable cross-platform SDK for real-time VoIP chat technology in games, apps, and websites. Voice data handled via datagram callbacks with channel masks for routing. Event-driven architecture with room lifecycle management -
1
.

UniVoice
Voice chat/VoIP solution for Unity. Networking-agnostic with built-in support for Mirror and Netcode for GameObjects. Features Opus encoding, RNNoise-based noise removal, and energy-based voice activity detection. MIT licensed.

Talknado
Lightweight combined client-server for real-time voice chat and screen sharing. All control and media packets encrypted. Signaling via TCP, low-latency audio/screen via LiteNetLib (UDP). H.264 encoding via FFmpeg.AutoGen, audio via NAudio with RNNoise noise suppression -
9
.

Nona Config
Open-source self-hosted remote configuration and feature flag service, positioned as a Firebase Remote Config alternative. Embedded web UI, HTTP API, and bundled libSQL database. Supports standalone and primary/replica deployments. Docker image available -
2
-
10
.

Flagsmith
Open-source feature flag, remote config, and A/B testing service. Self-host or use hosted API. Provides SDKs for Node.js, Java, Ruby, PHP, JavaScript, Rust, and more. BSD-3-Clause licensed -
15
.

Dittofeed
Open-source customer engagement platform for omni-channel messaging. Send broadcasts or automated user journeys via email, push notifications, SMS, WhatsApp, and Slack. Dev-friendly alternative to OneSignal and Customer.io. Self-hostable to keep PII in your own VPC. MIT licensed -
8
.

Additional Strong Open-Source Options

Real-Time Voice: LiveKit (self-hosted WebRTC infrastructure for voice/video), mediasoup (SFU for multi-party audio), Janus (general-purpose WebRTC gateway) -
14
.

Remote Config & Flags: Nona (Firebase Remote Config alternative), Flagsmith (feature flags + remote config + A/B testing), OpenFeature (vendor-neutral flag SDK standard).

Engagement & Messaging: Dittofeed (omni-channel journeys, push, email, SMS), Novu (open-source notification infrastructure for in-app, email, SMS, push).

Game Backend Foundations: Nakama (battle-tested, enterprise-ready), Namazu Elements (self-hosted runtime with LiveOps CMS), OpenGB (modular, forkable architecture).

Frameworks for building custom systems: Combine Nakama for core backend services (accounts, chat, matchmaking), Satori for LiveOps event scheduling and feature flags, 4Players ODIN or UniVoice for in-game voice chat, Dittofeed for player engagement messaging, and PostgreSQL + Redis for persistence. Deploy via Docker Compose for a complete self-hosted stack.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

Game LiveOps platforms handle player data and real-time communications; ensure compliance with platform requirements (Steam, Xbox, PlayStation) and data protection regulations.

Self-hosted open-source solutions require proper security hardening, scaling strategy, and operational monitoring.

Made for game developers, live operations producers, backend engineers, and studio technical directors.
Let's make game LiveOps more open, scalable, and player-focused.
