<p align="center">
  <img src="assets/banner.svg" alt="Pavankalyan Mathala: Backend and AI Engineer" width="100%">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=DAA520&center=true&vCenter=true&width=480&height=44&lines=Charged+twice%3F+Not+on+my+watch.;15s+to+2s+with+one+Redis+cache;Bulk+reports%3A+8+hrs+to+2+hrs;The+LLM+talks.+The+rules+decide.">
    <img alt="Charged twice? Not on my watch. 15s to 2s with one Redis cache. Bulk reports: 8 hrs to 2 hrs. The LLM talks, the rules decide." src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=9A7209&center=true&vCenter=true&width=480&height=44&lines=Charged+twice%3F+Not+on+my+watch.;15s+to+2s+with+one+Redis+cache;Bulk+reports%3A+8+hrs+to+2+hrs;The+LLM+talks.+The+rules+decide.">
  </picture>
</p>

<p align="center">
  <a href="#impact"><img src="assets/icons/zap.svg" height="16" align="absmiddle" alt=""> <b>Impact</b></a> &nbsp;·&nbsp;
  <a href="#ai"><img src="assets/icons/cpu.svg" height="16" align="absmiddle" alt=""> <b>AI Work</b></a> &nbsp;·&nbsp;
  <a href="#projects"><img src="assets/icons/code.svg" height="16" align="absmiddle" alt=""> <b>Projects</b></a> &nbsp;·&nbsp;
  <a href="#stack"><img src="assets/icons/layers.svg" height="16" align="absmiddle" alt=""> <b>Stack</b></a> &nbsp;·&nbsp;
  <a href="#contact"><img src="assets/icons/mail.svg" height="16" align="absmiddle" alt=""> <b>Contact</b></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OPEN_TO_WORK-Backend_%7C_AI_Engineer-DAA520?style=for-the-badge&labelColor=111111" alt="Open to work: Backend and AI Engineer"/>
</p>

---

<h2><img src="assets/icons/user.svg" height="26" align="absmiddle" alt=""> About</h2>

Java backend engineer with 2+ years in healthcare and fintech, based in Bengaluru. I make slow things fast, silent failures loud, and AI agents boring in the best way: the LLM understands the question, and deterministic rules make the decision.

**Looking for:** Backend Engineer and AI Engineer roles, ideally where Spring Boot, AWS, and agentic AI meet. I will treat your production database with the respect of a very nervous person.

<a id="impact"></a>

<h2><img src="assets/icons/zap.svg" height="26" align="absmiddle" alt=""> Impact</h2>

*Numbers I'm allowed to brag about (all from my work at Endava).*

| Result | How |
|---|---|
| **15s → 2s** repeat plan evaluation (~87% faster) | Redis cache keyed on plan ID and configuration, so identical requests skip recalculation |
| **~8 hrs → ~2 hrs** for 10,000+ reports | Replaced one-at-a-time synchronous generation with batch processing, and extended reports from PDF-only to PDF + Excel with multi-attachment email delivery |
| **15 → 6 min** deploys, 88% JUnit coverage | Per-Lambda GitHub Actions pipelines (OIDC, no stored AWS keys) that redeploy only the Lambdas that changed |
| **Silent failures eliminated** in an SQS pipeline | Plans that exhausted their retries used to vanish with no status. Dead-letter-queue handling now marks them FAILED, so every request ends visibly |
| **50,000-plan catalog**, 5-6k daily users | Built client-specific plan configuration features on a healthcare plan platform |

<h3><img src="assets/icons/briefcase.svg" height="22" align="absmiddle" alt=""> Experience at Endava</h3>

**Software Developer** · Sep 2025 – Present · *Benefit Calculation Rules Platform*
Replaced an Excel-based benefit-rules tool (the spreadsheet did not put up a fight) with a serverless REST rules engine built with a team of 7, evaluating 8-10 scenarios per plan. I built its API Gateway + Lambda layer, and also shipped 5+ GenAI and agentic POCs (below).

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,aws,dynamodb,redis,githubactions&theme=dark">
  <img alt="Java, Spring Boot, AWS, DynamoDB, Redis, GitHub Actions" src="https://skillicons.dev/icons?i=java,spring,aws,dynamodb,redis,githubactions&theme=light">
</picture>

**Associate Software Engineer** · Aug 2024 – Sep 2025 · *Healthcare Plan Management Platform*
Built the Kafka consumer in the rule service that applies business rules to every plan event and validates it against configured constraints.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,kafka,redis&theme=dark">
  <img alt="Java, Spring Boot, Kafka, Redis" src="https://skillicons.dev/icons?i=java,spring,kafka,redis&theme=light">
</picture>

<a id="ai"></a>

<h2><img src="assets/icons/cpu.svg" height="26" align="absmiddle" alt=""> GenAI &amp; Agentic AI</h2>

### <img src="assets/icons/cpu.svg" height="22" align="absmiddle" alt=""> Plan Recommendation Assistant (RAG + Knowledge Graph + MCP)
*"The LLM gets a tool menu, not the keys to the database."*

- RAG pipeline over ~100 policy and rule documents (OpenAI Embeddings, Chroma, top-k retrieval), with retrieval relevance and recommendations validated against plan data.
- Custom weighted knowledge graph in MongoDB: ranking signals (age, monthly premium, plan type) score each policy and steer the agent to the right documents.
- FastAPI tools (DB fetch, RAG, summarize) exposed to the agent through MCP, so the LLM only sees tool interfaces and never the underlying data sources.
- Demoed to leadership and a client.

