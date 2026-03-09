<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:58a6ff&height=120&section=header" />

<h1 align="center">David Aguilar</h1>

<p align="center">
<strong>Senior AI Engineer</strong> &nbsp;·&nbsp; System Architecture &nbsp;·&nbsp; Digital Transformation &nbsp;·&nbsp; Production ML
</p>

<p align="center">
<a href="https://www.linkedin.com/in/aguilardavidp/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>&nbsp;
<a href="mailto:david.aguilar@pucp.edu.pe"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

<br>

I architect and ship AI systems that transform business operations — not prototypes. I've replaced manual clinical audits at hospitals with automated pipelines, turned WhatsApp into a sales channel with AI agents closing real transactions, and deployed computer vision on factory production lines. I make the technical decisions on model selection, system design, and infrastructure, and I own the outcome from architecture to production.

<table>
<tr>
<td>🎓</td>
<td><strong>MSc Artificial Intelligence</strong> — Pontificia Universidad Catolica de Chile</td>
</tr>
<tr>
<td>🎓</td>
<td><strong>BSc Mechatronics Engineering</strong> — Pontificia Universidad Catolica del Peru</td>
</tr>
<tr>
<td>📍</td>
<td>Lima, Peru &nbsp;·&nbsp; Open to remote</td>
</tr>
</table>

<br>

## Systems I've Designed & Deployed

<table>
<tr>
<td width="100%" valign="top">

### Clinical Audit Automation — Healthcare
<img src="https://img.shields.io/badge/Highest_Complexity-Private_Repo-6B7280?style=flat-square" alt="Private"/> <img src="https://img.shields.io/badge/Production-Deployed-00C853?style=flat-square" alt="Deployed"/>

Designed and built the full AI platform that replaced manual clinical audits at a major hospital. Multi-stage pipeline: document ingestion (OCR + layout parsing), medical NLP classification, rule engine for compliance validation, and structured reporting with audit trails.

**Architectural decisions I owned:**
- Chose a hybrid extraction pipeline (OCR + layout-aware parsing) over pure LLM extraction for regulatory compliance — the system needed deterministic, auditable outputs
- Designed the classification layer to separate medical coding from compliance rules, making each independently testable
- Built the reporting module to generate structured outputs that integrate directly with the hospital's existing audit workflow

**Business impact:** Transformed a multi-person manual process into an automated pipeline. Reduced audit processing time from days to minutes while maintaining regulatory compliance standards.

`Python` `TensorFlow` `OCR` `NLP` `FastAPI` `PostgreSQL` `Docker`

</td>
</tr>
</table>

<table>
<tr>
<td width="50%" valign="top">

### WhatsApp Sales Agent — Telecom
<img src="https://img.shields.io/badge/Production-Live-00C853?style=flat-square" alt="Live"/>

Digitized the phone sales channel for a major telecom operator. Architected the agentic pipeline: intent detection, catalog recommendation with personalized pricing, CRM integration, real-time payment processing. Serving real customers via WhatsApp.

**Key decisions:** LangGraph orchestration, RAG with Qdrant + CrossEncoder for objection handling, Redis-backed state with HITL confirmation flows. Designed the system to handle concurrent conversations with message buffering and per-user locking.

`LangGraph` `FastAPI` `RAG` `Qdrant` `WhatsApp API` `Redis`

</td>
<td width="50%" valign="top">

### Industrial Quality Control — Manufacturing
<img src="https://img.shields.io/badge/Production-Deployed-00C853?style=flat-square" alt="Deployed"/>

Brought AI to the factory floor. Real-time defect detection integrated with PLC Beckhoff automation on actual production lines. Designed the full system: CNN inference, operator HMI, and automated reject logic with hard real-time constraints.

**Key decisions:** TensorFlow Lite for edge inference latency, custom protocol bridge between Python and PLC via pyads, fail-safe logic ensuring production continuity when the model is uncertain.

`TensorFlow` `OpenCV` `pyads` `PLC Beckhoff` `CustomTkinter`

</td>
</tr>
</table>

<br>

## Featured Open Source

<table>
<tr>
<td>

### [vendedor-ai](https://github.com/DavidAguilarParedes/vendedor-ai) — AI Sales Agent for WhatsApp

Open-source version of my production sales agent, rebuilt from scratch to demonstrate system design. Custom agentic orchestrator (no LangGraph), multi-LLM support (Claude + GPT-5 + GPT-4o), 10 tools, 3 human-in-the-loop checkpoints.

**Why I built it custom instead of using LangGraph:**
- The original production system used LangGraph, but `create_react_agent()` hides the engineering — 15 lines of config don't show that you understand how agentic loops work
- The custom orchestrator is ~200 lines of explicit Python: tool execution, HITL pause/resume with Redis state, auto-actions that bypass the LLM when reliability matters
- Unified LLM abstraction that handles Anthropic and OpenAI quirks (different tool calling formats, `max_tokens` vs `max_completion_tokens`)

`Claude API` `OpenAI API` `FastAPI` `Redis` `Pydantic` `Docker` `WhatsApp Cloud API`

<a href="https://github.com/DavidAguilarParedes/vendedor-ai">
<img src="https://img.shields.io/badge/View_Source-58A6FF?style=for-the-badge&logo=github&logoColor=white" alt="View Source"/>
</a>

</td>
</tr>
<tr>
<td>
<img src="https://raw.githubusercontent.com/DavidAguilarParedes/vendedor-ai/master/docs/assets/panel_vendedor_ai.png" alt="vendedor-ai — WhatsApp mock + agent trace viewer" width="100%"/>
</td>
</tr>
</table>

<table>
<tr>
<td width="50%" valign="top">

### [Scientific RAG System](https://github.com/DavidAguilarParedes/mia-uc-chile-proyecto-aplicado-1)
End-to-end RAG pipeline for scientific literature. Document ingestion, embeddings, vector search, reranking, answer synthesis with evaluation framework. MSc applied project at UC Chile.

`LangChain` `FAISS` `OpenAI` `Python`

</td>
<td width="50%" valign="top">

### [Industrial QC — CNN + PLC](https://github.com/DavidAguilarParedes/Lab-IA-1MTR56-Automatizacion-Industrial-Inteligente)
CNN image classification integrated with PLC Beckhoff for factory quality control. Custom HMI for operators, real-time inference, automated rejection.

`TensorFlow` `OpenCV` `pyads` `PLC Beckhoff`

</td>
</tr>
</table>

<br>

## Technical Depth

<p align="center">
<img src="https://skillicons.dev/icons?i=python,tensorflow,pytorch,fastapi,docker,redis,postgres,aws,linux,git&theme=dark" alt="Tech Stack" />
</p>

| Area | Technologies |
|------|-------------|
| **LLM & Agent Systems** | Claude API, OpenAI API, LangChain, LangGraph, custom agentic loops, tool use, RAG (FAISS, Qdrant), HITL patterns, prompt engineering, multi-model orchestration |
| **ML / Deep Learning** | TensorFlow, PyTorch, scikit-learn, Hugging Face, computer vision, NLP, OCR, document AI |
| **System Architecture** | Microservices, async Python, FastAPI, Redis, PostgreSQL, Docker Compose, event-driven design, API design, state management |
| **Industrial Automation** | PLC Beckhoff (TwinCAT), pyads, OPC-UA, OpenCV, SCADA, real-time inference, edge deployment |
| **Process & Strategy** | AI system design, build-vs-buy evaluation, production readiness, technical documentation, cross-functional delivery |

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:58a6ff&height=80&section=footer" />
