<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:58a6ff&height=120&section=header" />

<h1 align="center">David Aguilar</h1>

<p align="center">
<strong>AI Engineer</strong> &nbsp;·&nbsp; Production ML Systems &nbsp;·&nbsp; Conversational AI &nbsp;·&nbsp; Industrial Automation
</p>

<p align="center">
<a href="https://www.linkedin.com/in/aguilardavidp/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>&nbsp;
<a href="mailto:david.aguilar@pucp.edu.pe"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

<br>

I build AI systems that run in production — from WhatsApp sales agents processing real transactions to CNN classifiers on factory inspection lines. I focus on the full pipeline: model development, system architecture, deployment, and maintenance.

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

## Featured Project

<table>
<tr>
<td>

### [vendedor-ai](https://github.com/DavidAguilarParedes/vendedor-ai) — AI Sales Agent for WhatsApp

End-to-end conversational sales agent: custom agentic orchestrator, 10 tools, 3 human-in-the-loop checkpoints, multi-LLM support (Claude + GPT-5 + GPT-4o). Handles the complete purchase flow — catalog browsing, product selection, address validation, delivery scheduling, and order confirmation.

**Not a wrapper around LangGraph.** The orchestrator is ~200 lines of explicit Python: agentic loop, tool execution, HITL pause/resume with Redis state, auto-actions that bypass the LLM for reliability.

`Claude API` `OpenAI API` `FastAPI` `Redis` `Pydantic` `Docker` `WhatsApp Cloud API`

<a href="https://github.com/DavidAguilarParedes/vendedor-ai">
<img src="https://img.shields.io/badge/View_Project-58A6FF?style=for-the-badge&logo=github&logoColor=white" alt="View Project"/>
</a>

</td>
</tr>
<tr>
<td>
<img src="https://raw.githubusercontent.com/DavidAguilarParedes/vendedor-ai/master/docs/assets/panel_vendedor_ai.png" alt="vendedor-ai demo" width="100%"/>
</td>
</tr>
</table>

<br>

## Production Experience

<table>
<tr>
<td width="50%" valign="top">

### WhatsApp Sales Agent — Telecom Enterprise
Conversational AI handling live sales for a major telecom operator. Intent detection, catalog recommendation, CRM integration, payment processing. Deployed to real customers.

`LangGraph` `FastAPI` `RAG` `Qdrant` `WhatsApp API` `Redis`

<img src="https://img.shields.io/badge/Production-Live-00C853?style=flat-square" alt="Live"/>

</td>
<td width="50%" valign="top">

### Clinical Audit Automation — Hospital
AI pipeline that automated manual medical audits: OCR extraction, NLP classification, structured reporting. Replaced a multi-person manual process.

`Python` `NLP` `TensorFlow` `OCR` `FastAPI`

<img src="https://img.shields.io/badge/Production-Deployed-00C853?style=flat-square" alt="Deployed"/>

</td>
</tr>
</table>

<br>

## Open Source Projects

<table>
<tr>
<td width="50%" valign="top">

### [Scientific RAG System](https://github.com/DavidAguilarParedes/mia-uc-chile-proyecto-aplicado-1)
End-to-end retrieval-augmented generation for scientific literature. Document ingestion, embeddings, vector search, reranking, answer synthesis with evaluation framework.

`LangChain` `FAISS` `OpenAI` `Python`

</td>
<td width="50%" valign="top">

### [Industrial Quality Control](https://github.com/DavidAguilarParedes/Lab-IA-1MTR56-Automatizacion-Industrial-Inteligente)
Real-time defect detection on production lines. CNN image classification + custom HMI + PLC Beckhoff integration. Running on actual factory equipment.

`TensorFlow` `OpenCV` `pyads` `PLC Beckhoff`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Ultimate Tic-Tac-Toe RL](https://github.com/DavidAguilarParedes/ultimate-ttt-rl)
Reinforcement learning agent for the extended tic-tac-toe variant. Self-play training with policy optimization.

`Python` `Reinforcement Learning`

</td>
<td width="50%" valign="top">

### [GameQuizAI](https://github.com/DavidAguilarParedes/GameQuizAI)
Educational app that generates personalized quizzes from uploaded documents using LLMs. Interactive learning with AI-generated questions and feedback.

`Python` `OpenAI API` `NLP`

</td>
</tr>
</table>

<br>

## Technical Skills

<p align="center">
<img src="https://skillicons.dev/icons?i=python,tensorflow,pytorch,fastapi,docker,redis,postgres,aws,linux,git&theme=dark" alt="Tech Stack" />
</p>

| Area | Technologies |
|------|-------------|
| **LLMs & Agents** | Claude API, OpenAI API, LangChain, LangGraph, tool use, agentic loops, RAG, HITL patterns |
| **ML/DL** | TensorFlow, PyTorch, scikit-learn, Hugging Face, FAISS, Qdrant, computer vision |
| **Backend** | FastAPI, Redis, PostgreSQL, Docker, REST APIs, WebSockets, async Python |
| **Industrial** | PLC Beckhoff (TwinCAT), pyads, OPC-UA, OpenCV, SCADA, real-time HMI |

<br>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:161b22,100:58a6ff&height=80&section=footer" />