### <img src="assets/icons/users.svg" height="22" align="absmiddle" alt=""> AI-Native Workforce Management System
**Winner, APAC, OpenAI × Endava Codex Hackathon (55+ teams).** I designed the multi-agent workflow that recommends available candidates matched to an opportunity's details. Built with Codex, React, Python, and FastAPI.

### <img src="assets/icons/shield.svg" height="22" align="absmiddle" alt=""> [Payment-Resolution Assistant](https://github.com/mathalapavankalyan/paytm-resolve)
**Top 20 of ~4,774 in the Paytm Build AI Hackathon** (team of 2). A LangGraph agent handles intent understanding, tool selection, and session memory, while deterministic search handles lookups, so money-critical answers are never left to the LLM. Progress streams to a React UI over Server-Sent Events, so users watch the investigation instead of a spinner.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=python,fastapi,react&theme=dark">
  <img alt="Python, FastAPI, React" src="https://skillicons.dev/icons?i=python,fastapi,react&theme=light">
</picture>
<img src="https://img.shields.io/badge/LangGraph-111111?style=for-the-badge&logo=langchain&logoColor=DAA520" alt="LangGraph" align="top">

<a id="projects"></a>

<h2><img src="assets/icons/code.svg" height="26" align="absmiddle" alt=""> Projects</h2>

### <img src="assets/icons/shield.svg" height="22" align="absmiddle" alt=""> [Idempotent Payment Gateway](https://github.com/mathalapavankalyan/payment-gateway)
*"Charged twice? Not on my watch."*

**The problem:** Users double-tap Pay, networks drop, clients retry, and the customer should still be charged exactly once.
**The fix:** Every request carries an `Idempotency-Key`, plus a hash of the payload, so reusing a key with a different amount gets rejected (a ₹500 key can't sneak in a ₹5000 payment). When two requests race, a database unique constraint is the final referee. Order and payment state machines run inside `@Transactional` boundaries, and tests cover duplicates, key reuse, concurrency, and rollback. CI builds the Docker image and pushes it to Amazon ECR through GitHub OIDC.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,mysql,docker,githubactions,aws&theme=dark">
  <img alt="Java, Spring Boot, MySQL, Docker, GitHub Actions, AWS" src="https://skillicons.dev/icons?i=java,spring,mysql,docker,githubactions,aws&theme=light">
</picture>

<details>
<summary><b>More: Load Balancer</b></summary>

[**Load Balancer**](https://github.com/mathalapavankalyan/load-balancer): *3 servers, 1 Nginx, 0 drama.* Three Spring Boot instances behind Nginx round-robin, sharing one MySQL 8 database, started with a single `docker compose up`.

</details>

<a id="stack"></a>

<h2><img src="assets/icons/layers.svg" height="26" align="absmiddle" alt=""> Stack</h2>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,python,fastapi,mysql,mongodb,redis,kafka,aws,docker,githubactions,git&theme=dark&perline=6">
    <img alt="Java, Spring Boot, Python, FastAPI, MySQL, MongoDB, Redis, Kafka, AWS, Docker, GitHub Actions, Git" src="https://skillicons.dev/icons?i=java,spring,python,fastapi,mysql,mongodb,redis,kafka,aws,docker,githubactions,git&theme=light&perline=6">
  </picture>
</p>

**Languages:** Java 17, Python, SQL
**Backend:** Spring Boot, REST APIs, Hibernate/JPA, FastAPI, JUnit, Mockito
**GenAI & Agentic AI:** LangChain, LangGraph, RAG (OpenAI Embeddings, Chroma), knowledge graphs, MCP, LLM tool calling
**Data & Messaging:** MS SQL Server, MySQL, MongoDB, DynamoDB, Redis, Kafka, SQS
**Cloud & DevOps:** AWS (Lambda, API Gateway, SQS, DynamoDB, S3, ECR), Docker, Git, GitHub Actions CI/CD (OIDC)

<a id="contact"></a>

<h2><img src="assets/icons/mail.svg" height="26" align="absmiddle" alt=""> Contact</h2>

<a href="https://pavankalyan-portfolio-eight.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-111111?style=for-the-badge&logo=vercel&logoColor=DAA520" alt="Portfolio"></a>
<a href="https://www.linkedin.com/in/pavankalyan-mathala/"><img src="https://img.shields.io/badge/LinkedIn-111111?style=for-the-badge&logo=linkedin&logoColor=DAA520" alt="LinkedIn"></a>
<a href="mailto:mathalapavankalyan@gmail.com"><img src="https://img.shields.io/badge/Email-111111?style=for-the-badge&logo=gmail&logoColor=DAA520" alt="Email"></a>
<a href="https://leetcode.com/u/pavanmathala"><img src="https://img.shields.io/badge/LeetCode_500%2B-111111?style=for-the-badge&logo=leetcode&logoColor=DAA520" alt="LeetCode, 500+ problems"></a>

Fastest reply: email. Slowest: carrier pigeon.

<details>
<summary><img src="assets/icons/award.svg" height="18" align="absmiddle" alt=""> <b>Achievements &amp; education</b></summary>

- Winner, APAC: OpenAI × Endava Codex Hackathon (55+ teams)
- Top 20 of ~4,774: Paytm Build AI Hackathon
- Two-time Inter-College CodeHack winner (the second one wasn't a fluke)
- Top scorer, NPTEL Joy of Computing
- B.Tech, Computer Science, NRI Institute of Technology (CGPA 8.6/10), 2020 – 2024

</details>

---

<p align="center"><i>Star a repo and I'll say thanks exactly once, no matter how many times you click. It's idempotent.</i></p>
