<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
</p>

<h1 align="center">CollectiVAI App</h1>
<h3 align="center">Democratic AI Companion & Civic Client</h3>

<p align="center">
  <a href="https://collectivai.org">
    <img src="https://img.shields.io/badge/Website-collectivai.org-003399?style=flat" alt="Website" />
  </a>
  <a href="https://github.com/collectiv-ai/collectiv-ai-app-chain">
    <img src="https://img.shields.io/badge/Chain-Pre--Alpha-999999?style=flat" alt="Chain Pre-Alpha" />
  </a>
  <img src="https://img.shields.io/badge/Status-Alpha-ffcc00?style=flat" alt="App Alpha" />
  <img src="https://img.shields.io/badge/Made%20in-Europe-003399?style=flat" alt="Made in Europe" />
</p>

---

## Overview

The **CollectiVAI App** is the **client application** for the CollectiVAI ecosystem:  
a democratic, human-centred AI platform with a European focus.

The app acts as an **AI companion** for democracy, policy and civic tech:

- helps people **understand** proposals and policies,  
- supports **discussion, participation and co-creation**  
  (citizens, experts, institutions),  
- is intended to become a **full client for the CollectiVAI Chain**  
  (Cosmos-based App-Chain in a separate repository).

This repository contains the **Xcode project** for iOS / iPadOS / macOS.

---

## Feature areas (current prototype)

The current (alpha / prototype) app is structured into four main tabs:

### 1. Chat

- AI chat focused on topics such as **democracy, climate, economy, security, research, health**  
- **Mode** selection (Ethical · Research · Technical)  
- **Provider** selection (Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek)  
- Transparent routing meta (model used, latency – optional in Developer Mode)

### 2. Contracts

- “Civic Application Hub” for **applications and project drafts**  
- Categories: universities, schools, NGOs, cities, startups, custom  
- **3-step wizard**:
  1. basics (organisation, country, title)  
  2. content & impact (summary, impact, target groups)  
  3. budget & duration (amount, currency, duration, status)  
- All content stays **human-readable** and can later be mirrored to on-chain proposals.

### 3. Chain

- Civic dashboard (concept view, no live network yet)  
- Shows how your applications could later appear as:
  - **on-chain proposals**
  - **votes**
  - **public treasury allocations**  
- Cards/tiles for universities, schools, cities, NGOs, startups, and your impact/reputation.

### 4. Settings & Info

- Default settings (mode, provider, topic)  
- Routing profiles (Balanced, Research-heavy, Code & Security)  
- Text size, haptics, Developer Mode, live monitoring  
- Simple privacy toggles (App Lock, telemetry opt-in, auto-delete planning)  
- “About” screen with explanation and links (website, GitHub organisation).

> **Goal of the current stage:**  
> Provide a **working prototype UI** that demonstrates how a democratic AI app  
> for participation, analysis and governance could feel – before a real chain is live.

---

## Status & roadmap (App)

**Current status:**

- ✅ Core concept & public business plan  
- ✅ Initial Xcode app (SwiftUI, navigation, basic views)  
- ✅ Chat router (multi-provider + mode/topic routing)  
- ✅ Contracts wizard for civic applications  
- ✅ Chain dashboard as a conceptual view  
- ⏳ Integration with real programmes / pilots (cities, universities, NGOs)  
- ⏳ Integration with the CollectiVAI Chain (Cosmos devnet/testnet)  
- ⏳ App Store release (depends on governance & partners)

**Planned phases (short):**

1. **Alpha – AI Companion & Concept App**  
   - Focus: understanding, explanations, pro/con analysis, early civic drafts.

2. **Beta – Civic Participation (off-chain)**  
   - additional roles (citizen, expert, institution)  
   - discussion-based workflows (draft → discussion → “vote” off-chain)  
   - multi-language use (EN + others)

3. **Chain Phase – Full Cosmos App-Chain integration**  
   - connection to `collectivai-devnet` / testnet  
   - on-chain proposals & votes  
   - display of proposal IDs, vote status, treasury movements  
   - the app acts as a **full client of the CollectiVAI Chain**.

---

## Architecture (simplified)

- **Platforms**
  - iOS  
  - iPadOS  
  - macOS (SwiftUI / Catalyst if needed)

- **Layers (planned / partially implemented)**
  - **UI layer** – SwiftUI views (Chat, Contracts, Chain dashboard, Settings)  
  - **State & config** – central `CollectivAIConfig` (providers, modes, topics, projects, applications)  
  - **Backend client** – `CollectivAIBackend` (HTTP client to the router backend)  
  - **Chain client (planned)** – Cosmos client for the CollectiVAI Chain (RPC / REST / gRPC)  
  - **Local storage** – AppStorage, local drafts, future cache/persistence layer

---

## Getting started (for developers)

> The app is currently in **alpha / prototype** state. API contracts and internal
> structure may change as the router and chain evolve.

### Requirements

- Xcode 16+ (or current Xcode with iOS 18 SDK)  
- macOS with SwiftUI support  
- A configured **CollectiVAI Router** endpoint (for real API calls) or the demo router.

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/collectiv-ai/collectiv-ai-app.git
   cd collectiv-ai-app
   ```

2. Open the Xcode project:

   - Open `collectivai.xcodeproj` in Xcode.

3. Select a target & run:

   - Choose the `collectivai` target.  
   - Run on an iOS Simulator, iPad Simulator or a connected Mac Catalyst device.

4. Configure backend URL (optional):

   - In early prototypes, the app may use a simple configuration struct or plist  
     to point to your **CollectiVAI Router** (e.g. `http://localhost:8000/api/chat`).  
   - For production, the router should be available via HTTPS and protected  
     according to your infrastructure.

---

## Relation to CollectiVAI Chain

The CollectiVAI App and the CollectiVAI Chain are tightly connected but serve different roles:

- **CollectiVAI App**  
  - front-end for citizens, experts and institutions  
  - drafts, discussions, local “what-if” analysis  
  - later: on-chain proposal creation & voting

- **CollectiVAI Chain**  
  - neutral governance infrastructure (Cosmos App-Chain)  
  - stores proposals, votes, parameters and roles **on-chain**  
  - ensures auditability and transparency across time

The App lives in this repository,  
the Chain is developed in [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain).

---

## Related repositories

- ⛓ **Cosmos App-Chain (backend):**  
  [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

- 🧠 **AI routing backend (multi-provider):**  
  [`collectiv-ai-router`](https://github.com/collectiv-ai/collectiv-ai-router)

- 🌐 **Main website & public docs:**  
  [`collectiv-ai.github.io`](https://github.com/collectiv-ai/collectiv-ai.github.io)

- 🧭 **Business plan & strategy:**  
  [`collectiv-ai-business`](https://github.com/collectiv-ai/collectiv-ai-business)

- 🎨 **Branding & visual identity:**  
  [`collectiv-ai-branding`](https://github.com/collectiv-ai/collectiv-ai-branding)

- 🤝 **Sponsors & partners:**  
  [`collectiv-ai-sponsors`](https://github.com/collectiv-ai/collectiv-ai-sponsors)

- 👤 **Founder profile & portfolio:**  
  [`collectiv-ai-about-founder`](https://github.com/collectiv-ai-about-founder)

---

## Licences & branding

Source code licences for this repository are defined in the  
`LICENSE` file of this project.

The **CollectiVAI name, logo and visual identity** are protected.  
Any use in products, services or campaigns requires prior written permission.

© David Miecznikowski, CollectiVAI.
