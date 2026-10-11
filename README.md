<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,50:161b22,100:58a6ff&height=240&section=header&text=Bishwajit%20Chakraborty&fontSize=60&fontAlignY=36&fontColor=c9d1d9&desc=AI%20%E2%80%A2%20Backend%20%E2%80%A2%20Multi-Agent%20LLM%20Systems%20%E2%80%A2%20MCP&descAlignY=58&descSize=18&animation=fadeIn" alt="header banner" />

<a href="https://github.com/Bishwajit-2810">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=24&duration=2800&pause=900&color=58a6ff&center=true&vCenter=true&width=940&lines=AI+%26+Backend+Engineer;Architecting+Multi-Agent+LLM+Platforms+with+LangGraph;Building+MCP+Servers+%2B+RAG+Pipelines+over+pgvector;Ex-Software+Engineer+Intern+(AI+%26+Backend)+%40+Cloudly+Infotech;FastAPI+%E2%80%A2+FastMCP+%E2%80%A2+LangChain+%E2%80%A2+Flutter;From+Dhaka%2C+Bangladesh+%F0%9F%87%A7%F0%9F%87%A9" alt="typing-banner" />
</a>

<br />

<a href="https://bishwajit.app"><img src="https://img.shields.io/badge/Portfolio-bishwajit.app-0d1117?style=for-the-badge&logo=googlechrome&logoColor=58a6ff&labelColor=161b22" alt="portfolio" /></a>
<a href="https://www.linkedin.com/in/bishwajit-chakraborty/"><img src="https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=58a6ff&labelColor=161b22" alt="linkedin" /></a>
<a href="mailto:bishwajit2810@gmail.com"><img src="https://img.shields.io/badge/Gmail-0d1117?style=for-the-badge&logo=gmail&logoColor=EA4335&labelColor=161b22" alt="email" /></a>
<a href="https://github.com/Bishwajit-2810"><img src="https://komarev.com/ghpvc/?username=Bishwajit-2810&label=Profile+Views&color=0d1117&style=for-the-badge&labelColor=161b22" alt="profile views" /></a>
<a href="https://github.com/Bishwajit-2810?tab=followers"><img src="https://img.shields.io/github/followers/Bishwajit-2810?label=Followers&style=for-the-badge&color=0d1117&labelColor=161b22" alt="followers" /></a>
<img src="https://img.shields.io/badge/Open%20to-Opportunities-0d1117?style=for-the-badge&labelColor=161b22&color=0d1117" alt="open to opportunities" />

</div>

## <picture><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28" /></picture> &nbsp;About Me

```yaml
name: "Bishwajit Kumar Chakraborty"
role: "AI & Backend Engineer"
experience: "Ex-Software Engineer Intern (AI & Backend) @ Cloudly Infotech (Feb 2026 – Aug 2026)"
education: "B.Sc. CSE — Daffodil International University (Aug 2022 – Sep 2026)"
status: "All coursework completed (CGPA: 3.72 / 4.00)"
location: "Dhaka, Bangladesh 🇧🇩"
portfolio: "https://bishwajit.app"

building:
  - "🧠 Production multi-agent LLM systems (LangGraph & FastAPI)"
  - "🔌 MCP servers (FastMCP + SSE) & custom agent toolkits"
  - "🔍 High-recall RAG pipelines (hybrid pgvector + lexical search, breadcrumb chunking)"
  - "🛡 Robust backend architectures (FastAPI, Alembic, PostgreSQL, MinIO/S3)"

current_focus: [Healthcare AI & analytics, Advanced RAG eval, LoRA/QLoRA fine-tuning]
interests: [Agentic AI, LLM Ops, System Design, Healthcare Analytics, DSA]
mantra: "ship secure · ship explainable · ship measurable"
```

---

## <picture><img src="https://media.giphy.com/media/iY8CRBdQXODJSCERIr/giphy.gif" width="28" /></picture> &nbsp;Work Experience

<table>
<tr>
<td>

