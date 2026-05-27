<!--
  SOHAM PATIL — GITHUB PROFILE README
  Design language: Systems Observability Terminal
  All SVGs are self-contained. No external image deps except GitHub Stats cards and snake.
-->

<div align="center">

<!-- ═══════════════════════════════════════════════════════════════
     HERO BANNER — SVG animated terminal header
═══════════════════════════════════════════════════════════════ -->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://capsule-render.vercel.app/api?type=waving&color=0D1117&height=0">
</picture>

<img src="./assets/banner.svg" width="100%" alt="Soham Patil — Systems Engineer" />

</div>

---

<!-- ═══════════════════════════════════════════════════════════════
     SYSTEM IDENTITY BLOCK
═══════════════════════════════════════════════════════════════ -->

<div align="center">

```
┌─────────────────────────────────────────────────────────────────┐
│  PROCESS     soham-patil                                        │
│  ROLE        SDE Intern candidate · AI & Systems Engineering    │
│  INSTITUTION Pune Institute of Computer Technology  [9.14 GPA]  │
│  STATUS      ████████████████████░░░░  B.E. IT — Year 2 of 4   │
│  SIGNAL      building at the intersection of AI + infrastructure│
└─────────────────────────────────────────────────────────────────┘
```

</div>

---

<!-- ═══════════════════════════════════════════════════════════════
     TELEMETRY STRIP — LIVE STATS
═══════════════════════════════════════════════════════════════ -->

<div align="center">

<table border="0" cellspacing="0" cellpadding="0">
<tr>
<td width="50%" align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=soham-patil-05&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=3fb950&text_color=8b949e&ring_color=58a6ff&hide=prs&custom_title=system+metrics)

</td>
<td width="50%" align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=soham-patil-05&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=21262d&ring=58a6ff&fire=ff7b72&currStreakLabel=58a6ff&sideLabels=8b949e&dates=8b949e)

</td>
</tr>
</table>

</div>

---

<!-- ═══════════════════════════════════════════════════════════════
     SYSTEMS MAP — WHAT I BUILD
═══════════════════════════════════════════════════════════════ -->

<details open>
<summary><b>› SYSTEM ARCHITECTURE MAP</b> &nbsp;— what I actually build</summary>

<br>

```
                          ┌─ INGESTION LAYER ──────────────────────┐
                          │                                        │
  [LOG STREAMS] ──────── Kafka Topic ──── Orchestrator Daemon      │
  [METRICS]     ──────── Thresholds ──── Rule Engine               │
  [EVENTS]      ──────── ZooKeeper  ──── State Coordinator         │
                          └────────────────────┬───────────────────┘
                                               │ anomaly detected
                          ┌─ REASONING LAYER ──▼───────────────────┐
                          │                                        │
                          │  Gemini LLM ── ReAct Agent Loop        │
                          │    step 1: observe → tool_call         │
                          │    step 2: reason  → next_action       │
                          │    step N: [max 8] → remediation plan  │
                          │                                        │
                          └────────────────────┬───────────────────┘
                                               │ decision made
                          ┌─ RECOVERY LAYER ───▼───────────────────┐
                          │                                        │
                          │  Docker Socket ── restart / rollback   │
                          │  Redis Pub/Sub ── async worker pool    │
                          │  WebSocket     ── real-time telemetry  │
                          │  AES-256-GCM   ── encrypted audit log  │
                          │                                        │
                          └────────────────────────────────────────┘
```

> This is not pseudocode. This is the actual architecture of projects I've shipped.

</details>

---

<!-- ═══════════════════════════════════════════════════════════════
     PROJECT DOSSIER — 5 key projects as incident reports
═══════════════════════════════════════════════════════════════ -->

<details open>
<summary><b>› PROJECT DOSSIER</b> &nbsp;— incident-driven engineering log</summary>

<br>

