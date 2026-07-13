<picture>
  <source media="(prefers-color-scheme: dark)" srcset="dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="light.svg">
  <img src="dark.svg" alt="Anushka Dhawas — Java Backend Developer" width="100%"/>
</picture>

<br/>

## 🚀 About Me

Java Backend Developer focused on **distributed systems**, **fintech infrastructure**, and **microservices architecture**. Final-year B.Tech ECE student at ABES Engineering College (2026), with internship experience at **Zoho Corporation**.

Currently building production-grade backend systems — most notably **UPI Mesh Network**, an offline-first distributed payment platform.

---

## 🔥 Featured Project — UPI Mesh Network

> Offline-first distributed payment platform using gossip protocol propagation

**What it does:** Encrypted payment packets travel peer-to-peer through nearby devices when there's no internet. A bridge node with 4G relays the packet to the cloud backend, which validates and settles the transaction atomically.

**Architecture highlights:**
- RSA-OAEP + AES-256-GCM end-to-end encryption on every MeshPacket
- Gossip protocol propagation with TTL decrement per hop
- Redis SETNX idempotency — exactly-once settlement guaranteed
- Kafka `payment.settled` event → async notification to both parties
- Spring `@Transactional` atomic PostgreSQL settlement
- Full Docker Compose local dev setup

[![Repo](https://img.shields.io/badge/GitHub-upi--offline--mesh-22D3EE?style=for-the-badge&logo=github&logoColor=white)](https://github.com/anushkad17/upi-offline-mesh)

---

## 🛠️ Tech Stack

| Layer | Technologies |
|---|---|
| **Backend** | Java · Spring Boot · Spring Security · OAuth2/JWT |
| **Messaging** | Apache Kafka |
| **Caching** | Redis |
| **Database** | PostgreSQL · Hibernate JPA |
| **DevOps** | Docker · Docker Compose |
| **Frontend** | React.js |
| **Cloud** | AWS (Cloud Practitioner ✓) |
| **Security** | RSA-OAEP · AES-256-GCM · JWT |

---

## 📌 Other Projects

| Project | Stack | Links |
|---|---|---|
| **CutLink** — URL shortener with analytics & JWT auth | Spring Boot · PostgreSQL · React · Docker | [![Live](https://img.shields.io/badge/Live-cutlinkurl.netlify.app-10B981?style=flat-square)](https://cutlinkurl.netlify.app) |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=anushkad17&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0F172A&title_color=22D3EE&icon_color=7C3AED&text_color=F8FAFC" height="160"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=anushkad17&layout=compact&theme=tokyonight&hide_border=true&bg_color=0F172A&title_color=22D3EE&text_color=F8FAFC" height="160"/>
</p>

---

## 🔗 Connect

<p>
  <a href="https://github.com/anushkad17"><img src="https://img.shields.io/badge/GitHub-anushkad17-181717?style=for-the-badge&logo=github"/></a>
  &nbsp;
  <a href="https://linkedin.com/in/anushka-dhawas-b9300a266"><img src="https://img.shields.io/badge/LinkedIn-Anushka_Dhawas-0A66C2?style=for-the-badge&logo=linkedin"/></a>
  &nbsp;
  <a href="https://anushhka.dev"><img src="https://img.shields.io/badge/Portfolio-anushhka.dev-22D3EE?style=for-the-badge&logo=vercel&logoColor=white"/></a>
</p>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=anushkad17&color=7C3AED&style=flat-square&label=profile+views"/>
</p>

<p align="center">
  <sub>Open to fresher backend / full-stack roles · Noida, India · Available immediately</sub>
</p>
