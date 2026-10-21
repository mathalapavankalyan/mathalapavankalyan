<p align="center">
  <img src="assets/banner.svg" alt="Pavankalyan Mathala: Backend, Full-Stack and AI Engineer" width="100%">
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=DAA520&center=true&vCenter=true&width=480&height=44&lines=Charged+twice%3F+Not+on+my+watch.;Same+request%2C+10+retries%2C+1+payment;The+LLM+talks.+The+rules+decide.;3+Spring+Boot+servers%2C+1+Nginx%2C+0+drama">
    <img alt="Charged twice? Not on my watch. Same request, 10 retries, 1 payment. The LLM talks, the rules decide." src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=17&duration=3000&pause=900&color=9A7209&center=true&vCenter=true&width=480&height=44&lines=Charged+twice%3F+Not+on+my+watch.;Same+request%2C+10+retries%2C+1+payment;The+LLM+talks.+The+rules+decide.;3+Spring+Boot+servers%2C+1+Nginx%2C+0+drama">
  </picture>
</p>

<p align="center">
  <a href="#projects"><img src="assets/icons/code.svg" height="16" align="absmiddle" alt=""> <b>Projects</b></a> &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="#stack"><img src="assets/icons/layers.svg" height="16" align="absmiddle" alt=""> <b>Stack</b></a> &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="#contact"><img src="assets/icons/mail.svg" height="16" align="absmiddle" alt=""> <b>Contact</b></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OPEN_TO_WORK-Backend_%7C_Full--Stack_%7C_AI_Engineer-DAA520?style=for-the-badge&labelColor=111111" alt="Open to work: Backend, Full-Stack, AI Engineer"/>
</p>

---

<h2><img src="assets/icons/user.svg" height="26" align="absmiddle" alt=""> About</h2>

I build backends that survive retries, race conditions, and users mashing the Pay button twice.
Java and Spring Boot for the serious parts, React for the pretty parts, and LangGraph for when an LLM needs to be useful without being trusted near the money.

**Looking for:** entry-level Backend, Full-Stack, or AI Engineering roles. I will treat your production database with the respect of a very nervous person.

<a id="projects"></a>

<h2><img src="assets/icons/code.svg" height="26" align="absmiddle" alt=""> Projects</h2>

### <img src="assets/icons/shield.svg" height="22" align="absmiddle" alt=""> [Payment Gateway](https://github.com/mathalapavankalyan/payment-gateway)
*"Charged twice? Not on my watch."*

**The problem:** Users double-tap Pay, networks drop, clients retry, and the customer should still be charged exactly once.
**The fix:** Every request carries an `Idempotency-Key`, plus a hash of the payload, so reusing a key with a different amount gets rejected (a ₹500 key can't sneak in a ₹5000 payment). When two requests race, a database unique constraint is the final referee, and payment creation runs in a single transaction. CI runs the tests, builds the Docker image, and pushes it to Amazon ECR through GitHub OIDC: no long-lived AWS keys, least-privilege IAM role.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,mysql,docker,githubactions,aws&theme=dark">
  <img alt="Java, Spring Boot, MySQL, Docker, GitHub Actions, AWS" src="https://skillicons.dev/icons?i=java,spring,mysql,docker,githubactions,aws&theme=light">
</picture>

### <img src="assets/icons/cpu.svg" height="22" align="absmiddle" alt=""> [Paytm Payment Resolution Assistant](https://github.com/mathalapavankalyan/paytm-resolve)
*"The LLM talks. The rules decide."*

**The problem:** "Payment failed but money was deducted" is five words and one very stressed user, and a generic chatbot reply doesn't help.
**The fix:** A four-stage LangGraph pipeline (understand → investigate → resolve → respond) that turns the message into structured intent, looks up the transaction, refund, and policy records, and applies deterministic resolution rules. The model understands language; it doesn't get to improvise a refund. Progress streams to a React UI over Server-Sent Events, so users watch the investigation instead of staring at a spinner.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=react,vite,python,fastapi&theme=dark">
  <img alt="React, Vite, Python, FastAPI" src="https://skillicons.dev/icons?i=react,vite,python,fastapi&theme=light">
</picture>
<img src="https://img.shields.io/badge/LangGraph-111111?style=for-the-badge&logo=langchain&logoColor=DAA520" alt="LangGraph" align="top">

### <img src="assets/icons/share.svg" height="22" align="absmiddle" alt=""> [Load Balancer](https://github.com/mathalapavankalyan/load-balancer)
*"3 servers, 1 Nginx, 0 drama."*

**The problem:** One server shouldn't have to carry the whole crowd.
**The fix:** Three Spring Boot instances behind Nginx doing round-robin, all sharing one MySQL 8 database, started with a single `docker compose up`.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,nginx,mysql,docker&theme=dark">
  <img alt="Java, Spring Boot, Nginx, MySQL, Docker" src="https://skillicons.dev/icons?i=java,spring,nginx,mysql,docker&theme=light">
</picture>

<a id="stack"></a>

<h2><img src="assets/icons/layers.svg" height="26" align="absmiddle" alt=""> Stack</h2>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=dark&perline=7">
    <img alt="Java, Spring Boot, React, JavaScript, Python, FastAPI, MySQL, MongoDB, Docker, Nginx, GitHub Actions, AWS, Git" src="https://skillicons.dev/icons?i=java,spring,react,js,python,fastapi,mysql,mongodb,docker,nginx,githubactions,aws,git&theme=light&perline=7">
  </picture>
</p>

**Backend:** Java, Spring Boot, Spring Data JPA, FastAPI · **Frontend:** React, JavaScript
**AI:** LangGraph, LangChain · **Data:** MySQL, MongoDB
**DevOps:** Docker, Nginx, GitHub Actions, AWS (ECR, IAM)

<h2><img src="assets/icons/compass.svg" height="26" align="absmiddle" alt=""> Currently</h2>

- **Next on my own roadmap:** Redis, Kafka, Terraform. My Payment Gateway README lists them under "production hardening," so I'm basically legally obligated.

<a id="contact"></a>

<h2><img src="assets/icons/mail.svg" height="26" align="absmiddle" alt=""> Contact</h2>

<a href="https://pavankalyan-portfolio-eight.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-111111?style=for-the-badge&logo=vercel&logoColor=DAA520" alt="Portfolio"></a>
<a href="https://www.linkedin.com/in/pavankalyan-mathala/"><img src="https://img.shields.io/badge/LinkedIn-111111?style=for-the-badge&logo=linkedin&logoColor=DAA520" alt="LinkedIn"></a>
<a href="mailto:mathalapavankalyan@gmail.com"><img src="https://img.shields.io/badge/Email-111111?style=for-the-badge&logo=gmail&logoColor=DAA520" alt="Email"></a>

Fastest reply: email. Slowest: carrier pigeon.

<details>
<summary><img src="assets/icons/award.svg" height="18" align="absmiddle" alt=""> <b>Achievements</b></summary>

- Two-time Inter-College CodeHack winner (the second one wasn't a fluke)
- Top scorer, NPTEL Joy of Computing

</details>

---

<p align="center"><i>Star a repo and I'll say thanks exactly once, no matter how many times you click. It's idempotent.</i></p>
