<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="260" />
</p>

<h1 align="center">CollectiVAI App (Alpha)</h1>
<h3 align="center">Democratic AI Companion & Civic Client</h3>

<p align="center">
  iOS · iPadOS · macOS · SwiftUI
</p>

---

## Overview

The **CollectiVAI App** is the client application for CollectiVAI –  
a democratic, human-centred AI project with a European focus.

The app is designed to:

- help people **understand** proposals and policies with AI assistance,
- support **discussion and participation** (citizens, experts, institutions),
- and later act as a **full client of the CollectiVAI Chain**  
  (a Cosmos-based governance App-Chain, developed in a separate repository).

This repository contains the **Xcode project** for the iOS / iPadOS / macOS app.

---

## Status

- ✅ Concept & public business plan
- ✅ Initial Xcode project (SwiftUI, basic structure)
- ✅ Roadmap for Alpha → Beta → Chain Phase
- ⏳ AI provider router (multi-model)
- ⏳ Civic participation features (off-chain Beta)
- ⏳ Cosmos App-Chain integration (devnet / testnet)
- ⏳ App Store launch (TBD, depends on pilots & governance)

---

## Roadmap & Feature Stages

The CollectiVAI App will evolve in three main stages:

### 🔹 Alpha – AI Companion & Concept App (current stage)

**Focus:** Local AI assistant and concept prototype for democratic decision-making.

Planned / current features:

- Topic explorer for democracy, civic tech and policy questions
- Chat-based interface with an AI assistant (Q&A, explanations, summaries)
- Simple proposal view:
  - title, description, background
  - AI-generated explanation in simple language
- Pro / contra helper:
  - AI suggests arguments for and against a proposal
- Basic app structure:
  - iOS / iPadOS / macOS (SwiftUI, Xcode)
  - initial navigation and screen layout
- Integration with the public business / strategy docs:
  - links to CollectiVAI website and GitHub organization

> **Goal of the Alpha:** show how AI can help people **understand** and **discuss** proposals.

---

### 🔹 Beta – Civic Participation App (off-chain)

**Focus:** turn the app into a real participation tool, still **off-chain** (no Cosmos connection yet).

Planned features:

- User roles (concept level):
  - Citizen view
  - Expert view
  - Institution / organization view
- Proposal lifecycle:
  - draft → discussion → (simulated) vote → result
- Expert & comment mode:
  - experts can add comments / annotations
  - AI summarizes expert perspectives
- Insights & reports:
  - AI-generated summaries of discussions
  - simple impact / risk overview for proposals
- Local “what-if” simulations:
  - users can ask the AI to explore consequences of different outcomes
- Basic settings:
  - language selection (DE/EN first)
  - topic preferences (e.g. housing, climate, digital, health)

> **Goal of the Beta:** show how CollectiVAI can be used as a
> **participation and analysis app**, even before the blockchain infrastructure is live.

---

### 🔹 Chain Phase – Cosmos App-Chain Integration

**Focus:** connect the app to the **CollectiVAI Chain** (Cosmos-based App-Chain).

Planned features:

- Connect to CollectiVAI devnet / testnet:
  - RPC endpoint selection (e.g. `collectivai-devnet-1`)
- On-chain proposals:
  - create proposals as on-chain transactions
  - show on-chain status and proposal IDs
- On-chain voting:
  - users can cast votes via the app (transaction signing flow)
  - display of on-chain vote results
- Role-aware UI:
  - different actions / views depending on the user’s role
    (citizen, expert, institution – as defined by the chain)
- Governance transparency:
  - timeline for each proposal (created → voting → decided)
  - links to block explorer / transaction details
- Network awareness:
  - show which network is used (local devnet, public testnet, future mainnet)

> **Goal of the Chain Phase:** turn the CollectiVAI App into a **full client for the CollectiVAI Chain**,  
> where democratic decisions are not only discussed, but also **recorded and executed on-chain**.

---

## Relation to the CollectiVAI Chain

This app is designed as the primary client for the **CollectiVAI Chain**  
(a Cosmos-based App-Chain developed in a separate repository):

- Chain repo: [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

The app can already be developed and tested in **Alpha** and **Beta** stages  
without a running chain. Later, the Chain Phase will add full on-chain governance support.

---

## Future Levels – Beyond the Chain Phase

After the initial Alpha, Beta and Chain phases, the CollectiVAI App is planned to grow into
a full civic ecosystem. The following levels are conceptual building blocks for that evolution.

### 🔹 Level 4 – AI Governance Layer

**Focus:** use AI not only as a helper, but as a **governance companion**.

Planned ideas:

- AI checks for each proposal / vote:
  - highlight potential risks, blind spots and affected groups
  - point out unclear or ambiguous wording
- Multiple AI perspectives per proposal:
  - legal, economic, social, privacy-focused views (via different providers / prompts)
- AI audit log:
  - keep track of which AI analyses were used before or during a decision
  - later link these analyses to on-chain proposals and votes

### 🔹 Level 5 – Spaces & Multi-Tenant Support

- Separate spaces for cities, NGOs, universities, projects
- Per-space roles and rules (voting duration, quorums, thresholds)
- Later configurable and enforceable via the CollectiVAI Chain

### 🔹 Level 6 – Civic Data & Privacy Hub

- Personal civic profile (topics, accessibility, language) with full user control
- Optional anonymised data donation for research and democratic innovation
- Transparent data paths: which AI provider was used for which task

### 🔹 Level 7 – Lab & Simulation Mode

- Experimental voting methods (approval voting, ranked choice, liquid democracy)
- “What-if” simulations for different outcomes and parameters
- Clearly separated from real governance flows on the chain

These future levels are intentionally long-term and exploratory.
They are meant to guide the evolution of the CollectiVAI App beyond
a single use case – towards a full civic infrastructure client.

---

## Architecture (high level)

The Xcode project is structured as a SwiftUI app:

- **Targets / platforms**
  - iOS
  - iPadOS
  - macOS (Catalyst or native, depending on configuration)

- **Planned layers**
  - **UI layer** – SwiftUI views (topics, proposals, chat, insights)
  - **View models** – state management for screens and flows
  - **AI provider router** – routes prompts to different AI providers
  - **Chain client (planned)** – HTTP/gRPC client for the CollectiVAI Chain
  - **Settings & storage** – local preferences, drafts, cached data

As the project evolves, a dedicated `docs/` folder may contain:

- `01-overview.md` – app overview & roles  
- `02-architecture.md` – technical structure & modules  
- `03-roadmap.md` – detailed milestones for Alpha / Beta / Chain Phase  

---

## Related repositories

- **Cosmos App-Chain (backend):**  
  [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

- **Main website & public docs:**  
  [`collectiv-ai.github.io`](https://github.com/collectiv-ai/collectiv-ai.github.io)

- **Business plan & strategy:**  
  [`collectiv-ai-business`](https://github.com/collectiv-ai/collectiv-ai-business)

- **Branding & visual identity:**  
  [`collectiv-ai-branding`](https://github.com/collectiv-ai/collectiv-ai-branding)
