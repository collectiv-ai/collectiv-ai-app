<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
</p>

<h1 align="center">CollectiVAI App</h1>
<h3 align="center">Democratic AI Companion & Civic Client</h3>

<p align="center">
  <a href="#deutsch">🇩🇪 Deutsch</a> &nbsp;|&nbsp; <a href="#english">🇬🇧 English</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Prototype%200.1-ffcc00?style=flat" alt="Status Prototype 0.1" />
  <img src="https://img.shields.io/badge/Platforms-iOS%20%7C%20iPadOS%20%7C%20macOS-333333?style=flat" alt="Platforms" />
  <img src="https://img.shields.io/badge/Tech-SwiftUI%20%7C%20Xcode-0c7bdc?style=flat" alt="Tech" />
  <img src="https://img.shields.io/badge/Made%20in-Europe-003399?style=flat" alt="Made in Europe" />
</p>

---

## 🇩🇪 Übersicht <a id="deutsch"></a>

Die **CollectiVAI App** ist der **Client** für das CollectiVAI-Ökosystem:  
eine demokratische, menschenzentrierte AI-Plattform mit Fokus auf Europa.

Die App verbindet drei Ebenen:

1. **Chat** – ein sicherer AI-Assistent, der bei Anträgen, Konzepten und Policy-Fragen hilft  
   (Demokratie, Klima, Wirtschaft, Sicherheit, Forschung, Gesundheit).

2. **Contracts** – strukturierte, menschlich lesbare Anträge für  
   Universitäten, Schulen, NGOs, Städte und Startups – vorbereitet für reale Programme.

3. **Chain** – ein Civic-Dashboard, das zeigt, wie diese Anträge später als  
   **On-Chain-Proposals, Abstimmungen und Budgets** auf einer eigenen CollectiVAI-App-Chain erscheinen könnten.

Alle Anfragen laufen über deinen eigenen **CollectiVAI-Backend-Router**:  
kein Tracking, keine Werbung, keine API-Keys auf dem Gerät.

---

### 🇩🇪 Funktionsbereiche (Prototype 0.1)

#### 1. Chat · Democratic AI Router

- Themenfokus:
  - Democracy & Society, Climate & Environment, Economy & Geopolitics  
  - Security & Infrastructure, Science & Innovation, Health & Wellbeing
- **Modes:** Ethical · Research · Technical  
- **Provider:** Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek  
- **Router-Sidebar** (inspiriert von ChatGPT):
  - Service Profile (Cities, Universities, NGOs, Citizen, Startups)
  - Topics, Providers & Models
  - Projects (z. B. „Tallinn Citizens’ Budget“)
  - Developer Mode mit Live-Monitoring (Latenz, Provider, Model – geplant)

#### 2. Contracts · Civic Applications

Screen „Contracts“ mit 6 Kacheln:

- Universities – Research, Labs, Citizen Science  
- Schools – Education & Democracy Projects  
- NGOs – Campaigns & Civic Engagement  
- Cities – Public Participation, Councils  
- Startups – Prototypes & Pilots  
- Custom – Freie Anträge

Features:

- **3-Schritte-Wizard** (Basics → Content → Budget & Status)  
- Felder für Organisation, Land, Zielgruppe, Impact, Budget, Dauer  
- Status: Draft · Ready · Submitted · Archived  
- Übersicht „Your drafts“ für alle eigenen Entwürfe

#### 3. Chain · Civic Dashboard (Konzept)

- Dashboard mit Kacheln:
  - Universities & Research  
  - Schools & Education  
  - Cities & Public Services  
  - NGOs & Civil Society  
  - Startups & Innovation  
  - My Impact & Reputation
- Demo-Bereiche:
  - Civic Processes (z. B. „Tallinn Citizens’ Budget 2026“)  
  - Governance & Voting (Fact-Checking Hub, Youth Assembly, etc.)  
  - Chain-Status (erklärt die geplante App-Chain)  
  - Wie Chat, Contracts & Chain zusammenhängen

> Im aktuellen Prototyp gibt es **noch keine Live-Blockchain-Anbindung**.  
> Die Chain-Ansicht zeigt, wie es später aussehen könnte.

#### 4. Settings · Privacy & Control

- Standard-Mode / Provider / Topic  
- Routing-Profile: Balanced · Research-heavy · Code & Security  
- Textgröße, Haptik, Developer Mode, Live-Monitoring  
- App-Lock (Platzhalter für Face ID / Passcode)  
- Telemetry-Toggle (anonymisiert, geplant)  
- Auto-Delete-Planung für lokale Chats  
- Hinweise: „No API keys on device“, „No ads, no trackers“

---

### 🇩🇪 Status & Roadmap

**Aktueller Status (Prototype 0.1):**

- ✅ Konzept & öffentliches Business-Dokument  
- ✅ Xcode-App mit Multi-Tab-Layout (Chat, Contracts, Chain, Settings)  
- ✅ Chat-Router (Themen, Provider, Modes)  
- ✅ Contracts-Wizard für Civic Applications  
- ✅ Chain-Dashboard als Konzeptansicht  
- ⏳ Anbindung echter Programme / Piloten (Städte, Unis, NGOs)  
- ⏳ Integration mit CollectiVAI Chain (Cosmos Devnet/Testnet)  
- ⏳ App-Store-Release (abhängig von Governance & Partnern)

