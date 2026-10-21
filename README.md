<h1 align="center">Pavankalyan Mathala</h1>
<h3 align="center">Backend & Full-Stack Engineer · Java, Spring Boot · AI Agents with LangGraph</h3>

<p align="center">
  <a href="https://pavankalyan-portfolio-eight.vercel.app/">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/pavankalyan-mathala/">LinkedIn</a> ·
  <a href="mailto:mathalapavankalyan@gmail.com">Email</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OPEN_TO_WORK-Backend_%7C_Full--Stack_%7C_AI_Engineer-DAA520?style=for-the-badge" alt="Open to work"/>
</p>

---

## 👋 About

I build backend systems where correctness matters: payments, retries, concurrency, and scaling across instances.
I work in Java/Spring Boot with React frontends, and I build LLM agent workflows (LangGraph, FastAPI) that stay grounded in deterministic business rules.
**Looking for:** entry-level Backend, Full-Stack, or AI Engineering roles. Email or LinkedIn is the fastest way to reach me.

## 🚀 Featured Projects

### 💳 [Payment Gateway](https://github.com/mathalapavankalyan/payment-gateway)
**Problem:** A client retry or a concurrent request must never create a duplicate payment.
**What I built:** A payment backend where every request carries an `Idempotency-Key`, and a hash of the payload catches the same key being reused for a different request. A database unique constraint is the final guard against races, and payment creation runs inside one transaction. Orders and payments use explicit state enums (UPI, card, net banking).
**DevOps:** Dockerized, with GitHub Actions running tests, then building the image and pushing it to Amazon ECR using OIDC (no long-lived AWS keys) and a least-privilege IAM role. Images are tagged with the git SHA.
`Java 17` `Spring Boot` `MySQL` `JPA/Hibernate` `Docker` `GitHub Actions` `AWS ECR`

### 🤖 [Paytm Payment Resolution Assistant](https://github.com/mathalapavankalyan/paytm-resolve)
**Problem:** Payment support questions ("payment failed but money was deducted") need an investigation, not a generic chatbot reply.
**What I built:** A four-stage LangGraph pipeline (understand → investigate → resolve → respond) that turns a message into structured intent, looks up transaction, refund, and policy records, and applies deterministic resolution rules. Progress streams to a React UI over Server-Sent Events, so users see each step, a transaction card, and a resolution card.
**Design choice:** The LLM interprets language; the decision comes from structured data and rules, which reduces hallucination risk.
`React` `Vite` `FastAPI` `LangGraph` `Pydantic` `SSE`

### ⚖️ [Load Balancer](https://github.com/mathalapavankalyan/load-balancer)
**Problem:** Show how one service scales horizontally behind a single entry point.
**What I built:** Three Spring Boot instances behind Nginx (round-robin) sharing one MySQL 8 database, all orchestrated with Docker Compose.
`Spring Boot` `Nginx` `MySQL` `Docker Compose`

## 🧰 Tech Stack

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=dark">
    <img alt="Tech stack" src="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=light">
  </picture>
</p>

**Backend:** Java, Spring Boot, Spring Data JPA, REST, FastAPI · **Frontend:** React, JavaScript
**AI:** LangGraph, LangChain, agentic workflows · **Data:** MySQL, MongoDB
**DevOps:** Docker, Docker Compose, Nginx, GitHub Actions, AWS (ECR, IAM)

## 🔭 Currently

- 🔨 Building: [CURRENT_PROJECT]
- 📚 Learning: [e.g. Redis, Kafka, system design]

## 🐍 Contributions

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/mathalapavankalyan/mathalapavankalyan/output/github-contribution-grid-snake-dark.svg">
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/mathalapavankalyan/mathalapavankalyan/output/github-contribution-grid-snake.svg">
  </picture>
</p>

<details>
<summary><b>🏆 Achievements & more</b></summary>

- Two-time Inter-College CodeHack winner
- Top scorer, NPTEL Joy of Computing

</details>

---

<p align="center"><i>If my work fits what you're looking for, let's talk. Stars on the repos are always appreciated ⭐</i></p>
