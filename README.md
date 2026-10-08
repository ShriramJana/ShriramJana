# Shriram Janardhan

**Software Engineer — AI/ML · Agentic Systems · Full Stack**

CS @ UT Dallas ('27, Finance minor). I build autonomous agent systems and the infrastructure that keeps them trustworthy: orchestration, evaluation, and retrieval pipelines that hold up outside a demo.

Currently at Nebula Labs. Open to SWE, backend, and AI engineering roles.

[shriramjana.com](https://shriramjana.com) · [LinkedIn](https://linkedin.com/in/shriramjana) · [shriram.j.iyengar@gmail.com](mailto:shriram.j.iyengar@gmail.com)

---

### Selected work

**Aegis** &nbsp;·&nbsp; 🔨 *currently building*<br>
MCP-native security middleware for agent deployments in air-gapped environments. Sits between the model and its tools to enforce policy on what an agent is allowed to call, and writes an audit trail of every invocation.<br>
`Python`

**[Crossbar](https://github.com/ShriramJana/crossbar)**<br>
Multi-provider LLM gateway in Go. Authenticates callers, enforces per-team rate limits and spend budgets in Redis, and fails over across providers, with the circuit breaker, token bucket, and fallback chain written from scratch rather than imported. Load-tested on a single host against a mock provider: 7,174 req/s at 7.4 ms p99 gateway overhead, exactly 100 of 1,000 simultaneous requests admitted against a 100 rpm limit, and zero client-visible 5xx across 461,858 requests while the primary provider was down.<br>
`Go` `Redis` `Prometheus` `Grafana`

**[Trajectory Prediction](https://github.com/ShriramJana/av2-trajectory-prediction)** &nbsp;·&nbsp; *v1.0 released*<br>
Predicts where a vehicle will be over the next 6 seconds from 5 seconds of history on Argoverse 2. Built as a ladder from constant velocity to a VectorNet-style polyline transformer, with every stage scored on the same 5,000 frozen validation scenarios: endpoint error (minFDE) falls from 11.7 m to 1.9 m. Predicting six futures instead of one was the largest single gain, because an agent at an intersection may turn either way and the mean of those is a curb. 0.92M parameters, trained in 1.5 hours on one RTX 4060.<br>
`Python` `PyTorch`

**[Sentinel](https://github.com/ShriramJana/sentinel)** &nbsp;·&nbsp; *v1 complete*<br>
AI-assisted retrieval and triage for telecom incidents. Combines BM25, dense retrieval, RRF fusion, and cross-encoder reranking to search historical incidents from plain-language outage reports. Evaluated across 2,730 synthetic alarms and 100 frozen operator-style queries, demonstrating that incident relevance and causal-alarm identification require separate objectives.<br>
`Python` `Cohere` `Qdrant` `Docker`

**[evalgate](https://github.com/ShriramJana/evalgate)**<br>
A regression gate for LLM systems. Scores answer quality against a committed baseline and fails CI when a change degrades it — so prompt and model changes get the same scrutiny as code.<br>
`Python`

**[Autonomous Research Assistant (ARA)](https://github.com/ShriramJana/autonomous-research-assistant)** &nbsp;·&nbsp; [live demo →](https://autonomous-research-assistant-tawny.vercel.app)<br>
Turns a research question into a cited, multi-source report. A Planner decomposes the question into 3–7 sub-queries, parallel Researcher agents search the live web, and a Synthesizer merges the findings — all streamed to the browser over SSE with per-agent status and a running cost meter. Citations are stable UUIDs, so sources never get mis-numbered when deduplicated. A failed researcher degrades gracefully: the report still completes and notes the gap. Bring-your-own-key, with credentials encrypted per-user via Fernet.<br>
`Python` `FastAPI` `LangGraph` `Next.js` `Supabase`

**Autonomous AI Prediction Market Trading Bot**<br>
Monitors 4,100+ live Polymarket markets, ingesting 120+ news articles per polling cycle to find contracts mispriced against breaking news. Ten LLM analyst personas produce a crowd-consensus probability; Kelly Criterion sizing caps risk at 5% per trade. A circuit breaker halts trading on three consecutive losses or 10% daily drawdown. 130 unit tests across a 5-layer pipeline.<br>
*Private repository — architecture walkthrough available on request.*<br>
`Python` `FastAPI` `React`

**[portfolio-rag-chatbot](https://github.com/ShriramJana/portfolio-rag-chatbot)**<br>
Retrieval-augmented chatbot answering questions about my background, running in production on shriramjana.com.<br>
`TypeScript`

**[Notebook](https://github.com/UTDNebula/utd-notebook)** — Nebula Labs &nbsp;·&nbsp; [dev.notebook.utdnebula.com →](https://dev.notebook.utdnebula.com)<br>
Student-facing AI-powered note platform at UT Dallas. Next.js and PostgreSQL backend with multi-tenant auth and role-based access control.<br>
`TypeScript`

**[UTD Trends](https://github.com/UTDNebula/utd-trends)** — Nebula Labs &nbsp;·&nbsp; [trends.utdnebula.com →](https://trends.utdnebula.com)<br>
Course and professor data visualization serving 20,000+ UT Dallas students — aggregates grade distributions and Rate My Professors scores so students can compare sections before registering. Contributed frontend redesigns that lifted engagement 5x, and backend optimizations that cut API latency 30%.<br>
`TypeScript` `Next.js`

---

`Python` `TypeScript` `Go` `Java` `C++` `SQL` · `React` `Next.js` `Node.js` `FastAPI` · `LangGraph` `PyTorch` `scikit-learn` · `PostgreSQL` `Redis` `Docker` `AWS` `GCP`
