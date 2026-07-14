<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=200&section=header&text=Anushka%20Dhawas&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Java%20Backend%20Developer&descAlignY=58&descSize=18&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=3000&pause=800&color=A78BFA&center=true&vCenter=true&multiline=false&width=680&lines=Java+Backend+Developer+%7C+Spring+Boot+Engineer;Distributed+Systems+%7C+Fintech+Infrastructure;Kafka+%7C+Redis+%7C+PostgreSQL+%7C+Docker;Open+to+Fresher+SDE+%7C+Backend+Roles)](https://git.io/typing-svg)

<br/>

![B.Tech ECE](https://img.shields.io/badge/B.Tech-Electrical_%26_Computer_Engineering-7C3AED?style=for-the-badge&logo=graduation-cap&logoColor=white)
![ABES Engineering](https://img.shields.io/badge/ABES_Engineering_College-2022--2026-4F46E5?style=for-the-badge&logo=university&logoColor=white)
![India](https://img.shields.io/badge/📍_Noida%2C_India-1E1B4B?style=for-the-badge)

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-anushhka.dev-7C3AED?style=for-the-badge&logo=vercel&logoColor=white)](https://anushhka.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Anushka_Dhawas-4F46E5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anushka-dhawas-b9300a266/)
[![Email](https://img.shields.io/badge/Email-anushkad178@gmail.com-6D28D9?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anushkad178@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-anushkad17-312E81?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anushkad17)

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=anushkad17&style=for-the-badge&color=7C3AED&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/anushkad17?style=for-the-badge&color=4F46E5&label=FOLLOWERS&logo=github&logoColor=white)

</div>

---

## 〈 About 〉

```yaml
name       : Anushka Dhawas
role       : Java Backend Developer
location   : Noida, India
education  : B.Tech ECE — ABES Engineering College (2022–2026)
internship : Zoho Corporation — Java Backend Intern
```

I'm a backend-focused developer building **distributed systems**, **microservices**, and **event-driven architectures** with Java and Spring Boot. My internship at **Zoho Corporation** gave me hands-on exposure to production-grade Spring Boot microservices, OAuth2/JWT security, and CI/CD pipelines.

My flagship project — **UPI Mesh Network** — is an offline-first distributed payment platform that routes encrypted payments peer-to-peer through nearby devices using a gossip protocol, with Redis idempotency guaranteeing exactly-once settlement.

**Open To:**
- Fresher / Junior SDE roles at product-led companies
- Java backend and full-stack engineering positions
- Fintech startups and cloud-native backend teams

---

## 〈 Tech Stack 〉

<div align="center">

**Languages**

[![Java](https://skillicons.dev/icons?i=java)](https://java.com)
[![Python](https://skillicons.dev/icons?i=python)](https://python.org)
[![JavaScript](https://skillicons.dev/icons?i=js)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![HTML](https://skillicons.dev/icons?i=html)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://skillicons.dev/icons?i=css)](https://developer.mozilla.org/en-US/docs/Web/CSS)

**Frontend**

[![React](https://skillicons.dev/icons?i=react)](https://reactjs.org)

**Backend & Databases**

[![Spring](https://skillicons.dev/icons?i=spring)](https://spring.io)
[![Docker](https://skillicons.dev/icons?i=docker)](https://docker.com)
[![PostgreSQL](https://skillicons.dev/icons?i=postgres)](https://postgresql.org)
[![MySQL](https://skillicons.dev/icons?i=mysql)](https://mysql.com)
[![Redis](https://skillicons.dev/icons?i=redis)](https://redis.io)
[![Kafka](https://skillicons.dev/icons?i=kafka)](https://kafka.apache.org)

**Cloud & Tooling**

[![AWS](https://skillicons.dev/icons?i=aws)](https://aws.amazon.com)
[![Git](https://skillicons.dev/icons?i=git)](https://git-scm.com)
[![Linux](https://skillicons.dev/icons?i=linux)](https://linux.org)
[![Maven](https://skillicons.dev/icons?i=maven)](https://maven.apache.org)

</div>

---

## 〈 Featured Projects 〉

<details>
<summary><b>⬡ &nbsp;UPI Mesh Network &nbsp;—&nbsp; Offline-First Distributed Payment Platform</b></summary>

<br/>

An offline-first distributed payment platform that routes encrypted payment packets peer-to-peer through nearby devices using a **gossip protocol** — no internet required on the sender's side. A bridge node with connectivity relays the packet to the cloud backend, which validates and settles atomically.

<br/>

| Attribute | Detail |
|-----------|--------|
| **Stack** | Java · Spring Boot · Apache Kafka · Redis · PostgreSQL · Docker |
| **Security** | RSA-OAEP + AES-256-GCM end-to-end encryption on every MeshPacket |
| **Idempotency** | Redis SETNX guarantees exactly-once transaction settlement |
| **Notifications** | Kafka `payment.settled` → JavaMailSender async email to both parties |
| **Settlement** | Spring `@Transactional` atomic PostgreSQL write |
| **Dev** | Full Docker Compose local setup |
| **Repository** | [![GitHub](https://img.shields.io/badge/View_Repo-7C3AED?style=flat-square&logo=github&logoColor=white)](https://github.com/anushkad17/upi-offline-mesh) |

**Architecture flow:** Sender creates an encrypted MeshPacket → gossip propagation via stranger devices (TTL decrements each hop) → bridge node POSTs via HTTPS → 4-gate backend validation (SHA-256 hash → Redis SETNX → RSA+AES decrypt → 24hr freshness check) → PostgreSQL settlement → Kafka event → email notifications to both parties.

<br/>

</details>

<details>
<summary><b>⬡ &nbsp;AI Fitness Platform &nbsp;—&nbsp; Event-Driven Microservices Backend</b></summary>

<br/>

An event-driven fitness platform backend built on independently deployable Spring Boot microservices. Implements enterprise-grade identity and authorization using Keycloak RBAC and OAuth2/JWT across all service-to-service communication.

<br/>

| Attribute | Detail |
|-----------|--------|
| **Stack** | Spring Boot · Java · RabbitMQ · Keycloak · React.js · Docker |
| **Auth** | OAuth2/JWT + Keycloak RBAC for service-to-service authorization |
| **Messaging** | RabbitMQ decoupling services for async event-driven workflows |
| **Frontend** | React.js consuming backend REST APIs |
| **Repository** | [![GitHub](https://img.shields.io/badge/View_Repo-7C3AED?style=flat-square&logo=github&logoColor=white)](https://github.com/anushkad17) |

<br/>

</details>

<details>
<summary><b>⬡ &nbsp;CutLink &nbsp;—&nbsp; URL Shortener with Analytics</b></summary>

<br/>

A full-stack URL shortening platform with custom alias support, click analytics, and JWT-based authentication. Deployed on Netlify (frontend) and Render (backend) with Docker containerization for local development.

<br/>

| Attribute | Detail |
|-----------|--------|
| **Stack** | Spring Boot · Java · MySQL · React.js · Docker |
| **Auth** | JWT-based authentication |
| **Deployment** | Netlify (frontend) · Render (backend) |
| **Live Demo** | [![Live](https://img.shields.io/badge/Live_Demo-cutlinkurl.netlify.app-10B981?style=flat-square)](https://cutlinkurl.netlify.app) |
| **Repository** | [![GitHub](https://img.shields.io/badge/View_Repo-7C3AED?style=flat-square&logo=github&logoColor=white)](https://github.com/anushkad17) |

<br/>

</details>

<details>
<summary><b>⬡ &nbsp;Hierarchical Disease Prediction &nbsp;—&nbsp; Explainable AI Research Project</b></summary>

<br/>

A hierarchical disease prediction system using NLP and ML, built as a 3-person team project at ABES Engineering College. Combines sentence embeddings and gradient boosting with explainability tooling.

<br/>

| Attribute | Detail |
|-----------|--------|
| **Stack** | Python · SBERT · XGBoost · Explainable AI (XAI) |
| **Approach** | Hierarchical classification using sentence embeddings + gradient boosting |
| **Explainability** | XAI tooling to surface model reasoning for clinical predictions |
| **Deliverables** | Institutional report · Project poster · Front matter documentation |

<br/>

</details>

---

## 〈 Experience 〉

<div align="left">

### Java Backend Intern &nbsp;·&nbsp; Zoho Corporation
Noida, India

Worked on production Spring Boot microservices within Zoho's engineering environment. Owned security, reliability, and CI/CD automation deliverables across a multi-service Java backend architecture.

- Built and maintained REST API pipelines across Spring Boot microservices
- Implemented OAuth2/JWT authentication and RBAC authorization using Spring Security
- Set up CI/CD pipelines using Docker and GitHub Actions for automated deployments
- Collaborated with cross-functional teams in Agile/Scrum ceremonies and authored technical documentation

<br/>

![Java](https://img.shields.io/badge/Java-7C3AED?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-4F46E5?style=flat-square&logo=springboot&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-6D28D9?style=flat-square&logo=docker&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2%2FJWT-7C3AED?style=flat-square&logo=auth0&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-4F46E5?style=flat-square&logo=githubactions&logoColor=white)
![Microservices](https://img.shields.io/badge/Microservices-312E81?style=flat-square&logoColor=white)

</div>

---

## 〈 Achievements 〉

<div align="center">

| 🏆 Recognition | Details |
|----------------|---------|
| **2nd Place — HackHaven Hackathon** | Built and shipped a working product under time constraints |


</div>

---

## 〈 Certifications 〉

<div align="center">

[![AWS Cloud Practitioner](https://img.shields.io/badge/AWS_Cloud_Practitioner_Essentials-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/certification/)

</div>

---

## 〈 GitHub Analytics 〉

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=anushkad17&show_icons=true&theme=tokyonight&bg_color=0D0D1A&title_color=A78BFA&icon_color=7C3AED&text_color=C4B5FD&border_color=4F46E5&hide_border=false&count_private=true&include_all_commits=true"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anushkad17&layout=compact&theme=tokyonight&bg_color=0D0D1A&title_color=A78BFA&text_color=C4B5FD&border_color=4F46E5&hide_border=false&langs_count=8"/>

</div>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com?user=anushkad17&theme=tokyonight&background=0D0D1A&ring=7C3AED&fire=A78BFA&currStreakLabel=C4B5FD&sideLabels=C4B5FD&currStreakNum=ffffff&sideNums=ffffff&dates=6D28D9&border=4F46E5"/>

</div>

---

## 〈 GitHub Trophies 〉

<div align="center">

[![Trophies](https://github-profile-trophy.vercel.app/?username=anushkad17&theme=darkhub&column=7&margin-w=8&margin-h=8&no-bg=true&no-frame=false)](https://github.com/ryo-ma/github-profile-trophy)

</div>

---

## 〈 Contribution Activity 〉

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=anushkad17&bg_color=0D0D1A&color=A78BFA&line=7C3AED&point=C4B5FD&area=true&area_color=4F46E5&border_color=4F46E5&hide_border=false)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

---

## 〈 Contribution Snake 〉

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/anushkad17/anushkad17/output/github-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/anushkad17/anushkad17/output/github-snake.svg"/>
  <img alt="github contribution snake" src="https://raw.githubusercontent.com/anushkad17/anushkad17/output/github-snake-dark.svg"/>
</picture>

</div>

---

## 〈 Current Focus 〉

```yaml
learning:
  - System Design — distributed consensus, CAP theorem, idempotency patterns
  - DSA — sliding window, dynamic programming, graph traversal
  - AWS Solutions Architect concepts
  - Observability with Spring Boot Actuator

building:
  - Extending UPI Mesh Network with Kubernetes deployment
  - Kafka event streaming with schema registry
  - Spring Boot 3 with Java 21 virtual threads

open_to:
  - Fresher SDE roles at product-led companies
  - Java backend and full-stack positions
  - Fintech startups and distributed systems teams
  - Open source in Java / Spring ecosystem
```

---

## 〈 Connect 〉

<div align="center">

[![Gmail](https://img.shields.io/badge/Gmail-anushkad178@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anushkad178@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Anushka_Dhawas-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anushka-dhawas-b9300a266/)
[![GitHub](https://img.shields.io/badge/GitHub-anushkad17-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anushkad17)
[![Portfolio](https://img.shields.io/badge/Portfolio-anushhka.dev-7C3AED?style=for-the-badge&logo=vercel&logoColor=white)](https://anushhka.dev)

</div>

---

<div align="center">

*"Build systems that fail gracefully — then make sure they rarely have to."*

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>
