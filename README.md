# Shriram Janardhan

**Software Engineer — AI/ML · Agentic Systems · Full Stack**

CS @ UT Dallas ('27, Finance minor). I build autonomous agent systems and the infrastructure that keeps them trustworthy — orchestration, evaluation, and retrieval pipelines that hold up outside a demo.

Currently at Nebula Labs. Open to SWE, backend, and AI engineering roles.

[shriramjana.com](https://shriramjana.com) · [LinkedIn](https://linkedin.com/in/shriramjana) · [shriram.j.iyengar@gmail.com](mailto:shriram.j.iyengar@gmail.com)

---

### Selected work

**Aegis** &nbsp;·&nbsp; 🔨 *currently building*  
MCP-native security middleware for agent deployments in air-gapped environments. Sits between the model and its tools to enforce policy on what an agent is allowed to call, and writes an audit trail of every invocation.  
`Python`

**Sentinel** · 🔨 *currently building*

Retrieval triage for telecom incidents. Describe an outage in plain language, get ranked root causes grounded in similar historical alarm clusters and the exact vendor spec page.
Rerank v4 scores alarm records as structured JSON, not flattened prose. Hand labeled eval set, graded relevance, and every config run 3× with variance reported.
`Python` `Cohere` `Qdrant` `FastAPI`

**Trajectory Prediction** · 🔨 *currently building*

Predicts where an agent goes next from a few seconds of observed positions. Trained on Argoverse, scored with minADE/minFDE. Emits K candidate futures rather than one averaged
path, because an agent at an intersection may turn either way and the mean of those is a curb.
`Python` `PyTorch`

**[evalgate](https://github.com/ShriramJana/evalgate)**  
A regression gate for LLM systems. Scores answer quality against a committed baseline and fails CI when a change degrades it — so prompt and model changes get the same scrutiny as code.  
`Python`

**[Autonomous Research Assistant (ARA)](https://github.com/ShriramJana/autonomous-research-assistant)** &nbsp;·&nbsp; [live demo →](https://autonomous-research-assistant-tawny.vercel.app)  
Turns a research question into a cited, multi-source report. A Planner decomposes the question into 3–7 sub-queries, parallel Researcher agents search the live web, and a Synthesizer merges the findings — all streamed to the browser over SSE with per-agent status and a running cost meter. Citations are stable UUIDs, so sources never get mis-numbered when deduplicated. A failed researcher degrades gracefully: the report still completes and notes the gap. Bring-your-own-key, with credentials encrypted per-user via Fernet.  
`Python` `FastAPI` `LangGraph` `Next.js` `Supabase`

**Autonomous AI Prediction Market Trading Bot**  
Monitors 4,100+ live Polymarket markets, ingesting 120+ news articles per polling cycle to find contracts mispriced against breaking news. Ten LLM analyst personas produce a crowd-consensus probability; Kelly Criterion sizing caps risk at 5% per trade. A circuit breaker halts trading on three consecutive losses or 10% daily drawdown. 130 unit tests across a 5-layer pipeline.  
*Private repository — architecture walkthrough available on request.*  
`Python` `FastAPI` `React`

**[portfolio-rag-chatbot](https://github.com/ShriramJana/portfolio-rag-chatbot)**  
Retrieval-augmented chatbot answering questions about my background, running in production on shriramjana.com.  
`TypeScript`

**[Notebook](https://github.com/UTDNebula/utd-notebook)** — Nebula Labs &nbsp;·&nbsp; [https://dev.notebook.utdnebula.com →](https://dev.notebook.utdnebula.com)   
Student-facing AI-powered note platform at UT Dallas. Next.js and PostgreSQL backend with multi-tenant auth and role-based access control.  
`TypeScript`

**[UTD Trends](https://github.com/UTDNebula/utd-trends)** — Nebula Labs &nbsp;·&nbsp; [trends.utdnebula.com →](https://trends.utdnebula.com)  
Course and professor data visualization serving 20,000+ UT Dallas students — aggregates grade distributions and Rate My Professors scores so students can compare sections before registering. Contributed frontend redesigns that lifted engagement 5x, and backend optimizations that cut API latency 30%.  
`TypeScript` `Next.js`


---

`Python` `TypeScript` `Java` `C++` `SQL` · `React` `Next.js` `Node.js` `FastAPI` · `LangGraph` `PyTorch` `scikit-learn` · `PostgreSQL` `Docker` `AWS` `GCP`