### 🏥 Software Engineer Intern (AI & Backend) — Cloudly Infotech Limited
**Feb 2026 – Aug 2026** *(Completed)* $\cdot$ Full-time $\cdot$ On-site, Dhaka  
*Clinical decision-support platform powered by LangGraph multi-agent systems, RAG, and FHIR/OpenEMR*

- 🧠 **Multi-Agent LLM Platform:** Engineered a production multi-agent system on **LangGraph** and **FastAPI**; fixed orchestrator defects misrouting queries between Diagnostic and Treatment agents via state graphs, conditional routing, and refined system prompts.
- 📑 **RAG Ingestion Overhaul:** Led a comprehensive ingestion overhaul improving retrieval quality through **heading-hierarchy breadcrumb chunking**, **table-aware atomic chunking**, list-boundary splitting, and font-size heading inference for unstructured clinical PDFs.
- ⚡ **Hybrid Search & Object Storage:** Implemented hybrid vector + full-text search over **pgvector** (Postgres `tsv` generated column, Alembic migrations incl. multi-head merge) and built an async **MinIO/S3** ingestion pipeline (`aioboto3`) with a resumable, idempotent CLI uploader.
- 🛡 **Clinical Integration & Test Gates:** Enhanced **FHIR-backed patient search** (exact full-name, title-inclusive matching) and clinical-note PDF export; authored **80+ tests** across 15 modules enforced under `ruff`/`black` CI gates.

</td>
</tr>
</table>

---

## <picture><img src="https://media.giphy.com/media/QssGEmpkyEOhNN7eM1/giphy.gif" width="28" /></picture> &nbsp;Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🤖 [GitHub MCP Suite](https://github.com/Bishwajit-2810/GitHubMCPOfficial)
*Full-Stack GitHub Automation with AI & MCP*  
`FastMCP` · `FastAPI` · `pgvector` · `Flutter` · `PostgreSQL` · `Firebase Auth`

- Built a production-grade **MCP server** (12 tools via FastMCP/SSE) for repository management, GitHub Projects v2 (GraphQL), branch/PR automation, and **RAG-powered codebase Q&A** using pgvector for semantic retrieval.
- Architected a **BFF API layer** (FastAPI + SQLAlchemy + Alembic + PostgreSQL) with Firebase Auth, GitHub OAuth 2.0, JWT signing, and **Fernet-encrypted token storage**.
- Created a cross-platform **Flutter mobile app** (Riverpod) with real-time streaming agent responses.
- Set up **GitHub Actions CI** on every PR: `pgvector:pg16` service container, `uv` sync, `black --check`, **34 pytest tests** on API + **67 Flutter tests**.

</td>
<td width="50%" valign="top">

### 🗳️ [Secure Voting System](https://github.com/Bishwajit-2810/VotingSystem)
*Backend REST API with Role-Based Access Control*  
`Node.js` · `Express` · `MongoDB` · `JWT` · `Docker` · `Jest`

