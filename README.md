<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
</p>

<h1 align="center">CollectiVAI App (Prototype 0.1)</h1>
<h3 align="center">Democratic AI Companion & Civic Client</h3>

<p align="center">
  iOS · iPadOS · macOS · SwiftUI
</p>

---

## 🇩🇪 Kurzüberblick

**CollectiVAI** ist eine demokratische, menschenzentrierte AI-App mit europäischem Fokus.

Die App verbindet drei Ebenen:

1. **Chat** – ein sicherer AI-Assistent, der bei Anträgen, Konzepten und Policy-Fragen hilft (Demokratie, Klima, Wirtschaft, Sicherheit, Gesundheit, Forschung).  
2. **Contracts** – strukturierte, menschlich lesbare Anträge für Universitäten, Schulen, NGOs, Städte und Startups – vorbereitet für reale Förderprogramme.  
3. **Chain** – ein Civic-Dashboard, das zeigt, wie diese Anträge später als On-Chain-Proposals, Abstimmungen und öffentliche Budgets auf einer eigenen CollectiVAI-App-Chain erscheinen könnten.

Alle Anfragen laufen über einen **eigenen CollectiVAI-Backend-Router**:  
kein Tracking, keine Werbung, keine API-Keys auf dem Gerät.

---

## 🇬🇧 Overview

The **CollectiVAI App** is the client application for CollectiVAI –  
a democratic, human-centred AI project with a European focus.

The app connects three layers:

1. **Chat** – a safe AI assistant that helps you draft applications, policies and concepts for democracy, climate, economy, security, research and health.  
2. **Contracts** – structured, human-readable application forms for universities, schools, NGOs, cities and startups – ready to be plugged into real-world programmes.  
3. **Chain** – a civic dashboard illustrating how these applications could later appear as on-chain proposals, votes and public treasury allocations on a dedicated CollectiVAI app-chain.

All requests are routed through your own **CollectiVAI backend router**:  
no tracking, no ads, no API keys stored on device.

---

## Status

- ✅ Concept & public business plan  
- ✅ Initial Xcode project (SwiftUI, multi-tab layout)  
- ✅ Chat tab with topic & provider routing  
- ✅ Contracts tab with civic application wizard  
- ✅ Chain tab with civic dashboard & demo processes  
- ⏳ Full AI provider router (multi-model, production)  
- ⏳ Civic participation features (off-chain Beta)  
- ⏳ Cosmos App-Chain integration (devnet / testnet)  
- ⏳ App Store launch (depends on pilots & governance)

---

## ✨ Features in Prototype 0.1

### Chat · Democratic AI Router

- Chat-Interface mit Themenfokus:
  - Democracy & Society, Climate & Environment, Economy & Geopolitics  
  - Security & Infrastructure, Science & Innovation, Health & Wellbeing
- **Modes**: Ethical · Research · Technical  
- **Providers**: Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek  
- **Router-Sidebar** (wie bei ChatGPT):
  - Service profile (City, Universities, NGOs, Citizen, Startups)  
  - Topics, Providers & Models  
  - Projects (z.B. „Tallinn Citizens’ Budget“)  
  - Developer Mode mit Live Monitoring (Latency, Provider, Model)

### Contracts · Civic Applications

Screen „Contracts“ mit 6 Kacheln:

- Universities – Research, labs, citizen science  
- Schools – Education & democracy projects  
- NGOs – Campaigns & civic engagement  
- Cities – Public participation, councils  
- Startups – Prototypes & pilots  
- Custom – Free-form applications

Features:

- Schrittweiser **Application Wizard** (Basics → Content → Budget & Status)  
- Felder für Organisation, Land, Zielgruppe, Impact, Budget, Dauer  
- Status: Draft · Ready · Submitted · Archived  
- Übersicht über alle eigenen Entwürfe („Your drafts“)

### Chain · Civic Dashboard (Concept)

