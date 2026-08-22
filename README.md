<div align="center">

# Johan Lin

**AI Application Developer · Full Stack Development · M.Eng. CS @ Guangzhou University**

[![Profile views](https://komarev.com/ghpvc/?username=Linz1248&label=Profile+views&color=0e75b6&style=flat-square)](https://github.com/Linz1248)
[![Email](https://img.shields.io/badge/Email-1552855968%40qq.com-D14836?style=flat-square)](mailto:1552855968@qq.com)

</div>

---

## 🧑‍💻 About Me

- 🔭 I build **LLM-powered agent systems** and **full-stack apps** — multi-agent orchestration, hybrid RAG pipelines, and end-to-end services with **LangGraph / LangChain**, **FastAPI** and **Vue.js**
- 🌱 M.Eng. student in Computer Science at **Guangzhou University** (2024–2027); my research focuses on **image generation & editing** with diffusion models (Stable Diffusion, CLIP, DreamBooth)
- 💬 Ask me about **LLM agents, RAG optimization, FastAPI, Spring Boot, or Vue.js**
- 🎯 Open to **AI application / full-stack development** opportunities (graduating June 2027)
- 📍 Based in **Guangzhou, China**

## 💼 Internship Experience

### 🤖 AI Development Intern · Xin'an Data Co., Ltd., Guangzhou `Mar 2026 – Jun 2026`

> A Dify-based intelligent agent for project-report review, analyzing new proposals against historical reports and custom criteria.

- Co-built an **NL2SQL agent** and designed a version-based optimistic-locking mechanism to keep multi-user concurrent edits consistent
- Designed a chapter-level document chunking strategy — LLM-based heading classification with rule-based fallback for out-of-taxonomy documents
- Built a multi-stage concurrent ingestion pipeline (independent stages chained by queues) enabling cross-stage parallel processing of bulk files

### ⚙️ Algorithm Intern · Suanwei Technology Co., Ltd., Guangzhou `Jul 2025 – Oct 2025`

> A local-first AI office tool for confidentiality-sensitive archives: long-context document extraction plus CLIP-powered image search.

- Deployed the long-context **Qwen2.5-1M** model locally via **Ollama**, with **Nginx** multi-GPU load balancing
- Combined **PaddleOCR** structured recognition with dynamic prompt templates to extract targeted information via the LLM's long context window
- Designed a **multi-level caching strategy** (intermediate OCR states + extraction results), cutting response latency from minutes to milliseconds
- Implemented image-to-image and text-to-image search based on **CLIP** vision–language alignment

## 🚀 Featured Projects

### 🐾 Pet Wellness Advisor Agent

An AI-powered Q&A platform for pet owners: private knowledge bases, long-term user memory profiles, multi-expert collaboration, and an extensible skill-plugin marketplace.

- **Multi-agent orchestration** — Supervisor routing node + Specialist executors built on LangGraph, with parallel task execution and ReAct-style tool calling
- **Hybrid RAG** — dual-channel vector + BM25 recall fused with RRF, parent–child chunk indexing, and fine-grained reranking via `qwen3-rerank`
- **Knowledge-graph memory** — Neo4j-based long-term memory with an LLM triple-extraction pipeline, entity deduplication, community clustering, and four-layer provenance

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### 🧭 Multi-Agent Travel Planner · [GitHub](https://github.com/Linz1248/trip-planner) `Oct 2025 – Dec 2025`

A multi-agent travel planning system built on **LangGraph**, integrating the AMap (Gaode) Maps API for intelligent itinerary generation — attraction search, weather checks, and hotel filtering rolled into personalized daily plans.

- Designed a Supervisor/Specialist multi-agent architecture with shared workflow state for cross-stage information passing
- Implemented **dynamic MCP tool binding** — agents asynchronously discover and invoke external tools at runtime
- Exposed RESTful services via FastAPI with real-time POI, routing, and weather queries

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-Model_Context_Protocol-5E5CE6?style=flat-square)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)

## 🔬 Research & Publications

My research focuses on **image generation and editing**: cross-modal representations (CLIP), diffusion models (VAE / DDPM / DDIM), personalized fine-tuning (Textual Inversion, DreamBooth), and classic editing methods (Instruct-Pix2Pix, PnP).

- 📄 *EmoPrompt+: Emotional Image Content Generation via Emotion-Driven Prompting and Multi-Level Emotional Guidance in Stable Diffusion* — **CCBR 2025** (accepted)
- 📄 *C-EmoEditor: Affective Image Editing Based on Valence-Arousal Model* — **The Visual Computer** (under review)

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

**Backend & Data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)
![Milvus](https://img.shields.io/badge/Milvus-00A1EA?style=flat-square)

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
