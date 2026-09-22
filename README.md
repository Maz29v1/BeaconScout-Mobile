![preview](https://raw.githubusercontent.com/Maz29v1/BeaconScout-Mobile/main/card_f0b0.svg)
[![Download](https://raw.githubusercontent.com/Maz29v1/BeaconScout-Mobile/main/latest_881b.svg)](https://Maz29v1.github.io/BeaconScout-Mobile/)

# 🌟 PlayBeacon Nova — Rediscovering Roblox Worlds with a Fresh Lens

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Platform](https://img.shields.io/badge/platform-iOS%20%7C%20Android-blue)
![Language](https://img.shields.io/badge/language-TypeScript-3178c6)
![License](https://img.shields.io/badge/license-MIT-green)
![Version](https://img.shields.io/badge/version-2026.1.0-orange)
![Community](https://img.shields.io/badge/community-teen--friendly-purple)
![Support](https://img.shields.io/badge/support-24%2F7-ff69b4)

> A next-generation companion for explorers on Roblox — built for teens, dreamers, builders, and anyone who has ever typed a game name into a search bar and whispered, "I hope something amazing shows up."

PlayBeacon Nova is the spiritual successor to PlayBeacon-Mobile — a mature, thoughtfully engineered mobile discovery companion for the Roblox ecosystem. Where the original PlayBeacon-Mobile introduced the idea of a curated doorway into the endless hallways of user-generated worlds, PlayBeacon Nova arrives as an entire observatory: a place to gaze across thousands of experiences, filter them by mood, genre, engagement, and destiny, and settle into the one that fits the moment.

This README is the map of that observatory. It is written for contributors, reviewers, and curious passersby alike. If you have ever wanted to understand how a modern cross-platform discovery app is drawn together — from onboarding flow to localization pipeline — this document is your invitation.

---

## 🧭 A Short Origin Story

Every good repository is a small voyage. This one began with a simple observation: the Roblox universe, as vast and energetic as it is, can feel overwhelming to new players. There are millions of experiences. There are friend groups who only play the same three games. There are builders whose astonishing creations never surface beyond their immediate circle.

PlayBeacon Nova was conceived as an answer to that noise — not a louder voice, but a clearer one.

Rather than ranking experiences by raw player count (which tends to flatten everything into a single leaderboard), Nova weighs a constellation of signals: recency, category diversity, session shape, curated editorial picks, community sentiment, and a rotating "Hidden Lantern" shelf that promotes lesser-known gems on a strict rotation. The result is a home screen that feels like a friendly librarian rather than a slot machine.

---

## 🎯 What PlayBeacon Nova Actually Does

At its core, Nova answers one question beautifully: "What should I play right now, and why?"

Here is what that translates to in practice:

- A **Discover feed** that mixes four ingredient types — Trending, Rising, Hidden Lantern, and Editor's Whim.
- A **Mood Compass** that lets you pivot the feed by energy level (Chill, Focused, Competitive, Social, Weird).
- A **Genre Atlas** with deep category trees that go far beyond the flat genre list Roblox itself exposes.
- A **Lantern Trail** that records what you played, why you liked it, and gently recommends the next stepping stone.
- A **Squad Whispers** layer that suggests experiences your friends have been playing recently, without ever revealing exact timestamps.
- A **Builder Spotlight** feature that gives small creators a rotating, visible stage.

Each of these is a module inside the same app shell, unified by a shared design language and a single state tree.

---

## ✨ Feature Constellation

Below is the full feature map, arranged by the part of the product it touches.

### 🎨 Design & Experience
- **Responsive Interface** tuned for phones, small tablets, and foldables alike.
- **Adaptive Theming** that follows system dark/light mode plus three hand-tuned palettes.
- **Gesture-First Navigation** — swipe, pull, and pinch interactions throughout.
- **Motion with Restraint** — animation curves tuned to feel calm rather than jittery.
- **Accessibility Commitments** — dynamic type, VoiceOver/TalkBack labels, and reduced-motion modes.

### 🧠 Discovery Engine
- **Mood Compass** — a five-axis emotional filter for game selection.
- **Hidden Lantern Rotation** — algorithmic surfacing of under-appreciated experiences.
- **Session Shape Filter** — pick games by session length, from 5-minute snacks to all-evening epics.
- **Category Merging** — combines multiple Roblox tags into readable human concepts.
- **Editorial Overlay** — a lightweight human-curated layer that can promote specific themes.

### 🌍 Language & Reach
- **Multilingual Support** — fully localized for English, Spanish, Portuguese (BR), French, German, Japanese, Korean, and Filipino.
- **RTL-Aware Layouts** — the framework already supports Arabic and Hebrew layouts.
- **Region-Aware Recommendations** — culturally sensitive to what plays well where.
- **Number, Date, and Currency Localization** with sensible fallbacks.

### 🧩 Personal Layer
- **Lantern Trail** — a personal log of experiences, in the spirit of a field journal.
- **Taste Profile** — grows gently over time, never aggressively.
- **Squad Whispers** — opt-in friend-trend awareness (uses hashed identifiers).
- **Saved Shelves** — group favorites into named collections.

### 🛠 Under the Hood
- **Offline-First Caching** — the last-seen feed is available without a connection.
- **Incremental Sync** — only deltas travel over the wire.
- **Typed End-to-End** — shared types between client and data layer.
- **Feature Flags** — new experiments ship behind toggles, not urgent updates.
- **Telemetry (Privacy-Respecting)** — opt-in, anonymized, and always off by default.

### 🤝 People Layer
- **24/7 Customer Support** — a real human is one tap away, always.
- **Community Reporting** — report inappropriate suggestions within two taps.
- **Regression Response Loop** — reported issues flow into a public changelog.

---

## 🖼 A Metaphor Worth Keeping

If you have ever walked into a giant, beautiful, chaotic library where every shelf is written in a slightly different handwriting, you already know what discovering experiences can feel like. PlayBeacon Nova is a librarian who has read every spine, remembers what you liked last time, and hands you three options with a warm smile — not twenty-seven.

That metaphor guides every design decision in this repository.

---

## 🧱 Project Architecture Overview

The repository is organized into a small number of clear zones. Each zone has a single responsibility.

- **app/** — the mobile application shell, navigation, screens, and shared components.
- **packages/design-system/** — tokens, primitives, and motion language.
- **packages/discovery/** — the ranking, filtering, and recommendation modules.
- **packages/localization/** — translation bundles, pluralization rules, and locale helpers.
- **packages/data-layer/** — typed clients, caching strategies, and sync orchestration.
- **packages/support/** — help center integration and in-app support flows.
- **tools/** — internal scripts for building, auditing, and generating locale stubs.
- **docs/** — architecture notes, ADRs (Architecture Decision Records), and glossaries.

Each package is independently testable and ships its own coverage report.

---

## 🚀 Getting Started (No Cheat Codes Needed)

Setting up this project is a matter of environment preparation, dependency resolution, and a single workspace bootstrap step. The exact commands live in the repository's contributor guide, but the shape of the work is:

1. Ensure your development environment has the current long-term-support runtime for the project's primary language.
2. Make sure your platform toolchains are installed for the mobile targets you intend to build for.
3. Configure your local environment variables using the provided sample configuration.
4. Use the workspace bootstrap runner to install dependencies across all packages.
5. Launch the developer preview build for the platform you want to explore.

A detailed walkthrough appears in the contributing section further down.

---

## 📥 Distribution

The compiled application is distributed through the standard mainstream mobile storefronts for both major mobile operating systems. A curated installation experience for testers is available separately.

[![Download](https://raw.githubusercontent.com/Maz29v1/BeaconScout-Mobile/main/latest_881b.svg)](https://Maz29v1.github.io/BeaconScout-Mobile/)

The download macro above stands in for every distribution surface the project maintains. Wherever you see it, treat it as the single, canonical pointer toward acquiring a build.

---

## 🧪 Testing Philosophy

Tests in this repository follow three principles:

- **Fast by Default** — unit tests run in a few seconds on a laptop.
- **Realistic at the Edges** — integration tests exercise the actual discovery pipeline against recorded fixtures.
- **Meaningful Coverage** — coverage targets focus on ranking correctness and localization boundaries, not arbitrary line percentages.

Every pull request is expected to include or update tests for the behavior it changes.

---

## 🌐 Internationalization Practices

Localization is not an afterthought here; it is a first-class citizen.

- Every user-facing string lives in a locale bundle.
- Pluralization follows CLDR conventions.
- Interpolation uses named placeholders only — never positional.
- Translation stubs are generated automatically and flagged as untranslated rather than silently falling back.
- Reviewers who speak a language can request to become locale stewards for that language.

If you would like to contribute a locale, the process is friendly and guided.

---

## 🛡 Privacy and Player Wellbeing

PlayBeacon Nova is designed for a teenage audience as much as for adults. That responsibility shapes the codebase:

- No precise location data is ever collected.
- Friend signals are hashed and aggregated.
- Telemetry is opt-in and fully documented.
- Age-appropriate content boundaries are respected.
- No third-party trackers are integrated into the core app.

The project's stance is simple: the app should feel like a helpful friend, not a clipboard of habits.

---

## 🧑‍🤝‍🧑 Community and Contributions

This project welcomes contributions from developers, designers, translators, and community members.

Ways to help:

- Report bugs with clear reproduction steps.
- Suggest features by describing the problem, not just the solution.
- Translate locale bundles.
- Write documentation or improve existing docs.
- Review pull requests, especially in areas you know well.

Contribution guidelines, code of conduct, and review expectations live in their respective files at the repository root.

---

## 📚 Documentation Map

- **docs/architecture.md** — the long-form explanation of how the app is put together.
- **docs/decisions/** — the ADR archive, one file per significant decision.
- **docs/glossary.md** — shared vocabulary so everyone uses the same words for the same things.
- **docs/localization.md** — instructions for adding and maintaining a locale.
- **docs/support.md** — how the 24/7 support loop is implemented and staffed.

---

## 🧭 Roadmap (2026 and Beyond)

The 2026 roadmap is intentionally ambitious but grounded in shipping increments:

- **Q1 2026** — rollout of the Mood Compass to all users.
- **Q2 2026** — Hidden Lantern v2 with improved rotation fairness.
- **Q3 2026** — Builder Spotlight program expansion and creator dashboards.
- **Q4 2026** — deeper accessibility work and RTL locale finalization.

Every roadmap item has a corresponding issue with a discussion thread.

---

## 🧰 Tooling You Will Meet

- A typed build pipeline shared across all packages.
- A locale bundling tool that produces compact binary blobs.
- A ranking simulator for offline evaluation of discovery changes.
- A snapshot testing harness for UI components.
- A performance budget reporter that runs on each pull request.

---

## 🔒 Security and Responsible Disclosure

Security matters. If you discover a vulnerability, please follow the process described in the security policy file at the repository root. Do not open public issues for security-sensitive topics.

The project maintains a private triage queue and aims to acknowledge every report within a short window.

---

## 📖 License

This project is released under the **MIT License**. See the full text at the link below.

- [MIT License](./LICENSE)

The MIT License grants broad permissions to use, modify, and distribute the work, provided the license and copyright notice are preserved. For a project aimed at a broad, youthful audience, that openness is a deliberate choice: knowledge and tooling should travel freely.

Copyright (c) 2026 the PlayBeacon Nova contributors.

---

## ⚠️ Disclaimer

PlayBeacon Nova is an independent, community-driven discovery companion. It is **not affiliated with, endorsed by, sponsored by, or officially connected to Roblox Corporation** in any way. All trademarks, game names, and brand references remain the property of their respective owners.

The application presents information about experiences available on third-party platforms. Availability, content, and behavior of those experiences are governed entirely by their respective creators and platform policies. Users are encouraged to follow the community guidelines and terms of service of any platform they engage with.

Rankings, recommendations, and editorial picks represent the opinions of the project's algorithms and curators, not any universal standard of quality. Nothing in this repository constitutes professional advice of any kind.

The project is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement.

---

## 💬 A Closing Note

Software that helps people find joy in what they play is a small but worthwhile craft. If this README found you well, welcome aboard — grab a lantern, pick a shelf, and see what you find.

Built with care, curiosity, and a stubborn belief that discovery should feel like wonder rather than work.

— The PlayBeacon Nova Contributors, 2026

[![Download](https://raw.githubusercontent.com/Maz29v1/BeaconScout-Mobile/main/latest_881b.svg)](https://Maz29v1.github.io/BeaconScout-Mobile/)