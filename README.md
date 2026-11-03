<p align="center">
  <img src="assets/hero.svg" width="100%" alt="Rohan Chawla: SDET I at Cyware Labs. AI Engineering, SDET and Backend Services." />
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1400&color=A78BFA&center=true&vCenter=true&width=820&lines=Designing+API+automation+for+distributed+microservices;Evaluating+LLMs+with+RAGAS%2C+DeepEval+%26+LLM-as-judge;Stress-testing+multi-tenant+systems+on+Kubernetes;Building+agentic+AI+that+writes+its+own+negative+tests" alt="Designing API automation for distributed microservices. Evaluating LLMs. Stress-testing multi-tenant systems on Kubernetes. Building agentic AI." />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rohan-chawla-607145229/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:rohanchawla515@gmail.com"><img src="https://img.shields.io/badge/Email-rohanchawla515%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email rohanchawla515@gmail.com" /></a>
  <img src="https://komarev.com/ghpvc/?username=rohanchawla2003&style=for-the-badge&color=7c3aed&label=Profile+views" alt="profile views" />
</p>

---

## 👨‍💻 About

I'm an engineer at **Cyware Labs** working where **distributed systems, quality engineering and applied AI** meet. Day to day I design the frameworks that validate a microservices-based security platform. That means simulating failures across services, pushing multi-tenant workloads on Kubernetes, and building LLM-powered tooling that finds bugs humans miss.

I care about understanding systems deeply enough to know **exactly how they break**, and engineering them so they don't.

---

## 🧠 What I Work On

### 🤖 AI Engineering & LLM Evaluation

> *An LLM feature is only as good as your ability to measure it.*

- Built an **agentic AI negative-test generator** that automatically produces the invalid and edge-case inputs most likely to break a service
- Evaluate LLM and RAG pipelines with **RAGAS, DeepEval and promptfoo**, plus **LLM-as-judge** scoring and **guardrails**, with tracing in **LangSmith / Langfuse**
- Work across the RAG stack: **embeddings, hybrid search, re-ranking**, and vector stores (**Pinecone, Qdrant, Chroma, FAISS, pgvector**)
- Orchestrate agents with **LangGraph, LangChain, LlamaIndex, CrewAI** and **MCP**, on top of **OpenAI, Claude, Gemini and Bedrock**

<details>
<summary><b>📐 How I evaluate an LLM / RAG system</b></summary>
<br/>

1. **Golden dataset first:** curated questions with expected answers and source context, versioned alongside the code
2. **Score retrieval and generation separately:** context precision / recall for the retriever; faithfulness and answer relevancy for the generator
3. **LLM-as-judge with explicit rubrics**, calibrated against human-labelled samples so the judge itself is trustworthy
4. **Adversarial and safety cases:** prompt injection, jailbreaks, out-of-scope queries, with guardrails verified, not assumed
5. **Evals as regression tests:** run in CI on every prompt, model or retriever change, so quality can't silently drift
6. **Trace everything:** inspect failing runs step by step in LangSmith / Langfuse to fix root causes, not symptoms

</details>

### 🧪 Quality Engineering for Distributed Systems

> *A green test suite should mean something.*

| What I built | Impact |
|---|---|
| ⚙️ **API automation framework** for distributed microservices | **+75%** developer productivity |
| 🔗 **Centralized cross-service workflow framework** | **+40%** testing efficiency |
| 💥 **Failure & edge-case simulation** across services | **20+** critical cross-service defects caught |
| 🚀 **Dockerized Jenkins CI/CD** for UI + API suites | **−50%** execution time |
| 🧪 **Selenium + PyTest regression suites** | **−35%** manual QA effort · **500+** defects reported |
| 🔄 **Upgrade validation framework** & cross-product test repository | Safer releases across the product suite |

<details>
<summary><b>📐 How I test a distributed system</b></summary>
<br/>

1. **Contracts before flows:** validate each service's API schema, status codes and error semantics in isolation
2. **Then the workflows:** end-to-end cross-service scenarios that follow data as it moves through queues and services
3. **Break it on purpose:** service timeouts, partial failures, retries, out-of-order and duplicate events (is it *really* idempotent?)
4. **Concurrency and scale:** parallel writers, race conditions, and load against realistic multi-tenant data volumes
5. **Tenant isolation:** prove one tenant can never see, slow down or corrupt another's data
6. **Upgrades are features too:** validate data, config and API compatibility across version upgrades
7. **Observability is part of the test:** correlate failures with logs and Grafana metrics, so a bug report ships with its root cause

</details>

### ⚙️ Backend & Distributed Systems

> *Systems that stay up when the traffic doesn't stay down.*

