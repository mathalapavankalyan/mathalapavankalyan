<h1 align="center" style="color:#DAA520;">Pavankalyan Mathala</h1>
<h3 align="center" style="color:#DAA520;">Java Backend Engineer (Spring Boot | AWS | Kafka) • Agentic AI & RAG Engineer</h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=22&color=DAA520&center=true&vCenter=true&width=900&lines=Java+%7C+Spring+Boot+%7C+AWS+%7C+Redis+%7C+Kafka;Charged+twice%3F+Not+on+my+watch.;Agentic+AI+%7C+LangGraph+%7C+RAG+%7C+MCP;The+LLM+talks.+The+rules+decide." />
</p>

---

## <span style="color:#DAA520;">About Me</span>

I am a **Java Backend Engineer** with 2+ years across healthcare and payments, building systems that stay correct under retries, concurrency, and failure:

- **Java, Spring Boot** for APIs and rules engines where correctness matters more than cleverness  
- **Redis, Kafka, SQS** for fast, event-driven pipelines: a Redis cache took repeat plan evaluation from 15s to 2s, and batch processing took 10,000+ report generation from ~8 hrs to ~2 hrs  
- **AWS (Lambda, API Gateway, ECR), Docker, GitHub Actions** for serverless services and CI/CD with no stored cloud keys  

In addition to backend engineering, I also build **Gen-AI applications**, including:

- Agentic AI systems that investigate before they answer  
- LangGraph + LangChain multi-agent workflows (Winner, APAC: OpenAI × Endava Codex Hackathon)  
- RAG pipelines over ~100 policy documents using OpenAI Embeddings and Chroma, steered by a weighted knowledge graph in MongoDB  
- MCP tool servers on FastAPI, so the LLM sees tool interfaces and never the underlying data sources  

I combine **strong backend foundations** with **modern AI tooling**. My rule for AI in production: **the LLM understands the question, and deterministic rules make the decision.** I would rather ship systems that behave predictably under retries, failures, and real traffic than ones that only look good in a demo.

Open to roles in **Backend Engineering and AI Engineering**.

---

## <span style="color:#DAA520;">Connect with Me</span>

<p align="center">
  <a href="mailto:mathalapavankalyan@gmail.com"><img src="https://img.shields.io/badge/Email-000000?style=for-the-badge&logo=gmail&logoColor=DAA520"/></a>
  <a href="https://www.linkedin.com/in/pavankalyan-mathala/"><img src="https://img.shields.io/badge/LinkedIn-000000?style=for-the-badge&logo=linkedin&logoColor=DAA520"/></a>
  <a href="https://github.com/mathalapavankalyan"><img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=DAA520"/></a>
  <a href="https://pavankalyan-portfolio-eight.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=DAA520"/></a>
  <a href="https://leetcode.com/u/pavanmathala"><img src="https://img.shields.io/badge/LeetCode_500%2B-000000?style=for-the-badge&logo=leetcode&logoColor=DAA520"/></a>
</p>

---

# <span style="color:#DAA520;">Tech Stack</span>

### **Core Backend**
- Java 17 • Spring Boot  
- REST APIs • Hibernate/JPA  
- JUnit • Mockito  
- Python • FastAPI  

### **AI & Gen-AI Development**
- LangGraph  
- LangChain  
- RAG (OpenAI Embeddings, Chroma)  
- Knowledge Graphs • MCP  
- LLM Tool-Calling • Multi-Agent Workflows  

### **Database & DevOps**
- SQL • MySQL • MongoDB • DynamoDB • Redis  
- Kafka • Amazon SQS  
- AWS (Lambda, API Gateway, S3, ECR)  
- Docker • GitHub Actions (OIDC)  

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,python,fastapi,mysql,mongodb,redis,kafka,aws,docker,githubactions,git&theme=dark" />
</p>

---

# <span style="color:#DAA520;">Featured Projects</span>

### <span style="color:#DAA520;">[Idempotent Payment Gateway](https://github.com/mathalapavankalyan/payment-gateway) — Charged Twice? Not on My Watch</span>  
Tech: Java 17 • Spring Boot • MySQL • Docker • GitHub Actions • AWS ECR
- Every request carries an `Idempotency-Key` plus a hash of the payload, so retries return the original result and a reused key with a different amount is rejected  
- A database unique constraint closes the check-then-insert race, and order/payment state machines run inside `@Transactional` boundaries, with tests for duplicates, key reuse, concurrency, and rollback  
- CI builds the Docker image and pushes it to Amazon ECR through GitHub OIDC, with no long-lived AWS keys  

---

### <span style="color:#DAA520;">[Payment-Resolution Assistant](https://github.com/mathalapavankalyan/paytm-resolve) — An Agent That Investigates Before It Talks</span>  
Tech: Python • FastAPI • LangGraph • React
- Four-stage LangGraph pipeline (understand → investigate → resolve → respond) with session memory, where the LLM reads the message and deterministic search and rules decide the outcome  
- Investigation progress streams to a React UI over Server-Sent Events, so users watch each step instead of a spinner  
- Top 20 of ~4,774 in the Paytm Build for India AI Hackathon (team of 2)  

---

### <span style="color:#DAA520;">[Load Balancer](https://github.com/mathalapavankalyan/load-balancer) — 3 Servers, 1 Nginx, 0 Drama</span>  
Tech: Java • Spring Boot • Nginx • MySQL • Docker Compose
- Three Spring Boot instances behind Nginx round-robin routing  
- One shared MySQL 8 database, with the whole stack started by a single `docker compose up`  
- A hands-on demo of horizontal scaling versus load balancing  

---

# <span style="color:#DAA520;">Achievements</span>

- Winner, APAC: OpenAI × Endava Codex Hackathon (55+ teams)  
- Top 20 of ~4,774: Paytm Build for India AI Hackathon  
- Two-time Inter-College CodeHack Winner  
- Top Scorer – NPTEL Joy of Computing  
- 500+ problems solved on LeetCode  

---

# <span style="color:#DAA520;">GitHub Analytics</span>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=mathalapavankalyan&show_icons=true&theme=tokyonight" height="160px" />
  <img src="https://streak-stats.demolab.com/?user=mathalapavankalyan&theme=tokyonight" height="160px" />
</p>

---

# <span style="color:#DAA520;">Languages</span>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=mathalapavankalyan&layout=compact&theme=tokyonight"/>
</p>

---

<p align="center" style="color:#DAA520;">
  If this is the kind of work you're looking for, explore the repos and star them. I'll say thanks exactly once, no matter how many times you click.
</p>