- REST API for electronic voting featuring **JWT authentication**, **role-based access control** (voter/admin), atomic vote enforcement preventing double-voting, and bcrypt password hashing.
- Hardened for operations: **Zod** request validation, centralised error middleware, structured **Winston** log rotation, and full **docker-compose** containerisation.
- Backed by **61 Jest/Supertest tests** across 5 suites with **75% statement / 85% branch coverage** (100% on JWT module), isolated via `mongodb-memory-server`.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💧 [Water Quality Monitoring System](https://github.com/Bishwajit-2810/WMS_Backend)
*LoRa IoT Pipeline + AI Diagnostic Engine*  
`Node.js` · `MongoDB` · `Flutter` · `Gemini API` · `LoRa`

- Built an end-to-end IoT pipeline collecting pH, turbidity, TDS, and flow rate from LoRa sensors into MongoDB with schema-validated documents and automatic threshold alerting.
- Integrated **Gemini API** for AI-driven multi-parameter water quality analysis and anomaly detection, generating natural language health assessments and recommendations.
- Delivered a **Flutter real-time dashboard** with live sensor telemetry, historical trend charts, and push alerts; presented to industry leaders at DIU.  
👉 [Backend Repo](https://github.com/Bishwajit-2810/WMS_Backend) · [Frontend Repo](https://github.com/Bishwajit-2810/water_monitor)

</td>
<td width="50%" valign="top">

### 🖥️ [Local LLM Desktop Assistant](https://github.com/Bishwajit-2810/Local_LLM_Project)
*Zero-Cloud AI Assistant with System Monitor*  
`Python` · `Ollama` · `Tkinter` · `psutil` · `STT/TTS`

- Engineered a 100% offline desktop AI assistant powered by **Ollama** with a modular plugin architecture for hot-swapping LLM backends without restarting.
- Built a real-time **CPU/RAM/GPU telemetry** overlay via `psutil` and platform-native APIs, streamed to UI and optionally injected into LLM context for hardware-aware responses.
- Integrated end-to-end **voice interaction** via STT/TTS pipelines with configurable wake-word detection, model switching, and session management.

</td>
</tr>
</table>

---

## <picture><img src="https://media.giphy.com/media/LMcB8XospGZO8UQq87/giphy.gif" width="28" /></picture> &nbsp;Tech Arsenal

<div align="center">

<table>
<tr>
<td align="center" width="33%">

**🧠 &nbsp;LLM · Agents · ML**

<img src="https://skillicons.dev/icons?i=python,tensorflow,sklearn&perline=5" />

`LangChain` · `LangGraph` <br/>
`MCP` · `FastMCP` · `RAG` <br/>
`Ollama` · `HuggingFace` <br/>
`LoRA/QLoRA` · `Gemini API`

</td>
<td align="center" width="33%">

**⚙️ &nbsp;Backend · APIs**

<img src="https://skillicons.dev/icons?i=fastapi,nodejs,express,graphql,postman&perline=5" />

`FastAPI` · `FastMCP` · `SSE` <br/>
`Node.js` · `Express.js` <br/>
`SQLAlchemy` · `Alembic` <br/>
`Pydantic` · `REST` · `GraphQL`

</td>
<td align="center" width="33%">

**💻 &nbsp;Languages**

<img src="https://skillicons.dev/icons?i=py,js,cpp,java,dart&perline=5" />

`Python` · `JavaScript` <br/>
`Dart` · `C++` · `Java`

</td>
</tr>
<tr>
<td align="center">

**🗄 &nbsp;Databases & Storage**

<img src="https://skillicons.dev/icons?i=postgres,mongodb,mysql&perline=5" />

`PostgreSQL` · `pgvector` <br/>
`Postgres Full-Text (tsv)` <br/>
`MinIO / S3 (aioboto3)` <br/>
`ChromaDB` · `MongoDB` · `MySQL`

</td>
<td align="center">

**🔐 &nbsp;Auth & Security**

<img src="https://skillicons.dev/icons?i=firebase&perline=5" />

`Firebase Auth` · `JWT` <br/>
`OAuth 2.0` · `Fernet Encryption` <br/>
`bcrypt` · `RBAC`

</td>
<td align="center">

**🧰 &nbsp;DevOps, Testing & Tools**

<img src="https://skillicons.dev/icons?i=docker,git,linux,flutter,react,vscode&perline=6" />

`pytest` · `ruff / black` · `Jest` <br/>
`Docker` · `GitHub Actions CI` <br/>
`Flutter (Riverpod)` · `React` <br/>
`Arch Linux` · `Git`

</td>
</tr>
</table>

</div>

---

## <picture><img src="https://media.giphy.com/media/tHIRLUV5oTcTm/giphy.gif" width="28" /></picture> &nbsp;Education & Certifications

<table>
<tr>
<td width="50%" valign="top">

### 🎓 Education

- **B.Sc. in Computer Science & Engineering**  
  *Daffodil International University* · **Aug 2022 – Sep 2026**  
  **CGPA:** 3.72 / 4.00 · *All coursework completed*
- **Higher Secondary Certificate (HSC) — Science**  
  *Gurudayal Govt. College* · **2019 – 2021**  
  **GPA:** 5.00 / 5.00

</td>
<td width="50%" valign="top">

### 📜 Certifications & Training

- **AI+ Prompt Engineer Level 1™** — AI CERTs® *(Jun 2025)*
- **Agent X Certified** — NetCom Learning® *(Sep 2025)*
- **5-Day AI Agents Intensive** — Google & Kaggle *(Nov 2025)*
- **AI-Powered Learning Processing Workshop** — DIU NLP & ML Research Lab *(2025)*

</td>
</tr>
</table>

---

## <picture><img src="https://media.giphy.com/media/SWoSkN6DxTszqIKEqv/giphy.gif" width="28" /></picture> &nbsp;GitHub Activity

<div align="center">

<a href="https://github.com/Bishwajit-2810">
  <img alt="GitHub stats" height="170" src="https://github-readme-stats.shion.dev/api?username=bishwajit-2810&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=bc8cff&text_color=c9d1d9&include_all_commits=true&count_private=true&rank_icon=github" />
  <img alt="Top languages" height="170" src="https://github-readme-stats.shion.dev/api/top-langs/?username=bishwajit-2810&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=10" />
</a>

<a href="https://github.com/Bishwajit-2810">
  <img alt="GitHub streak" src="https://streak-stats.demolab.com?user=bishwajit-2810&theme=tokyonight&hide_border=true&background=0d1117&ring=58a6ff&fire=bc8cff&currStreakLabel=58a6ff&sideNums=c9d1d9&sideLabels=c9d1d9&dates=8b949e&stroke=58a6ff" />
</a>

<!-- <img alt="commits heartbeat activity graph" src="https://github-readme-activity-graph.vercel.app/graph?username=Bishwajit-2810&custom_title=Commits%20Heartbeat&bg_color=0d1117&color=58a6ff&line=bc8cff&point=bc8cff&title_color=58a6ff&area_color=58a6ff&hide_border=true&area=true" /> -->

</div>

---

## <picture><img src="https://media.giphy.com/media/jpVnC65DmYeyRL4LHS/giphy.gif" width="28" /></picture> &nbsp;Let's Connect

<div align="center">

<a href="https://bishwajit.app"><img src="https://img.shields.io/badge/Portfolio-bishwajit.app-0d1117?style=for-the-badge&logo=googlechrome&logoColor=58a6ff&labelColor=161b22" alt="portfolio" /></a>
<a href="mailto:bishwajit2810@gmail.com"><img src="https://img.shields.io/badge/Gmail-0d1117?style=for-the-badge&logo=gmail&logoColor=EA4335&labelColor=161b22" alt="email" /></a>
<a href="https://www.linkedin.com/in/bishwajit-chakraborty/"><img src="https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=58a6ff&labelColor=161b22" alt="linkedin" /></a>
<a href="https://github.com/Bishwajit-2810"><img src="https://img.shields.io/badge/GitHub-0d1117?style=for-the-badge&logo=github&logoColor=c9d1d9&labelColor=161b22" alt="github" /></a>
<a href="https://twitter.com/bishwajit_2810"><img src="https://img.shields.io/badge/X-0d1117?style=for-the-badge&logo=x&logoColor=c9d1d9&labelColor=161b22" alt="x" /></a>
<a href="https://www.leetcode.com/bishwajit2810"><img src="https://img.shields.io/badge/LeetCode-0d1117?style=for-the-badge&logo=leetcode&logoColor=d29922&labelColor=161b22" alt="leetcode" /></a>
<a href="https://dev.to/bishwajit2810"><img src="https://img.shields.io/badge/Dev.to-0d1117?style=for-the-badge&logo=devdotto&logoColor=c9d1d9&labelColor=161b22" alt="devto" /></a>
<a href="https://fb.com/bishwajit.2810"><img src="https://img.shields.io/badge/Facebook-0d1117?style=for-the-badge&logo=facebook&logoColor=58a6ff&labelColor=161b22" alt="facebook" /></a>
<a href="https://instagram.com/bishwajit_2810/"><img src="https://img.shields.io/badge/Instagram-0d1117?style=for-the-badge&logo=instagram&logoColor=f85149&labelColor=161b22" alt="instagram" /></a>

</div>

---

<div align="center">

<sub>⭐ &nbsp;If something here sparked an idea, feel free to connect or follow — I build and ship practical AI & backend systems. &nbsp;⭐</sub>

</div>