- Deep, hands-on understanding of **microservices, async processing, event streaming (Kafka)** and the failure modes between them
- **Multi-tenancy, concurrency and scalability** testing on **Kubernetes** for production-grade workloads
- Build services and tooling in **Python (Django, FastAPI)** and **Java**, backed by **SQL / NoSQL** stores and **Redis**
- Ship through **Docker → Jenkins → Kubernetes on AWS**, with **Grafana** and log analysis to understand behaviour in production

---

## 🎲 Fun Facts

<p align="center">
  <img src="assets/fun-facts.svg" width="100%" alt="Animated fun facts about Rohan" />
</p>

<details>
<summary><b>Can't see the animation? Read them all here 👇</b></summary>
<br/>

- 🐛 I break software for a living: **500+ bugs** found, and the count keeps climbing.
- 🤖 I built an AI whose only job is to **break my other code**. It's very good at it.
- 🚀 I made our CI pipeline **2x faster**. Waiting on builds was never my thing.
- ⚖️ I evaluate LLMs at work, and sometimes I hire **another LLM as the judge**.
- 🧩 I solve Codeforces problems **for fun**. Yes, for fun. (1200+ rating, CodeChef 3★)

</details>

---

## 🛠️ Tech Stack

<table>
<tr><td><b>Languages</b></td><td><img src="https://skillicons.dev/icons?i=python,java,js,ts&theme=dark" alt="Python, Java, JavaScript, TypeScript" /></td></tr>
<tr><td><b>Testing</b></td><td><img src="https://skillicons.dev/icons?i=selenium,postman&theme=dark" alt="Selenium, Postman" /><br/><sub>PyTest · Playwright · SoapUI · API / UI / E2E / Load / Regression testing · TDD</sub></td></tr>
<tr><td><b>Backend & Infra</b></td><td><img src="https://skillicons.dev/icons?i=django,fastapi,kafka,docker,kubernetes,jenkins,aws,grafana,git,linux&theme=dark" alt="Django, FastAPI, Kafka, Docker, Kubernetes, Jenkins, AWS, Grafana, Git, Linux" /></td></tr>
<tr><td><b>Databases</b></td><td><img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis&theme=dark" alt="PostgreSQL, MySQL, MongoDB, Redis" /></td></tr>
<tr><td><b>AI / LLM</b></td><td>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white" alt="LangGraph" />
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" alt="LangChain" />
<img src="https://img.shields.io/badge/LlamaIndex-6E40C9?style=flat-square" alt="LlamaIndex" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
<img src="https://img.shields.io/badge/RAGAS%20%C2%B7%20DeepEval%20%C2%B7%20promptfoo-0A66C2?style=flat-square" alt="LLM evaluation tools" />
<img src="https://img.shields.io/badge/Vector%20DBs-Pinecone%20%C2%B7%20Qdrant%20%C2%B7%20pgvector-0f766e?style=flat-square" alt="Vector databases" />
<img src="https://img.shields.io/badge/MCP-000000?style=flat-square" alt="MCP" />
<img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code" />
<img src="https://img.shields.io/badge/Cursor-111111?style=flat-square" alt="Cursor" />
</td></tr>
</table>

---

## 🎓 Foundations

- **B.Tech, Computer Science & Engineering**, Maharaja Agrasen Institute of Technology (2025) · **CGPA 8.6**
- **Competitive programming:** Codeforces **1200+** · CodeChef **3★**
- Internal hackathon **special mention**

---

## 🚀 Projects

| Project | What it does | Tech |
|---|---|---|
| [✋ Gesture Control Presentation](https://github.com/rohanchawla2003/Gesture-control-presentation) | Control a PowerPoint deck with hand gestures, using ML-based hand tracking | Python · OpenCV |
| [🧪 ML Lab](https://github.com/rohanchawla2003/MLlab) | Machine learning experiments & lab work | Python · Jupyter |
| [🎮 2048 Game](https://github.com/rohanchawla2003/2048-game) | The classic 2048 sliding-tile puzzle, built from scratch | C++ |
| [🛒 Amazon Clone](https://github.com/rohanchawla2003/AmazonClone) | Front-end clone of the Amazon homepage | HTML · CSS |

<sub>Most of my production work at Cyware lives in private repositories.</sub>

---

<p align="center">
  <img src="https://streak-stats.demolab.com?user=rohanchawla2003&theme=tokyonight&hide_border=true&background=0A0F1F&ring=A78BFA&fire=F472B6&currStreakLabel=A78BFA" alt="GitHub streak" />
</p>

<p align="center">
  <b>💬 Always happy to talk distributed systems, testing strategy or LLM evaluation.</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/rohan-chawla-607145229/"><img src="https://img.shields.io/badge/Connect%20on-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" /></a>
  <a href="mailto:rohanchawla515@gmail.com"><img src="https://img.shields.io/badge/Say-Hello-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Send an email" /></a>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0f1f,50:3b1d7a,100:0e7490&height=110&section=footer" alt="footer" />
</p>
