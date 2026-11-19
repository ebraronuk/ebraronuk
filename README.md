## Hi, I'm Ebrar

Full-Stack & AI Engineer. I build the AI layer and the services underneath it, and I carry both.

**What I'm after:** products where the agent behaviour and the API beneath it belong to the same engineer.

### What I do

- **Multi-agent systems in production** — LangGraph, intent routing, tool-calling loops, guardrails that keep agents inside their scope
- **RAG and retrieval** — pgvector, Chroma, hybrid retrieval, and working out *why* a live answer came back wrong, which is usually not the model
- **Evaluation** — eval sets, LLM-as-judge, regression runs. Without them you are guessing whether a change helped
- **Writing code with AI agents, and checking it** — Claude Code, Codex, Cursor. A generated service can pass its tests and still put a query in the wrong layer
- **The unglamorous half** — REST surfaces, database structures, service boundaries, Docker, CI/CD, store releases

Most recently [an AI family assistant in Turkish](https://apps.apple.com/tr/app/asisimo-aile-destek-asistan%C4%B1/id6757652820?l=tr), live on iOS and Android: 20+ specialist agents behind an orchestrator, close to 70 function definitions in the tool-calling loop. It arrived as an idea with no spec. The requirement work, the architecture and the stack calls were mine.

### Public repos

**[multi-agent-banking-rag](https://github.com/ebraronuk/multi-agent-banking-rag)** — the architecture I work with every day, written from scratch: LangGraph orchestration, hybrid RAG, FastMCP tool-calling, a rule-based guardrail layer.

**[ad-applicability](https://github.com/ebraronuk/ad-applicability)** — an FAA directive says which aircraft it binds in prose, not a list. This reads that paragraph and answers for a whole fleet, naming what it cannot determine instead of guessing. A missing fact can widen an answer to undetermined but never flip a definite yes into a no, and that is a property test rather than a comment.

**[talep-onay-sistemi](https://github.com/ebraronuk/talep-onay-sistemi)** — Spring Boot 3.5 and Java 21. The layer rules are ArchUnit tests instead of a paragraph in a document, and the audit trail is immutable in the database rather than in Java.

I check my own work and publish both numbers: `ad-applicability` extracted a constraint from 194 of 196 real directives, but a hand audit of 20 clauses found **10 of them wrong**. Three systematic defects later the same audit gives **18 of 20**.

---

[ebraronuk.com](https://ebraronuk.com) · [linkedin.com/in/ebraronuk](https://linkedin.com/in/ebraronuk) · İstanbul, Türkiye