**Geplante Phasen:**

1. **Alpha – AI Companion & Konzept-App**  
2. **Beta – Civic Participation (off-chain)**  
3. **Chain Phase – Vollständige Cosmos-App-Chain-Integration**

---

### 🇩🇪 Architektur (vereinfachter Überblick)

- **Plattformen**
  - iOS  
  - iPadOS  
  - macOS (SwiftUI / ggf. Catalyst)

- **Schichten**
  - **UI-Layer** – SwiftUI-Views (Chat, Contracts, Chain, Settings)  
  - **State & Config** – zentrale Konfiguration (Provider, Mode, Topics, Projekte)  
  - **Backend-Client** – `CollectivAIBackend` (HTTP-Client zu deinem Router-Backend)  
  - **Chain-Client (geplant)** – Cosmos-Client für CollectiVAI Chain  
  - **Local Storage** – AppStorage, lokale Drafts, später Caches & Persistence

---

## 🇬🇧 Overview <a id="english"></a>

The **CollectiVAI App** is the **client application** for the CollectiVAI ecosystem:  
a democratic, human-centred AI platform with a European focus.

It connects three main layers:

1. **Chat** – a safe AI assistant for drafting applications, policies and concepts  
   across democracy, climate, economy, security, research and health.

2. **Contracts** – structured, human-readable application forms for  
   universities, schools, NGOs, cities and startups – ready for real-world programmes.

3. **Chain** – a civic dashboard showing how these applications could later appear as  
   **on-chain proposals, votes and public treasury allocations** on a dedicated CollectiVAI app-chain.

All requests are routed through **your own CollectiVAI backend router**:  
no tracking, no ads, no API keys stored on device.

---

### 🇬🇧 Feature Areas (Prototype 0.1)

#### 1. Chat · Democratic AI Router

- Topic-focused chat:
  - Democracy & society, climate & environment, economy & geopolitics  
  - security & infrastructure, science & innovation, health & wellbeing
- **Modes:** Ethical · Research · Technical  
- **Providers:** Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek  
- Router-style sidebar (ChatGPT-inspired):
  - service profiles (cities, universities, NGOs, citizens, startups)  
  - topics, providers & models  
  - projects (e.g. “Tallinn Citizens’ Budget”)  
  - optional developer mode with live monitoring (latency, provider, model)

#### 2. Contracts · Civic Applications

- Screen with 6 tiles:
  - universities, schools, NGOs, cities, startups, custom
- **3-step wizard**:
  - basics (organisation, country, title)  
  - content & impact (summary, impact, target groups)  
  - budget & duration (amount, currency, duration, status)
- Status: Draft · Ready · Submitted · Archived  
- “Your drafts” overview for all local applications

#### 3. Chain · Civic Dashboard (Concept)

- 6-tile dashboard:
  - Universities & research  
  - Schools & education  
  - Cities & public services  
  - NGOs & civil society  
  - Startups & innovation  
  - My impact & reputation
- Demo sections:
  - civic processes (e.g. „Tallinn Citizens’ Budget 2026“)  
  - governance & voting (fact-checking hub, youth assembly, etc.)  
  - chain status (explaining the planned app-chain)  
  - how chat, contracts & chain connect

> In the current prototype, there is **no live blockchain connection yet**.  
> The Chain tab shows how things could look once the CollectiVAI Chain is live.

#### 4. Settings · Privacy & Control

- default mode / provider / topic  
- routing profiles: Balanced · Research-heavy · Code & Security  
- text size, haptics, developer mode, live monitoring  
- app lock (placeholder for Face ID / passcode integration)  
- telemetry toggle (anonymised, opt-in, planned)  
- auto-delete planning for local conversations  
- info blocks: “No API keys on device”, “No ads, no trackers”

---

### 🇬🇧 Status & Roadmap

**Current status (Prototype 0.1):**

- ✅ Core concept & public business plan  
- ✅ Initial Xcode app (SwiftUI, multi-tab layout)  
- ✅ Chat tab with topic & provider routing  
- ✅ Contracts tab with civic application wizard  
- ✅ Chain tab with civic dashboard & demo processes  
- ⏳ Integration with real programmes & pilots (cities, universities, NGOs)  
- ⏳ Integration with the CollectiVAI Chain (Cosmos devnet / testnet)  
- ⏳ App Store release (depends on governance & partners)

**Planned phases:**

1. **Alpha – AI Companion & Concept App**  
2. **Beta – Civic Participation (off-chain)**  
3. **Chain Phase – Full Cosmos App-Chain integration**

---

## 🔗 Related Repositories

- ⛓ **Cosmos App-Chain (backend)**  
  [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

- 🌐 **Website & public docs**  
  [`collectiv-ai.github.io`](https://github.com/collectiv-ai/collectiv-ai.github.io)

- 🧭 **Business plan & strategy**  
  [`collectiv-ai-business`](https://github.com/collectiv-ai/collectiv-ai-business)

- 🎨 **Branding & visual identity**  
  [`collectiv-ai-branding`](https://github.com/collectiv-ai/collectiv-ai-branding)

---

## 📄 Licence & branding

The source code licence for this repository is defined in the `LICENSE` file (if present).

The **CollectiVAI name, logo and visual identity** are protected.  
Any use in products, services or campaigns requires prior written permission.

© David Miecznikowski, CollectiVAI.
