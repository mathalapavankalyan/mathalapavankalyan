<p align="center">
  <img src="assets/banner.svg" alt="Pavankalyan Mathala: Backend, Full-Stack and AI Engineer" width="100%">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=DAA520&center=true&vCenter=true&width=480&height=44&lines=Idempotent+payment+APIs+in+Spring+Boot;LangGraph+agents+grounded+in+real+data;React+UIs+that+stream+live+progress;Dockerized+services+shipped+to+AWS+ECR">
    <img alt="Idempotent payment APIs, LangGraph agents, streaming React UIs, Dockerized services on AWS" src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=9A7209&center=true&vCenter=true&width=480&height=44&lines=Idempotent+payment+APIs+in+Spring+Boot;LangGraph+agents+grounded+in+real+data;React+UIs+that+stream+live+progress;Dockerized+services+shipped+to+AWS+ECR">
  </picture>
</p>

<p align="center">
  <a href="#projects"><code>📂 Projects</code></a> &nbsp;·&nbsp;
  <a href="#stack"><code>🧰 Stack</code></a> &nbsp;·&nbsp;
  <a href="#contact"><code>📬 Contact</code></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OPEN_TO_WORK-Backend_%7C_Full--Stack_%7C_AI_Engineer-DAA520?style=for-the-badge&labelColor=111111" alt="Open to work: Backend, Full-Stack, AI Engineer"/>
</p>

---

## 👋 About

I build backend systems where correctness matters: payments, retries, concurrency, and scaling across instances.
I work in Java/Spring Boot with React frontends, and I build LLM agent workflows (LangGraph, FastAPI) that stay grounded in deterministic business rules.

**Looking for:** entry-level Backend, Full-Stack, or AI Engineering roles.

<a id="projects"></a>

## 📂 Projects

### 💳 [Payment Gateway](https://github.com/mathalapavankalyan/payment-gateway)
**Problem:** A client retry or a concurrent request must never create a duplicate payment.
**What I built:** A payment backend where every request carries an `Idempotency-Key`, and a hash of the payload catches the same key being reused for a different request. A database unique constraint is the final guard against races, and payment creation runs inside one transaction. CI runs tests, builds the Docker image, and pushes it to Amazon ECR using GitHub OIDC (no long-lived AWS keys) and a least-privilege IAM role.

`Java 17` `Spring Boot` `MySQL` `JPA/Hibernate` `Docker` `GitHub Actions` `AWS ECR`

### 🤖 [Paytm Payment Resolution Assistant](https://github.com/mathalapavankalyan/paytm-resolve)
**Problem:** Payment support questions ("payment failed but money was deducted") need an investigation, not a generic chatbot reply.
**What I built:** A four-stage LangGraph pipeline (understand → investigate → resolve → respond) that turns a message into structured intent, looks up transaction, refund, and policy records, and applies deterministic resolution rules. Progress streams to a React UI over Server-Sent Events.

`React` `Vite` `FastAPI` `LangGraph` `Pydantic` `SSE`

### ⚖️ [Load Balancer](https://github.com/mathalapavankalyan/load-balancer)
**Problem:** Show how one service scales horizontally behind a single entry point.
**What I built:** Three Spring Boot instances behind Nginx (round-robin) sharing one MySQL 8 database, orchestrated with Docker Compose.

`Spring Boot` `Nginx` `MySQL` `Docker Compose`

<a id="stack"></a>

## 🧰 Stack

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=dark&perline=7">
    <img alt="Java, Spring Boot, React, JavaScript, Python, FastAPI, MySQL, MongoDB, Docker, Nginx, GitHub Actions, AWS, Git" src="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=light&perline=7">
  </picture>
</p>

**Backend:** `Java` `Spring Boot` `JPA` `FastAPI` · **Frontend:** `React` `JavaScript`
**AI:** `LangGraph` `LangChain` · **Data:** `MySQL` `MongoDB`
**DevOps:** `Docker` `Nginx` `GitHub Actions` `AWS ECR/IAM`

## 🔭 Currently

- 🔨 Building: [CURRENT_PROJECT]
- 📚 Learning: [e.g. Redis, Kafka, system design]

<a id="contact"></a>

## 📬 Contact

<a href="https://pavankalyan-portfolio-eight.vercel.app/"><code>🌐 Portfolio</code></a> &nbsp;·&nbsp;
<a href="https://www.linkedin.com/in/pavankalyan-mathala/"><code>💼 LinkedIn</code></a> &nbsp;·&nbsp;
<a href="mailto:mathalapavankalyan@gmail.com"><code>✉️ Email</code></a>

<details>
<summary><b>🏆 Achievements</b></summary>

- Two-time Inter-College CodeHack winner
- Top scorer, NPTEL Joy of Computing

</details>

---

<p align="center"><i>If my work fits what you're looking for, let's talk. Stars on the repos are always appreciated ⭐</i></p>
