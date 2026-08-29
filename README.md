<div align="center">

# Johan Lin

**AI Application Engineer · Full Stack Development · M.Eng. CS @ Guangzhou University**

[![Profile views](https://komarev.com/ghpvc/?username=Linz1248&label=Profile+views&color=0e75b6&style=flat-square)](https://github.com/Linz1248)
[![Email](https://img.shields.io/badge/Email-1552855968%40qq.com-D14836?style=flat-square)](mailto:1552855968@qq.com)

</div>

---

## 🧑‍💻 About Me

- 🔭 Currently an **AI Full-stack Intern @ MINISO** — building the group's internal **Agent platform** and **LLM evaluation & data-flywheel** pipelines
- 🤖 I build **LLM-powered agent systems** and **full-stack apps** — multi-agent orchestration, hybrid RAG pipelines, and end-to-end services with **LangGraph / LangChain**, **FastAPI / Spring Boot**, and **Vue.js**
- 🧩 Active open-source contributor — **Apache SeaTunnel**, **Mastra**, **Chroma**, **ContextGem**
- 🎓 M.Eng. student in Computer Science at **Guangzhou University** (2024–2027, GPA 3.96/5.0); research on **image generation & editing** with diffusion models (Stable Diffusion, CLIP, DreamBooth)
- 💬 Ask me about **LLM agents, RAG optimization, LLM evaluation, FastAPI, Spring Boot, or Vue.js**
- 🎯 Open to **AI application / full-stack development** opportunities (graduating June 2027) · 📍 **Guangzhou, China**

## 💼 Internship Experience

### 🛍️ AI Full-stack Intern · MINISO (Guangzhou) `Jun 2026 – Present`

> Building the group's **Agent platform** (centralized access, auth & governance for departmental agents) and the **evaluation + data flywheel** for MINISO's "XiaoMing" AI customer service.

- Designed centralized auth & routing on **Spring Cloud Gateway** — dual ordered `GlobalFilter`s with leaky-bucket rate limiting, covering OAuth authentication, cross-system token exchange, token validation, and unified downstream response wrapping
- Replaced full drop-and-rebuild permission sync with an **incremental diff-sync strategy** — computing the delta between old and new user sets and writing only changes in batches, cutting DB write volume and row-lock hold time
- Built an **RBAC** permission system on **Spring Security**, with reflection-based permission-integrity checks at startup that sync permission codes to the database
- Constructed a **~500-question offline eval set** for the AI customer service — covering core business, RAG retrieval, sentiment analysis, and safety compliance — with rule-based + **LLM-as-Judge** evaluators
- Designed the online **badcase reflow loop**: unified user- and agent-side feedback collection, dual-mode cross-validation, automatic attribution, and routed fixes flowing back into the eval set — closing the data loop

### 🤖 AI Application Development Intern · Xin'an Data Co., Ltd., Guangzhou `Mar 2026 – Jun 2026`

> A multi-agent report-review system for **China Southern Power Grid**: document parsing → knowledge-base construction → multi-agent collaborative review against historical reports and custom criteria.

- Orchestrated multi-node agent workflows in **Dify** with automatic report-type detection and type-based routing — turning a manually maintained knowledge base into a fully automated pipeline
- Optimized RAG retrieval with hierarchical Markdown chunking, **Milvus** Hybrid Search, and a **Reranker** — lifting QA accuracy from **60% to 88%**
- Built a multi-stage document-ingestion pipeline engine — queue-chained stages with independent intra-stage concurrency, enabling cross-stage parallel processing of bulk files
- Engineered an **OpenAI-compatible LLM connection pool** with multi-model dynamic routing, exponential-backoff retry, token-bucket rate limiting, and streaming

### ⚙️ AI Application Development Intern · Suanwei Technology Co., Ltd., Guangzhou `Jul 2025 – Oct 2025`

> A local-first AI office tool for confidentiality-sensitive archives: long-context document extraction plus CLIP-powered image search.

- Deployed the long-context **Qwen2.5-1M** model locally via **Ollama**, with **Nginx** multi-GPU load balancing supporting concurrent intranet users
- Combined **PaddleOCR** structured recognition with dynamic prompt templates over the ultra-long context window, extracting structured info from whole documents without chunk-boundary loss
- Designed a **multi-level caching strategy** — layering OCR intermediate states and extraction results — cutting repeated-query latency from minutes to milliseconds
- Implemented text-to-image and image-to-image search for massive asset libraries based on **CLIP** vision–language alignment

## 🚀 Featured Projects

### 🐾 Pet Wellness Advisor Agent `Dec 2025 – Feb 2026`

An AI-powered Q&A platform for pet owners: multi-agent orchestration, hybrid RAG, and knowledge-graph long-term memory — built solo, end to end.

- **Multi-agent orchestration** — LangGraph **Supervisor routing + Specialist executors** with parallel execution and ReAct-style tool calling; expert mode decomposes complex questions into a dependency-annotated **DAG**, layered by Kahn topological sort for same-layer parallel / cross-layer serial execution
- **Hybrid RAG** — vector + BM25 dual recall fused with **RRF**; parent–child chunk indexing (precise child matching, context-complete parent blocks); fine-grained reranking via `qwen3-rerank`
- **Knowledge-graph memory** — **Neo4j**-based long-term memory: ontology-constrained LLM triple extraction, two-layer entity dedup, vector + full-text + 1-hop-neighbor hybrid retrieval, **LPA** community clustering, and four-layer provenance (dialogue → chunk → statement → entity)

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### 🧪 LabMemory · Trusted Experiment Decision Platform `Jul 2026 – Aug 2026`

Team project for the **AI Pioneer Future Talent Competition** — a Feishu-embedded, full-link system for **AI for Science** experiment decisions: post-meeting review → parameter versioning → pre-action audit → task execution → result reflow → knowledge publishing.

- **Trusted decision kernel** — six quality gates, parameter-level versioning, a five-state knowledge lifecycle, and tri-valued audit trails with semantic guardrails and numeric conflict detection, so AI candidates never take effect unreviewed
- **Pre-action audit** — five pre-execution checks (version / evidence / approval / resource / failure boundary); stale-parameter references are automatically blocked with guided correction
- **Hybrid RAG** — BM25 + vector dual recall with multi-dimensional weighted reranking and relation expansion for trusted Q&A; streaming SSE output with multiple refusal paths
- **Experiment Passport** — every result traces back to the original meeting transcript, and every decision exposes its downstream impact, organized by meeting relation chains and experiment timelines

## 🌱 Open Source Contributions

- [**apache/seatunnel**](https://github.com/apache/seatunnel) (9.6k★) — Pulsar connector declarative-validation migration with 14 factory validation tests ([PR #11985](https://github.com/apache/seatunnel/pull/11985), in review)
- [**mastra-ai/mastra**](https://github.com/mastra-ai/mastra) (27.5k★) — fixed MCP `tools/call` responses dropping `_meta` / `ui.resourceUri`, mirroring `tools/list` normalization so third-party MCP hosts can render MCP Apps, with integration tests ([PR #22454](https://github.com/mastra-ai/mastra/pull/22454), in review)
- [**chroma-core/chroma**](https://github.com/chroma-core/chroma) — migrated the Gemini example off deprecated SDK APIs ([PR #7637](https://github.com/chroma-core/chroma/pull/7637), in review)
- [**shcherbak-ai/contextgem**](https://github.com/shcherbak-ai/contextgem) (2k★) — reported the Gemma3 vision-capability misdetection, confirmed and fixed in **v0.12.1** with an explicit vision-capability option ([issue #47](https://github.com/shcherbak-ai/contextgem/issues/47) → [PR #49](https://github.com/shcherbak-ai/contextgem/pull/49))

## 🔬 Research & Publications

My research focuses on **image generation and editing**: cross-modal representations (CLIP), diffusion models (VAE / DDPM / DDIM), personalized fine-tuning (Textual Inversion, DreamBooth), and classic editing methods (Instruct-Pix2Pix, PnP).

- 📄 *EmoPrompt+: Emotional Image Content Generation via Emotion-Driven Prompting and Multi-Level Emotional Guidance in Stable Diffusion* — **CCBR 2025** (accepted)
- 📄 *C-EmoEditor: Affective Image Editing Based on Valence-Arousal Model* — **The Visual Computer** (under review)

## 🏆 Honors & Certifications

- 🥇 Graduate Academic Scholarships (1st & 2nd Prize), Guangzhou University · First-Class Scholarship & National Encouragement Scholarship, Huizhou University
- 🏅 Lanqiao Cup Java Development (Graduate Division) · Guangdong 3rd Prize · National College Student Software Testing Contest (Developer Testing) · Provincial 3rd Prize
- 📜 CET-6 · Software Designer certification (China Soft Exam)

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)

**LLM & Agents**

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![Dify](https://img.shields.io/badge/Dify-155EEF?style=flat-square&logo=dify&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![LoRA](https://img.shields.io/badge/LoRA-fine--tuning-8A2BE2?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5E5CE6?style=flat-square)

**Backend & Data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

**Tools & Infra**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![PaddleOCR](https://img.shields.io/badge/PaddleOCR-2932E1?style=flat-square)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)

---

<div align="center">

🔥 Keep shipping —

<img src="https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FLinz1248%2FLinz1248%2Fmain%2Fassets%2Fcontributions-badge.json&style=flat-square" alt="Johan's GitHub contributions in 2026, updated daily via GitHub Actions" />

</div>
