<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=Pritish%20Sharma&fontSize=55&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Data%20Scientist%20|%20AI/ML%20Engineer%20|%20MLOps&descAlignY=55&descSize=19" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=21&duration=2800&pause=1200&color=38BDF8&center=true&vCenter=true&width=750&lines=Building+RAG+pipelines+%26+multi-agent+LLM+systems;Privacy-aware%2C+cost-aware+AI+architectures;Data+Science+%7C+LangGraph+%7C+LangChain+%7C+MCP+%7C+AWS+%7C+ML;Systems+that+are+verifiably+correct%2C+not+just+plausible" alt="Typing SVG"/>

<a href="https://www.linkedin.com/in/pritishsharma230805/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:pritishsharma08@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://github.com/Pritish-23"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>

</div>

<br/>

## 👋 About Me

- 🎓 B.Sc. Data Science, Thakur College of Science and Commerce — **CGPA 8.12** (2023–2026)
- 🧠 I build **end-to-end ML & AI systems** — RAG pipelines, multi-agent LLM orchestration, and production deployment
- 🔐 Focused on **privacy-preserving, cost-aware AI architecture** — systems that are correct by design, not just plausible-sounding
- ⚙️ Full MLOps stack: **Docker → AWS/Railway → GitHub Actions CI/CD**
- 📊 Strong foundations in classic ML, NLP, and data visualization alongside modern LLM tooling
- 💬 Ask me about: LangGraph orchestration, RAG evaluation harnesses, or deterministic-vs-LLM system design

<br/>

## 🧬 Core Stack

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge"/>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/Anthropic_Claude-D97757?style=for-the-badge"/>
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white"/>
<br/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
<img src="https://img.shields.io/badge/ChromaDB-FF6F00?style=for-the-badge"/>
<img src="https://img.shields.io/badge/FAISS-4285F4?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
<br/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
<img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
<img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
</p>

<br/>

## 🚀 Featured Projects

### 🧭 TieredFlow — Cost/Latency-Aware Multi-Agent LLM Orchestrator

```mermaid
flowchart LR
    A[📩 Incoming Query] --> B{Task Classifier}
    B --> C1[⚡ Groq<br/>Fast Tier]
    B --> C2[🔹 Claude Haiku<br/>Balanced Tier]
    B --> C3[🔷 Claude Sonnet<br/>Premium Tier]
    B --> C4[🌐 OpenAI<br/>Fallback Tier]
    C1 & C2 & C3 & C4 --> D[🧠 Semantic Cache<br/>FAISS + Embeddings]
    D -->|high similarity| E[✅ Auto-serve]
    D -->|mid similarity| F[🙋 Human-in-loop approval]
    D -->|low similarity| G[🔁 Full LLM call]
    G --> H[💾 SQLite Checkpointing<br/>Resumable State]

    style A fill:#0f2027,color:#fff
    style B fill:#203a43,color:#fff
    style D fill:#2c5364,color:#fff
    style H fill:#38BDF8,color:#000
```

Multi-agent **LangGraph** pipeline routing queries across four cost/latency tiers under real-time budget constraints, with automatic downgrade when budget runs low. Semantic caching (FAISS + Sentence-Transformers) cuts redundant LLM calls via a tiered transparency model — auto-serve, human-in-the-loop, or full bypass depending on similarity. Includes 5 integrated tools with fallback chains, confidence scoring, a multi-case evaluation harness, and a live-routing Streamlit UI with one-click CSV export.

`LangGraph` `LangChain` `LangSmith` `Anthropic/OpenAI/Groq` `FAISS` `SQLite` `Streamlit`

---

### 🔒 Tax Filing RAG Assistant — Privacy-First AI System

Privacy-by-design system aligned with India's **DPDP Act**: per-session ChromaDB collections are physically incapable of persisting beyond session end, enforced at the runtime level with a 20-minute TTL sweep. Tax math (slab rates, surcharge, cess, 87A rebate, HRA exemption) is computed in **pure deterministic Python — never delegated to the LLM** — achieving 100% regime recommendation accuracy across synthetic personas from ₹6L–₹50L income. A LangSmith redaction layer strips PII before traces leave the process.

| Metric | Result |
|---|---|
| Field extraction accuracy | **100%** (130/130 checks) |
| Regime recommendation accuracy | **100%** |
| RAG faithfulness / relevance | **89.3%** |

Deployed as independent FastAPI + Streamlit services on Railway via Docker, gated by threshold-based GitHub Actions CI on every push.

`FastAPI` `Streamlit` `ChromaDB` `Claude Haiku` `LangSmith` `Docker` `Railway`

---

### 🚗 Vehicle Insurance Cross-Sell Prediction — MLOps Pipeline

Production-grade MLOps pipeline: MongoDB Atlas ingestion → schema validation → transformation → training → evaluation, with automated retraining support. Containerized with Docker and deployed on AWS EC2; model artifacts versioned on S3 for reproducible runs and rollback. CI/CD via GitHub Actions + AWS ECR enables zero-touch redeployment on every push to main. Flask prediction API with a web UI for real-time inference.

`Scikit-learn` `MongoDB` `Docker` `AWS EC2/ECR/S3` `GitHub Actions` `Flask`

<br/>

## 📊 GitHub Stats

<p align="center"> <img height="165" src="https://github-readme-stats-sigma-five.vercel.app/api?username=Pritish-23&show_icons=true&theme=tokyonight&hide_border=true&count_private=true"/> <img height="165" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=Pritish-23&layout=compact&theme=tokyonight&hide_border=true"/> </p> <p align="center"> <img src="https://streak-stats.demolab.com?user=Pritish-23&theme=tokyonight&hide_border=true"/> </p> <p align="center"> <img src="https://github-readme-activity-graph.vercel.app/graph?username=Pritish-23&theme=tokyo-night&hide_border=true"/> </p> <div align="center"> <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer"/> </div>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Pritish-23&theme=tokyo-night&hide_border=true"/>
</p>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer"/>
</div>
