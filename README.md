<div align="center">

# Hey there, I'm Mihul Bairagi 👋
### **AI Backend Engineer · Systems Builder · Problem Solver**

<p align="center">
  <a href="https://linkedin.com/in/mihulbairagi"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:mihulbairagi01@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://leetcode.com/u/mihulbairagi"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
  <a href="https://github.com/mihulbairagi"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

```python
class Engineer:
    def __init__(self):
        self.name = "Mihul Bairagi"
        self.role = "AI Backend Engineer"
        self.focus = ["Multi-Agent Systems", "Deterministic AI Backends", "High-Throughput RAG", "System Design"]
        self.philosophy = "Explainable > Clever. Grounding > Hallucination."
        self.status = "Building resilient backend infrastructure for autonomous systems."
```

</div>

---

### 💡 Core Engineering Philosophy

> *"The LLM's job is to route the question and phrase the answer — never to compute the facts."*

* **Deterministic vs. Generative Separation:** LLMs should not do math, rate-limiting, or business-critical calculations. I isolate LLMs behind strict state graphs, while arithmetic, caching, and evaluation run in pure, predictable Python services.
* **Grounding First in RAG:** A refusal with `grounded: false` (HTTP 200) is a successful outcome, not an error. If context falls below the cosine floor, the LLM is never called—saving latency, cost, and hallucination.
* **Zero-Vibe Testing:** Unit test logic with mocked network transports (`respx`, `pytest`) and behavioral eval suites rather than guessing through manual prompts.

---

### 🛠️ Tech Stack & Systems Arsenal

<div align="center">

| Domain | Technologies |
| :--- | :--- |
| **AI & Agent Orchestration** | `LangGraph`, `LangChain`, `Claude / Anthropic API`, `OpenAI / Gemini`, `RAG Architectures`, `Agentic Routing` |
| **Vector Search & Embeddings** | `ChromaDB`, `Sentence-Transformers (all-MiniLM-L6-v2)`, `Cosine-Similarity Filtering`, `SHA-256 Chunk Caching` |
| **Backend & Microservices** | `Python`, `FastAPI`, `Node.js`, `Express.js`, `REST APIs`, `WebSockets / Socket.io`, `Pydantic v2` |
| **Databases & Caching** | `SQLite (TTL Cache)`, `MongoDB`, `PostgreSQL`, `Redis` |
| **Infrastructure & DevOps** | `Docker`, `Docker Compose`, `GitHub Actions (CI/CD)`, `Linux / Bash` |
| **Core Foundations & DSA** | `Java`, `Data Structures & Algorithms (1200+ LeetCode solves)`, `Distributed System Design` |

</div>

---

### 🚀 Flagship Systems & Architectures

#### 1. [Aegis AI Gateway](https://github.com/mihulbairagi/aegis-ai-gateway) — High-Throughput Reverse Proxy & Semantic Cache
> **FastAPI · FastEmbed (ONNX) · Circuit Breaker (Hystrix) · Sliding Token Bucket · 350+ RPS**
* **Two-Tier Caching:** $O(1)$ LRU exact match (<0.05ms) + FastEmbed dense semantic cache (`all-MiniLM-L6-v2`, <10ms on CPU) achieving >85% cosine similarity on paraphrased queries.
* **Production Resilience:** 3-state Circuit Breaker (`CLOSED`/`OPEN`/`HALF_OPEN`) with automated failover and RFC 6585 sliding token-bucket rate limiter.
* **Dual-Tier Observability:** Distinguishes in-memory cache hits ($p_{50} < 1\text{ms}$) from live upstream WAN round-trips with real-time financial USD token savings telemetry.

#### 2. [Aegis-Copilot](https://github.com/mihulbairagi/aegis-enterprise-copilot) — Enterprise Operations Platform with RLS & Circuit Breakers
> **FastAPI · DuckDB OLAP · PyJWT HS256 · Chained SQLite Ledger · 19/19 Tests Passing**
* **RLS Pre-Filtering:** Row-level security clearance tiers (`INTERN`, `ANALYST`, `EXECUTIVE`) enforced at database query planner layer—unauthorized tokens NEVER enter LLM context.
* **Data Quality Circuit Breaker:** Automated 3-state ingestion gate isolating dirty batches (>15% null rate or domain anomalies) into an encrypted Dead-Letter Queue (DLQ).
* **Cryptographic Tamper-Proof Audit:** Immutable operational ledger linked with SHA-256 Merkle-style hash chaining and distributed idempotency keys.

#### 3. [CP Tutor Agent](https://github.com/mihulbairagi/cp_tutor_agent) — Multi-Agent Competitive Programming Coach
> **FastAPI · LangGraph · ChromaDB · SQLite TTL Cache · Pytest Suite (200+ tests)**
* **Architecture:** Multi-agent state graph that parses live Codeforces and LeetCode histories, normalizes cross-platform tag taxonomies, and diagnoses user weaknesses.
* **Deterministic Weakness Arithmetic:** Weakness scoring decomposes into 4 mathematical signals (`coverage`, `staleness`, `difficulty`, `struggle`) with sample-size confidence damping.
* **Zero-Waste Ingestion:** Dual-TTL caching (1h user history, 24h problemset catalog) with SHA-256 request hashing, exponential retry backoff, and local zero-cost embedding search.
* **Testability:** 207 unit tests with zero network calls + 15 end-to-end behavioral eval gates.

#### 4. [CareerGraph](https://github.com/mihulbairagi/CareerGraph) — Enterprise Multi-Agent Grounded RAG
> **FastAPI · LangGraph · ChromaDB · Claude Sonnet · Pydantic v2**
* **Strict Grounding Floors:** Discards chunks below cosine similarity floor (`0.25`). Skips LLM calls entirely when ungrounded, returning verified citations.
* **Multi-Agent Routing:** Classifies recruiter questions into specialized nodes (`Resume QA` vs `JD Matcher` for skill gap and ATS analysis) with deterministic fallback.
* **Production Lifespan Engine:** Singleton startup composition root prevents reloading 90MB embeddings on requests.

#### 5. [ClashCode](https://github.com/mihulbairagi/ClashCode) — Distributed Real-Time Online Judge
> **Node.js · Express · MongoDB · React · Monaco Editor · Socket.io · Wandbox API**
* Full-stack code execution engine supporting multiple languages with isolated remote compilation.
* Asynchronous judging queue with live bi-directional Socket.io room streaming (`Queued -> Judging -> Verdict`).

---

### 📊 GitHub Activity & Metrics

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mihulbairagi&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mihulbairagi&layout=compact&theme=tokyonight&hide_border=true" width="45%" alt="Top Languages" />
</div>

---

### 🤝 Let's Connect!

I'm always open to discussing **distributed AI backends, agentic systems, low-latency RAG, and backend scalability**.

- 💼 **LinkedIn:** [linkedin.com/in/mihulbairagi](https://linkedin.com/in/mihulbairagi)
- 📧 **Email:** [mihulbairagi01@gmail.com](mailto:mihulbairagi01@gmail.com)
- 💻 **LeetCode:** [leetcode.com/u/mihulbairagi](https://leetcode.com/u/mihulbairagi)

<div align="center">
  <sub>Built with clean architectures and zero vibe-checks.</sub>
</div>
