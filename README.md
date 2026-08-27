<h1 align="center">👋 Hi, I'm Ebrar</h1>

<p align="center">
  <b>AI Engineer</b> · <b>Full-Stack Developer</b> · <b>Electrical & Electronics Engineer</b>
  <br/>
  Building agentic AI systems where <i>business clarity</i> meets <i>engineering discipline</i>.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ebraronuk">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="mailto:ebraronuk00@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

---

## 🎯 What I Work On

- 🤖 **Multi-agent AI orchestration:** LangGraph-based systems coordinating 30+ agents in production (planning, tool-calling, message passing, shared memory)
- 🔎 **RAG & retrieval architectures:** embedding models, vector databases, hybrid retrieval
- 💬 **Conversational AI:** chatbots, AI assistants, voice interfaces (STT/TTS), intent recognition
- 🔌 **Tool-calling & MCP:** Model Context Protocol integrations, function/tool-calling pipelines
- ☕ **Enterprise backend:** Spring Boot, JPA/Hibernate, layered architecture with the layer rules enforced as tests rather than documentation
- 🌿 **Configuration management:** PLM/ERP traceability, lifecycle consistency (defense industry background, embedded C/STM32)
- 🎯 **Product & technical architecture:** end-to-end ownership, from system design to shipped product

---

## 📱 Asisimo: Shipped, End-to-End

**Asisimo** is a Turkish-language AI family assistant for iOS & Android, built from the idea stage onward as one of two engineers on the team. I owned the product across every layer: frontend, backend, AI/agent architecture, database schema, a shared component library, and UI testing, through the initial release and every update since.

<p align="center">
  <a href="https://apps.apple.com/tr/app/asisimo-aile-destek-asistan%C4%B1/id6757652820">
    <img src="https://img.shields.io/badge/App_Store-Download-0D96F6?style=for-the-badge&logo=apple&logoColor=white" alt="Download on the App Store"/>
  </a>
  &nbsp;
  <a href="https://play.google.com/store/apps/details?id=com.asisimo.app&hl=tr">
    <img src="https://img.shields.io/badge/Google_Play-Download-414141?style=for-the-badge&logo=googleplay&logoColor=white" alt="Get it on Google Play"/>
  </a>
  &nbsp;
  <a href="https://asisimo.com/tr">
    <img src="https://img.shields.io/badge/Website-asisimo.com-000000?style=for-the-badge&logo=googlechrome&logoColor=white" alt="asisimo.com"/>
  </a>
</p>

**Stack:** React Native · Expo · TypeScript · Node.js · Express · LangGraph · Supabase · Redis · Google Gemini (multi-model) · Embedding-based semantic router · Custom agent framework (tool-defs + tool-handlers + LLMService)

---

## 🧪 Reference Implementations

Most of my professional work sits in private company repositories. These two are built deliberately as public reference pieces, each one covering a different side of what I do.

### 🤖 Multi-Agent Banking RAG

An open, from-scratch implementation of the AI architecture patterns I work with daily: LangGraph orchestration, hybrid RAG (vector + BM25), FastMCP tool-calling, rule-based NER and intent recognition, and a policy guardrail layer, wired around a fictional banking-support domain.

[**ebraronuk/multi-agent-banking-rag**](https://github.com/ebraronuk/multi-agent-banking-rag)

**Stack:** LangGraph · FastMCP · FastAPI · Chroma · Docker · Kubernetes

### ☕ Enterprise Approval Workflow

A corporate request-and-approval system, built to show how I write backend code when nobody is rushing me.

- Two-stage approval driven by amount thresholds: a unit manager approves up to a configurable limit, anything above goes to executive approval
- Audit trail that is immutable at the **database** level, not just in Java: a PostgreSQL trigger rejects `UPDATE` and `DELETE` on the audit table
- Optimistic locking so two managers deciding on the same request at the same moment cannot silently overwrite each other
- Every performance claim in the README is measured rather than asserted: N+1 query counts before and after, `EXPLAIN ANALYZE` output, p95 latency under 50 concurrent requests
- Layer rules (domain knows nothing about HTTP, controllers never touch repositories) are enforced as ArchUnit tests. They caught two real circular dependencies on the day they were written
- 202 tests, including 32 authorization tests that exercise every role against every endpoint through the real security filter chain

[**ebraronuk/talep-onay-sistemi**](https://github.com/ebraronuk/talep-onay-sistemi)

**Stack:** Spring Boot 3.5 · Java 21 · PostgreSQL 16 · Spring Security (JWT) · Flyway · Testcontainers · React + TypeScript · Docker · GitHub Actions

---

<details>
<summary><b>🛰️ Earlier work: aerospace, defense & tooling</b></summary>

<br/>

| Project | What it does | Stack |
|---|---|---|
| 💬 [**nextreach-chatbot**](https://github.com/ebraronuk/nextreach-chatbot) | B2B SaaS lead-qualification chatbot + admin dashboard, built in a 6-hour timed challenge | Next.js · Supabase · Gemini |
| 🛰️ [**embedded-telemetry-toolkit**](https://github.com/ebraronuk/embedded-telemetry-toolkit) | UAV telemetry simulator, parser and anomaly analyzer with a Streamlit GUI | Python · pytest · Streamlit · CI |
| 🧭 [**imu-gps-magnetometer-analyzer**](https://github.com/ebraronuk/imu-gps-magnetometer-analyzer) | Avionics sensor toolkit: hard/soft-iron calibration, FFT, complementary filtering | Python · NumPy/SciPy · PyQt5 · Plotly |
| 🏭 [**plm-config-migration-tool**](https://github.com/ebraronuk/plm-config-migration-tool) | Excel to PLM/ERP BOM migration with validation, normalization and traceability | Python · YAML · Excel · SQL |
| ✈️ [**engine-performance-analyzer**](https://github.com/ebraronuk/engine-performance-analyzer) | Aircraft engine performance and degradation-trend analysis | Python · MATLAB |

</details>

---

## ⚙️ Technologies & Tools

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/React_Native-61DAFB?style=flat&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=chainlink&logoColor=white"/>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/Anthropic_Claude-D97757?style=flat&logo=anthropic&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white"/>
</p>

---

<p align="center"><i>İstanbul, Türkiye</i></p>
