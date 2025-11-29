---

## Roadmap & Feature Stages

The CollectiVAI App will evolve in three main stages:

### 🔹 Alpha – AI Companion & Concept App (current stage)

Focus: Local AI assistant and concept prototype for democratic decision-making.

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

> Goal of the Alpha: show how AI can help people **understand** and **discuss** proposals.

---

### 🔹 Beta – Civic Participation App (off-chain)

Focus: turn the app into a real participation tool, still **off-chain** (no Cosmos connection yet).

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

> Goal of the Beta: show how CollectiVAI can be used as a **participation and analysis app**,  
> even before the blockchain infrastructure is live.

---

### 🔹 Chain Phase – Cosmos App-Chain Integration

Focus: connect the app to the **CollectiVAI Chain** (Cosmos-based App-Chain).

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

> Goal of the Chain Phase: turn the CollectiVAI App into a **full client for the CollectiVAI Chain**,  
> where democratic decisions are not only discussed, but also **recorded and executed on-chain**.

---

## Relation to the CollectiVAI Chain

This app is designed as the primary client for the **CollectiVAI Chain**  
(a Cosmos-based App-Chain developed in a separate repository):

- Chain repo: [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

The app can already be developed and tested in **Alpha** and **Beta** stages  
without a running chain. Later, the Chain Phase will add full on-chain governance support.
