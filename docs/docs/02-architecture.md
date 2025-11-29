# CollectiVAI App – Architecture (Draft)

This document describes the planned technical structure
of the CollectiVAI App (iOS / iPadOS / macOS, SwiftUI).

---

## 1. Platforms & Technologies

- **Platforms**
  - iOS
  - iPadOS
  - macOS (Catalyst or native SwiftUI, depending on configuration)

- **Technologies**
  - Swift & SwiftUI
  - Combine / async/await for reactive data flows
  - URLSession / HTTP clients for API calls
  - (later) gRPC / WebSocket client for the CollectiVAI Chain

---

## 2. High-Level Architecture

```text
+------------------------------+
|         SwiftUI UI           |
|  - screens & navigation      |
+--------------+---------------+
               |
               v
+------------------------------+
|        View Models           |
|  - state & intents           |
|  - coordinates services      |
+--------------+---------------+
               |
               v
+------------------------------+
|         Services             |
|  - AI provider router        |
|  - app backend APIs          |
|  - chain client (planned)    |
+--------------+---------------+
               |
               v
+------------------------------+
|   Storage & Configuration    |
|  - user settings             |
|  - cached data / drafts      |
+------------------------------+
