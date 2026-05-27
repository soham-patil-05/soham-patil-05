<div align="center">
<img src="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/main/assets/banner.svg" width="100%" alt="soham patil"/>
</div>

<br>

---

<br>

```
things I've built recently, and what made them interesting to build
```

<br>

**Autonomous microservice recovery** &nbsp;·&nbsp; a system that watches itself break and decides what to do about it.

Kafka feeds a log stream into an orchestrator. When a threshold trips, a Gemini ReAct agent takes over — it reasons in a loop, issues structured tool calls (restart, rollback, scale-out), and closes the incident without a human. Hard-capped at 8 reasoning steps to prevent drift. Provider health router switches models if the primary API degrades. The interesting part wasn't the AI — it was making the recovery actions deterministic enough to trust.

→ [self-healing-microservices-ai.vercel.app](https://self-healing-microservices-ai.vercel.app/)

<br>

**Financial reconciliation under concurrency** &nbsp;·&nbsp; three payment networks, one ground truth, no duplicates.

Three concurrent Kafka streams (bank ledger, payment gateway, UPI network) need to converge into a single consistent settlement state. Double-hashing on composite keys (UTR × RRN) handles deduplication deterministically. Match computation runs in async Redis Pub/Sub workers off the main thread. AES-256-GCM wraps merchant identifiers at ingestion. Built as a hackathon finalist entry — the constraint made the design tighter.

<br>

**OS-level lab daemon** &nbsp;·&nbsp; event capture without a VM, at sub-10s latency.

A Python background process using `psutil` + `asyncio` captures browser history, active processes, and USB interrupts. `asyncio.Queue(maxsize=4096)` with oldest-drop eviction bounds memory under bursts. SQLite buffers everything offline — a persistent WebSocket bridge drains it on reconnect. The design constraint was: no privileged access, no VM overhead, no data loss on disconnect.

→ [labguardian.vercel.app](https://labguardian.vercel.app/)

<br>

**Hackathon team-matching platform** &nbsp;·&nbsp; dynamic data, three components, one coherent system.

React + Express + FastAPI. The scraper is the interesting piece: Playwright with a 20-scroll lazy-load loop, `ThreadPoolExecutor`-backed PyMongo writes to keep FastAPI non-blocking, 3-attempt retry backoff. MongoDB compound text index covers team name, hackathon, and description for instant search. Socket.io for persistent group and private chat rooms. JWT + bcrypt + Google OAuth.

→ [hack-of-clans](https://vercel.com/soham-patils-projects-c6a065dc/hack-of-clans-frontend)

<br>

**Gemini Vision at the edge** &nbsp;·&nbsp; inference without a backend.

Supabase Edge Functions run the Gemini Vision API call entirely in-memory — no blob storage, no server. Client-side downscaling before Base64 encode keeps the payload small. Structured JSON output schema: objectName, confidence, description, additionalInfo. The goal was: fewest moving parts between image and answer.

→ [object-identification-3.onrender.com](https://object-identification-3.onrender.com/)

<br>

---

<br>

```
stack — what shows up across most of these
```

<br>

<div align="center">

| systems & messaging | ai & inference | web & runtime | languages |
|:---:|:---:|:---:|:---:|
| Kafka · ZooKeeper | Gemini API | Node.js · Express | Python |
| Redis Pub/Sub | ReAct agent pattern | FastAPI · React | TypeScript |
| Docker | LLM tool-calling | Socket.io | JavaScript |
| WebSockets | Supabase Edge | Playwright | C++ |
| asyncio · psutil | structured JSON prompting | JWT · OAuth2 | SQL |

</div>

<br>

---

<br>

```
elsewhere
```

<br>

<div align="center">

[![leetcode](https://img.shields.io/badge/leetcode-knight_%C2%B7_1923-e3b341?style=flat-square&labelColor=161b22&color=e3b341)](https://leetcode.com/u/sompatil2005/)
&ensp;
[![codechef](https://img.shields.io/badge/codechef-3★_%C2%B7_1638-58a6ff?style=flat-square&labelColor=161b22&color=58a6ff)](https://www.codechef.com/)
&ensp;
[![codeforces](https://img.shields.io/badge/codeforces-pupil_%C2%B7_1380-3fb950?style=flat-square&labelColor=161b22&color=3fb950)](https://codeforces.com/)
&ensp;
[![linkedin](https://img.shields.io/badge/linkedin-soham--patil-8b949e?style=flat-square&labelColor=161b22&color=8b949e)](https://www.linkedin.com/in/soham-patil-27a9b2287)

</div>

<br>

---

<br>

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake.svg">
  <img alt="contribution graph" src="https://raw.githubusercontent.com/soham-patil-05/soham-patil-05/output/github-contribution-grid-snake-dark.svg">
</picture>

</div>

<br>