- 6-Tile Dashboard für:
  - Universities & Research  
  - Schools & Education  
  - Cities & Public Services  
  - NGOs & Civil Society  
  - Startups & Innovation  
  - My Impact & Reputation
- Demo-Sektionen:
  - **Civic processes (demo)** – z.B. „Tallinn Citizens’ Budget 2026“  
  - **Governance & voting (demo)** – Fact-checking Hub, Youth Assembly, etc.  
  - **Chain status (concept)** – erklärt die geplante App-Chain  
  - **How chat, contracts & chain connect**  
  - **Next steps (technical)**

> In the current prototype, there is **no live blockchain connection yet**.  
> The Chain tab shows how things could look once the CollectiVAI chain is live.

### Settings · Privacy & Control

- Default mode / provider / topic  
- Routing profile: Balanced · Research-heavy · Code & Security  
- Text size, Haptics, Developer Mode, Live Monitoring  
- App Lock (placeholder for Face ID / Passcode integration)  
- Telemetry toggle (anonymised, optional, planned)  
- Auto-delete local chats (planning parameter)  
- „No API keys on device“, „No ads, no trackers“ Info

---

## Roadmap & Feature Stages

The CollectiVAI App will evolve in three main stages:

### 🔹 Alpha – AI Companion & Concept App (current)

Focus: Local AI assistant and concept prototype for democratic decision-making.

- Topic explorer for democracy, civic tech and policy questions  
- Chat-based interface with AI assistant (Q&A, explanations, summaries)  
- Simple proposal & process views (demo data in Chain tab)  
- Basic app structure:
  - iOS / iPadOS / macOS (SwiftUI, Xcode)
- Integration with public docs:
  - links to the CollectiVAI website and GitHub organisation

> **Goal of the Alpha:** show how AI can help people **understand**  
> and **discuss** proposals and policy ideas.

### 🔹 Beta – Civic Participation App (off-chain)

Focus: turn the app into a real participation tool, still **off-chain**.

Planned features:

- Conceptual user roles:
  - Citizen view, Expert view, Institution / organisation view  
- Proposal lifecycle:
  - draft → discussion → (simulated) vote → result  
- Expert & comment mode:
  - experts can add comments / annotations
  - AI summarises expert perspectives  
- Insights & reports:
  - AI-generated summaries of discussions
  - impact / risk overview for proposals  
- Local “what-if” simulations:
  - explore consequences of different outcomes  
- Language selection (DE/EN first), topic preferences

> **Goal of the Beta:** show how CollectiVAI can be used as a  
> **participation and analysis app**, even before the blockchain is live.

### 🔹 Chain Phase – Cosmos App-Chain Integration

Focus: connect the app to the **CollectiVAI Chain**  
(a Cosmos-based App-Chain developed in [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)).

Planned features:

- Connection to CollectiVAI devnet / testnet (RPC endpoint selection)  
- On-chain proposals & voting (transactions, IDs, status)  
- Role-aware UI (citizen, expert, institution)  
- Governance transparency (timelines, links to block explorer)  
- Network awareness (devnet / testnet / mainnet)

> **Goal of the Chain Phase:** turn the CollectiVAI App into a  
> **full client for the CollectiVAI Chain**, where decisions are not only  
> discussed, but also **recorded and executed on-chain**.

---

## Architecture (high level)

The Xcode project is structured as a SwiftUI app:

- **Targets / platforms**
  - iOS
  - iPadOS
  - macOS (Catalyst or native, depending on configuration)

- **Planned layers**
  - **UI layer** – SwiftUI views (chat, contracts, chain, settings)  
  - **View models** – state management for screens and flows  
  - **AI provider router** – routes prompts to different AI providers  
  - **Chain client (planned)** – HTTP/gRPC client for the CollectiVAI Chain  
  - **Settings & storage** – local preferences, drafts, cached data

A dedicated `docs/` folder may later contain:

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
