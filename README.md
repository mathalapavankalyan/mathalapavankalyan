<p align="center">
  <img src="assets/banner.svg" alt="Pavan Kalyan Mathala — Java Backend & Agentic AI Engineer" width="100%">
</p>

<p align="center">
  <strong>Java Backend Engineer · Spring Boot · AWS · Distributed Systems · Agentic AI</strong>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/pavankalyan-mathala/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin" alt="LinkedIn"></a>
  <a href="https://pavankalyan-portfolio-eight.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-Visit-111111?style=flat-square&logo=vercel" alt="Portfolio"></a>
  <a href="mailto:mathalapavankalyan@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail" alt="Email"></a>
  <a href="https://leetcode.com/u/pavanmathala"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode profile"></a>
</p>

About
I'm a Java backend engineer with 2+ years of experience building backend services and exploring AI-powered applications across healthcare and payment-related use cases. I focus on reliable APIs, business-rule execution, performance, failure handling, and practical agentic AI.

My core stack is Java 17, Spring Boot, SQL/NoSQL databases, and AWS. I also build AI workflows with RAG, LangGraph, tool calling, and MCP, with deterministic validation around decisions that require correctness.
- Backend: API design, service-layer architecture, transactions, idempotency, concurrency, and testing
- Cloud & delivery: AWS, Docker, GitHub Actions, and CI/CD
- AI systems: Retrieval-augmented generation, tool orchestration, session memory, and deterministic lookups
- Currently building: Backend projects that demonstrate reliability and AI systems that are useful, testable, and grounded in data
Selected Impact
Selected results from my work at Endava; details should be shared only where permitted.
Result	Engineering work
15s → 2s repeat plan evaluation	Added Redis caching keyed by plan ID and configuration to avoid recalculating identical requests
~8 hrs → ~2 hrs for 10,000+ reports	Reworked report generation into batch processing and expanded output from PDF to PDF + Excel with multi-attachment email delivery
15 → 6 min deployments; 88% JUnit coverage	Built per-Lambda GitHub Actions pipelines using OIDC and redeploying only changed Lambdas
Clear terminal status for retry-exhausted work	Added SQS dead-letter handling that marks exhausted plan requests as FAILED instead of leaving them without a visible outcome
50,000-plan catalog; 5–6k daily users	Delivered client-specific plan configuration features on a healthcare plan platform


Experience
Endava — Software Developer
September 2025 – Present · Benefit Calculation Rules Platform
- Worked on a serverless REST rules engine that replaced an Excel-based benefit-rules workflow.
- Built API Gateway and AWS Lambda components for evaluating configured plan scenarios.
- Worked with a team of seven on a platform evaluating approximately 8–10 scenarios per plan.
- Explored and delivered GenAI and agentic AI proofs of concept alongside backend engineering work.
Technologies: Java, Spring Boot, AWS Lambda, API Gateway, DynamoDB, Redis, GitHub Actions
Endava — Associate Software Engineer
August 2024 – September 2025 · Healthcare Plan Management Platform
- Built a Kafka consumer in the rule service to apply business rules to plan events and validate them against configured constraints.
- Contributed to backend services supporting healthcare plan management workflows.
Technologies: Java, Spring Boot, Kafka, Redis
Featured Projects
Idempotent Payment Gateway
A Java/Spring Boot payment gateway project focused on preventing duplicate payment processing when clients retry requests or requests race.
- Accepts an Idempotency-Key and validates a request hash to reject reuse of a key with a different payload.
- Uses a database uniqueness constraint as a concurrency safeguard.
- Models order and payment states and uses transactional boundaries for state changes.
- Includes tests for duplicate requests, key reuse, concurrency, and rollback scenarios.
- Uses GitHub Actions and OpenID Connect (OIDC) for CI delivery to Amazon ECR.
Stack: Java 17, Spring Boot, MySQL, Docker, GitHub Actions, AWS ECR
Payment-Resolution Assistant
A multilingual payment-issue assistant built for the Paytm Build for India AI Hackathon.
- Uses LangGraph for intent understanding, tool selection, and session memory.
- Uses deterministic search for payment lookups rather than relying on an LLM to invent transaction outcomes.
- Streams investigation progress to a React interface using Server-Sent Events.
- Built by a two-person team; the project was reported as a Top 20 entry among approximately 4,774 participants.
Stack: Python, FastAPI, LangGraph, React
Load Balancer
A containerized setup demonstrating multiple Spring Boot instances behind an Nginx reverse proxy.
- Runs three backend instances behind Nginx round-robin routing.
- Shares a MySQL 8 database across instances.
- Starts with Docker Compose.
Stack: Java, Spring Boot, Nginx, Docker Compose, MySQL
GenAI & Agentic AI
Plan Recommendation Assistant — RAG, Knowledge Graph & MCP
- Built a retrieval pipeline over approximately 100 policy and rules documents using OpenAI embeddings and Chroma.
- Used a weighted knowledge graph in MongoDB with signals such as age, monthly premium, and plan type to rank relevant policies.
- Exposed backend capabilities through FastAPI tools and MCP interfaces so the agent interacts through defined tool contracts rather than directly accessing underlying data sources.
- Demonstrated the project to leadership and a client.
AI-Native Workforce Management System
Winner, APAC — OpenAI × Endava Codex Hackathon (55+ teams).

Designed a multi-agent workflow to recommend available candidates for opportunities based on role details. Built with Codex, React, Python, and FastAPI.
Technical Skills
Area	Technologies
Languages	Java 17, Python, SQL
Backend	Spring Boot, REST APIs, Hibernate/JPA, FastAPI, JUnit, Mockito
AI & Agentic Systems	LangChain, LangGraph, RAG, OpenAI Embeddings, Chroma, knowledge graphs, MCP, tool calling
Databases & Messaging	MySQL, Microsoft SQL Server, MongoDB, DynamoDB, Redis, Kafka, Amazon SQS
Cloud & DevOps	AWS Lambda, API Gateway, S3, DynamoDB, ECR, Docker, Git, GitHub Actions, OIDC


Achievements & Education
- Winner, APAC: OpenAI × Endava Codex Hackathon (55+ teams)
- Top 20: Paytm Build for India AI Hackathon (approximately 4,774 participants, as reported)
- Two-time winner: Inter-College CodeHack
- Top scorer: NPTEL Joy of Computing
- B.Tech in Computer Science: NRI Institute of Technology, 2020–2024 · CGPA 8.6/10
Contact
- Portfolio: https://pavankalyan-portfolio-eight.vercel.app/
- LinkedIn: https://www.linkedin.com/in/pavankalyan-mathala/
- Email: mathalapavankalyan@gmail.com
- LeetCode: https://leetcode.com/u/pavanmathala
<p align="center">
  <em>I build backend systems that behave predictably under retries, failures, and real-world con
