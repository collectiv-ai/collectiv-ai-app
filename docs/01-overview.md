# CollectiVAI App – Overview

## 1. Vision

The **CollectiVAI App** is the client application of the CollectiVAI project –  
a democratic, human-centred AI initiative with a European focus.

The app is designed to:

- help people **understand** complex proposals and policies with AI assistance,
- support **discussion and participation** for citizens, experts and institutions,
- and later act as a **full client** of the Cosmos-based CollectiVAI Chain.

While the CollectiVAI Chain provides the neutral governance infrastructure,
the CollectiVAI App is the main **user-facing interface**.

---

## 2. Role in the Ecosystem

The CollectiVAI App is part of a broader ecosystem:

- **CollectiVAI App (this repository)**  
  - iOS / iPadOS / macOS app (SwiftUI, Xcode)  
  - provides the UI for topics, proposals, discussions and votes  
  - integrates AI providers (router) and, later, the CollectiVAI Chain

- **CollectiVAI Chain**  
  - Cosmos-based App-Chain (separate repository)  
  - stores proposals, votes, parameters and roles on-chain  
  - acts as a neutral, auditable governance layer

- **Public docs & business / strategy**  
  - published in separate repositories under the `collectiv-ai` organisation  
  - define vision, roadmap, governance model and branding

The app can already be developed and tested in **Alpha** and **Beta** stages  
without a running chain. In the **Chain Phase**, it will connect to a devnet /
testnet of the CollectiVAI Chain.

---

## 3. Target Users

The app is intended for:

- **Citizens**  
  - explore topics and proposals  
  - understand arguments and implications with AI help  
  - (later) participate in consultations and votes

- **Experts**  
  - provide specialised commentary and analysis  
  - review and annotate proposals  
  - collaborate with AI to generate summaries and impact assessments

- **Institutions / organisations**  
  - publish proposals and background information  
  - use the app as a channel for structured feedback and participation  
  - later connect the app to institutional spaces on the CollectiVAI Chain

Initially, the app can also be used purely as an **AI companion**  
for democracy and civic tech topics.

---

## 4. Development Phases (high level)

The app follows three main phases:

1. **Alpha – AI Companion & Concept App**  
   - focus on AI explanations, topic exploration and concept validation.

2. **Beta – Civic Participation (off-chain)**  
   - add roles, proposal lifecycle, discussion features and local simulations.

3. **Chain Phase – Cosmos App-Chain Integration**  
   - connect to the CollectiVAI Chain (devnet / testnet)  
   - enable on-chain proposals and votes.

For more details, see the roadmap section in the root `README.md`.

---

## 5. Repository Scope

This repository contains:

- the Xcode project (`collectivai.xcodeproj`)
- the app source code (`collectivai/`)
- the main `README.md` (roadmap, status, related repositories)
- this `docs/` folder with:
  - `01-overview.md` – this document
  - `02-architecture.md` – technical structure & layers (planned)

Backend logic, chain code and devnet configuration live in:

- [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)