### `[P-001]` Autonomous Self-Healing Microservices — AI SRE Engine
![Stack](https://img.shields.io/badge/Node.js-Kafka-3fb950?style=flat-square&labelColor=0d1117&color=3fb950)
![Stack](https://img.shields.io/badge/Gemini_ReAct-Agent-58a6ff?style=flat-square&labelColor=0d1117&color=58a6ff)
![Stack](https://img.shields.io/badge/Docker-ZooKeeper-ff7b72?style=flat-square&labelColor=0d1117&color=ff7b72)

> **Problem:** Distributed systems fail silently. Humans react too slowly.
> **Solution:** A closed-loop AI agent that ingests Kafka telemetry, reasons with a Gemini ReAct loop (8-step hard cap), and auto-executes Docker recovery ops.
> **Outcome:** Zero-touch remediation across LATENCY / ERROR / CRASH fault modes.

```
FAULT_DETECTED → AGENT_INVOKED → [reason→act×N] → RECOVERY_EXECUTED → INCIDENT_CLOSED
```

🔗 [Live Demo](https://self-healing-microservices-ai.vercel.app/) &nbsp;|&nbsp; [Source](https://github.com/soham-patil-05/self-healing-microservices)

---

### `[P-002]` TechFiesta — Real-Time Financial Reconciliation Engine
![Stack](https://img.shields.io/badge/Kafka-Redis_Pub/Sub-58a6ff?style=flat-square&labelColor=0d1117&color=58a6ff)
![Stack](https://img.shields.io/badge/AES--256--GCM-Encrypted-3fb950?style=flat-square&labelColor=0d1117&color=3fb950)
![Award](https://img.shields.io/badge/Hackathon-Finalist-ffd700?style=flat-square&labelColor=0d1117&color=e3b341)

> **Problem:** BANK_CBS ↔ PAYMENT_GATEWAY ↔ UPI_NETWORK produce concurrent high-frequency transaction logs. Duplicates corrupt settlement.
> **Solution:** Kafka ingestion + double-hash deduplication (UTR×RRN composite key) + Redis async worker pool. AES-256-GCM at ingestion boundary.
> **Outcome:** Plug-in comparator architecture. New payment networks = zero core changes.

---

### `[P-003]` Hack of Clans — Hackathon Team-Matching Ecosystem
![Stack](https://img.shields.io/badge/React-Express-58a6ff?style=flat-square&labelColor=0d1117&color=58a6ff)
![Stack](https://img.shields.io/badge/FastAPI-Playwright-3fb950?style=flat-square&labelColor=0d1117&color=3fb950)
![Stack](https://img.shields.io/badge/Socket.io-JWT-ff7b72?style=flat-square&labelColor=0d1117&color=ff7b72)

> 3-component ecosystem (React + Express + FastAPI scraper). Headless Playwright scraper with 20-scroll lazy-load, ThreadPoolExecutor-backed non-blocking PyMongo writes. Compound MongoDB text index for instant search. JWT + bcrypt + Google OAuth.

🔗 [Live Demo](https://vercel.com/soham-patils-projects-c6a065dc/hack-of-clans-frontend)

---

### `[P-004]` LabGuardian — OS-Level Lab Monitoring Daemon
![Stack](https://img.shields.io/badge/Python-psutil_asyncio-3fb950?style=flat-square&labelColor=0d1117&color=3fb950)
![Stack](https://img.shields.io/badge/SQLite-WebSockets-58a6ff?style=flat-square&labelColor=0d1117&color=58a6ff)

> Python daemon capturing browser history, active processes, USB interrupts at sub-10s latency. asyncio.Queue(maxsize=4096) with oldest-drop eviction. Offline-first SQLite buffer with reconnect-on-restore WebSocket bridge.

🔗 [Live Demo](https://labguardian.vercel.app/)

---

### `[P-005]` AI Object Identifier — Edge Inference Pipeline
![Stack](https://img.shields.io/badge/Gemini_Vision-Supabase_Edge-58a6ff?style=flat-square&labelColor=0d1117&color=58a6ff)
![Stack](https://img.shields.io/badge/TypeScript-React-3fb950?style=flat-square&labelColor=0d1117&color=3fb950)

> Gemini Vision API served via Supabase Edge Functions. Base64 in-memory processing — no blob storage. Client-side downscaling before encode. Structured JSON output: objectName · confidence · description · additionalInfo.

🔗 [Live Demo](https://object-identification-3.onrender.com/)

</details>

---

<!-- ═══════════════════════════════════════════════════════════════
     STACK REGISTRY — clean, no badge spam
═══════════════════════════════════════════════════════════════ -->

<details>
<summary><b>› STACK REGISTRY</b> &nbsp;— everything I've shipped with</summary>

<br>

| Layer | Technologies |
|:------|:-------------|
| **Languages** | Python · JavaScript · TypeScript · C++ · SQL |
| **Runtime & Frameworks** | Node.js · Express.js · FastAPI · React · Socket.io |
| **AI & Agents** | Gemini API (Text + Vision) · ReAct Agent Pattern · LLM Tool-Calling |
| **Messaging & Stream** | Apache Kafka · ZooKeeper · Redis Pub/Sub |
| **Async & Systems** | asyncio · psutil · ThreadPoolExecutor · WebSockets |
| **Databases** | MongoDB · Redis Cache · SQLite · Mongoose |
| **Infrastructure** | Docker · Vercel · Supabase · Cloudinary · AES-256-GCM |
| **Security & Auth** | JWT · bcryptjs · Google OAuth2 |
| **Scraping & Automation** | Playwright · Headless Chromium |

</details>

---

<!-- ═══════════════════════════════════════════════════════════════
     COMPETITIVE PROGRAMMING — operator metrics
═══════════════════════════════════════════════════════════════ -->

<details>
<summary><b>› OPERATOR METRICS</b> &nbsp;— competitive programming signal</summary>

<br>

```
┌──────────────────────────────────────────────────────────────────┐
│  PLATFORM          RANK / RATING        PROBLEMS               │
├──────────────────────────────────────────────────────────────────┤
│  LeetCode          Knight  ·  1923      600+ solved            │
│  CodeChef          3-Star  ·  1638      active                 │
│  Codeforces        Pupil   ·  1380      active                 │
│  GeeksforGeeks     —                   contributed             │
└──────────────────────────────────────────────────────────────────┘
```

[![LeetCode](https://img.shields.io/badge/LeetCode-Knight_1923-e3b341?style=flat-square&labelColor=0d1117&logo=leetcode&logoColor=e3b341)](https://leetcode.com/u/sompatil2005/)
[![CodeChef](https://img.shields.io/badge/CodeChef-3★_1638-58a6ff?style=flat-square&labelColor=0d1117)](https://www.codechef.com/)
[![Codeforces](https://img.shields.io/badge/Codeforces-Pupil_1380-3fb950?style=flat-square&labelColor=0d1117)](https://codeforces.com/)

</details>

---

<!-- ═══════════════════════════════════════════════════════════════
     CONTRIBUTION SNAKE ANIMATION
═══════════════════════════════════════════════════════════════ -->

<div align="center">

**CONTRIBUTION TRACE**

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake.svg">
  <img alt="contribution snake" src="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake.svg">
</picture>

</div>

---

<!-- ═══════════════════════════════════════════════════════════════
     MOST USED LANGUAGES
═══════════════════════════════════════════════════════════════ -->

<div align="center">

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=soham-patil-05&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=8b949e&langs_count=8&custom_title=language+distribution)

</div>

---

<!-- ═══════════════════════════════════════════════════════════════
     FOOTER — signal line
═══════════════════════════════════════════════════════════════ -->

<div align="center">

<br>

```
╔══════════════════════════════════════════════════════════╗
║  I build systems that observe themselves and recover.    ║
║  I write agents that reason and act.                     ║
║  I ship end-to-end.                                      ║
╚══════════════════════════════════════════════════════════╝
```

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-soham--patil-0a66c2?style=flat-square&labelColor=0d1117&logo=linkedin&logoColor=0a66c2)](https://www.linkedin.com/in/soham-patil-27a9b2287)
&nbsp;
[![Email](https://img.shields.io/badge/Email-sompatil2005@gmail.com-ff7b72?style=flat-square&labelColor=0d1117&logo=gmail&logoColor=ff7b72)](mailto:sompatil2005@gmail.com)
&nbsp;
[![LeetCode](https://img.shields.io/badge/LeetCode-Knight-e3b341?style=flat-square&labelColor=0d1117&logo=leetcode&logoColor=e3b341)](https://leetcode.com/u/sompatil2005/)

<br>

<sub>last compiled · auto-updated daily via GitHub Actions</sub>

</div>
