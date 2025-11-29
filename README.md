<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
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
- Integration with public docs:
  - links to the CollectiVAI website and GitHub organisation

> **Goal of the Alpha:** show how AI can help people **understand**  
> and **discuss** proposals and policy ideas.

---

### 🔹 Beta – Civic Participation App (off-chain)

**Focus:** turn the app into a real participation tool, still **off-chain**  
(no Cosmos integration yet).

Planned features:

- User roles (concept level):
  - Citizen view
  - Expert view
  - Institution / organisation view
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
> **participation and analysis app**, even before the blockchain is live.

---

### 🔹 Chain Phase – Cosmos App-Chain Integration

**Focus:** connect the app to the **CollectiVAI Chain**  
(a Cosmos-based App-Chain developed in [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)).

Planned features:

- Connect to CollectiVAI devnet / testnet:
  - RPC endpoint selection (e.g. `collectivai-devnet-1`)
- On-chain proposals:
  - create proposals as on-chain transactions
  - show on-chain status and proposal IDs
- On-chain voting:
  - cast votes via the app (transaction signing flow)
  - display on-chain vote results
- Role-aware UI:
  - different actions / views depending on the user’s role
    (citizen, expert, institution – as defined by the chain)
- Governance transparency:
  - timeline for each proposal (created → voting → decided)
  - links to block explorer / transaction details
- Network awareness:
  - show which network is used (local devnet, public testnet, future mainnet)

> **Goal of the Chain Phase:** turn the CollectiVAI App into a  
> **full client for the CollectiVAI Chain**, where decisions are not only  
> discussed, but also **recorded and executed on-chain**.

---

## Future Levels – Beyond the Chain Phase

After the initial Alpha, Beta and Chain phases, the app is planned to grow into
a full civic ecosystem. Some conceptual building blocks:

### 🔹 Level 4 – AI Governance Layer

- AI checks for each proposal / vote (risks, blind spots, unclear wording)
- multiple AI perspectives (legal, economic, social, privacy-focused)
- AI audit log: document which AI analyses influenced which decisions

### 🔹 Level 5 – Spaces & Multi-Tenant Support

- separate **spaces** for cities, NGOs, universities, projects
- per-space roles and rules (voting duration, quorums, thresholds)
- later configurable and enforceable via the CollectiVAI Chain

### 🔹 Level 6 – Civic Data & Privacy Hub

- personal civic profile (topics, accessibility, language) with full control  
- optional **data donation** for research (anonymised)
- transparent data paths: which AI provider was used for which task

### 🔹 Level 7 – Lab & Simulation Mode

- experimental voting methods (approval voting, ranked choice, liquid democracy)
- “what-if” simulations for different outcomes and parameters
- clearly separated from real on-chain governance flows

These future levels are intentionally long-term and exploratory.  
They guide the evolution of the app beyond a single use case.

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

(analogous to the documentation in the Chain repository).

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
