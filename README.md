## Hi, I'm Ebrar

Full-Stack & AI Engineer. My degree is in Electrical & Electronics Engineering.

The part of this job I like most is when someone describes a problem out loud and it isn't written down anywhere yet. I take it from there: work out what it actually needs to do, build it, and stay with it until it ships.

### What I do

**Figure out what needs building.** Sit with the people who need the thing, turn it into flows and a schema, decide what gets built in which week.

**Build with AI agents, and check their work.** Claude Code, Codex and Cursor are how I write code now. The part that still needs an engineer is reading what comes back. A generated service can pass its tests and still put a query in the wrong layer.

**Multi-agent systems in production.** LangGraph and LangChain: a router that reads intent, specialist agents behind it, tool-calling loops, shared memory, guardrails that keep agents inside their scope.

**RAG and retrieval.** Embeddings, vector stores (pgvector, Chroma), hybrid retrieval, reranking. And the part people skip: working out *why* a live answer came back wrong, which is usually not the model.

**Evaluation.** Eval sets, LLM-as-judge, regression runs, Langfuse. Without them you're guessing whether a change helped, and I'd rather know.

**The unglamorous half.** REST surfaces, database structures, service boundaries, Docker, CI/CD, store releases.

**Configuration management.** PLM and ERP traceability, change control. This is where I started, in aerospace.

### Asisimo

An AI family assistant in Turkish, live on iOS and Android. Small team, and I was on it from the first day.

It came to us as an idea. No spec, nothing written down. I did the requirement and process work, made the architecture and stack calls, then built it.

Underneath: 21 specialist agents behind a supervisor and an orchestrator on LangGraph, 68 function definitions in the tool-calling loop, three-tier intent detection, guardrails on every agent.

One thing I'm glad I got right. When wrong answers started showing up in production, the instinct is to blame the model. It wasn't the model, it was retrieval. I rewrote that layer and put eval sets and regression runs around it, so the next time I'd know instead of guessing.

`React Native · TypeScript · Node.js · FastAPI · LangGraph · Supabase · pgvector · Redis · Docker`

[App Store](#) · [Google Play](#) · [asisimo.com](https://asisimo.com)

### Two public repos

Most of what I've built sits in private company repos. These two are public on purpose, so there's something to point at.

**[multi-agent-banking-rag](https://github.com/ebraronuk/multi-agent-banking-rag)** — the architecture I work with every day, written from scratch: LangGraph orchestration, hybrid RAG (vector + BM25), FastMCP tool-calling, rule-based NER and intent recognition, a policy guardrail layer.
`LangGraph · FastMCP · FastAPI · Chroma · Docker · Kubernetes`

**[talep-onay-sistemi](https://github.com/ebraronuk/talep-onay-sistemi)** — backend code written with nobody rushing me. The layer rules are ArchUnit tests instead of a paragraph in a document, and they caught two real circular dependencies the day I added them. The audit trail is immutable in the database, not just in Java. Every performance number in the README is measured, not claimed.
`Spring Boot · Java 21 · PostgreSQL · Spring Security · Flyway · Testcontainers`

<details>
<summary><b>🛰️ Earlier work: aerospace, defense &amp; tooling</b></summary>

<br>

| Project | What it does | Stack |
|---|---|---|
| 💬 **[nextreach-chatbot](https://github.com/ebraronuk/nextreach-chatbot)** | B2B SaaS lead-qualification chatbot + admin dashboard, built in a 6-hour timed challenge | Next.js · Supabase · Gemini |
| 🛰️ **[embedded-telemetry-toolkit](https://github.com/ebraronuk/embedded-telemetry-toolkit)** | UAV telemetry simulator, parser and anomaly analyzer with a Streamlit GUI | Python · pytest · Streamlit · CI |
| 🧭 **[imu-gps-magnetometer-analyzer](https://github.com/ebraronuk/imu-gps-magnetometer-analyzer)** | Avionics sensor toolkit: hard/soft-iron calibration, FFT, complementary filtering | Python · NumPy/SciPy · PyQt5 · Plotly |
| 🏭 **[plm-config-migration-tool](https://github.com/ebraronuk/plm-config-migration-tool)** | Excel to PLM/ERP BOM migration with validation, normalization and traceability | Python · YAML · Excel · SQL |
| ✈️ **[engine-performance-analyzer](https://github.com/ebraronuk/engine-performance-analyzer)** | Aircraft engine performance and degradation-trend analysis | Python · MATLAB |

</details>

---

İstanbul, Türkiye · [ebraronuk.com](https://ebraronuk.com) · [linkedin.com/in/ebraronuk](https://linkedin.com/in/ebraronuk)
