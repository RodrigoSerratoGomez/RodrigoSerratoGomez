<h1 align="center">Rodrigo Serrato</h1>

<p align="center">
  <b>Full Stack Engineer</b> &nbsp;·&nbsp; .NET &nbsp;·&nbsp; SQL Server &nbsp;·&nbsp; TypeScript
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Arequipa,_Peru-UTC--5-0b7285?style=flat-square" alt="Arequipa, Peru - UTC-5" />
  <img src="https://img.shields.io/badge/4_years-fintech_platforms-2b8a3e?style=flat-square" alt="4 years on fintech platforms" />
  <img src="https://img.shields.io/badge/open_to-B2B_contract-862e9c?style=flat-square" alt="Open to B2B contract" />
</p>

---

### Hello

I build financial systems — factoring, guarantees, insurance and credit — where being wrong
costs money. For the last two years, fully remote from Peru for a fintech in **Santiago, Chile**:
another country, another timezone, no office.

I work on both ends, and my best work lives in two places most people find boring.

---

### Making slow things fast

A core invoice-management endpoint went from **242 seconds to 12** for the 29 operations staff
who opened it every day. I profiled the execution plans first, because I wanted the real cause
and not a guess — then rewrote the critical stored procedures, redesigned indexes across 6+
tables, and paginated and decomposed a monolithic endpoint.

| | Before | After |
| :-- | --: | --: |
| Response time | 242 s | **12 s** |
| Query cost | ~125,000 ms | **~2,300 ms** |
| Logical reads | ~4.5M | **~23K** |

Payroll batch processing got the same treatment with a Unit of Work and a single commit:
14 payrolls went from ~24 minutes to ~48 seconds, and commits per batch from 672 to 14.

### Making unsafe things safe

After an external ethical-hacking audit I implemented endpoint-level authorization across
**228 endpoints** — roles and claims with a dynamic permission scheme in Redis, plus OAuth2/JWT
via Microsoft Entra ID — and led the technical coordination of the fix.

---

### Front end is not the half I skip

I ship interfaces, not just APIs.

- **Next.js, React, TypeScript, Tailwind, SWR** — the front end and BFF of our internal delivery
  platform, where a ticket auto-creates its GitHub branch and the whole flow runs from the UI or
  from a chat client through an MCP integration. It became the only path the team used to close
  a user story.
- **Flutter across mobile, desktop and web** — one codebase for a cryptocurrency exchange client.
  One implementation of every screen and validation rule, instead of three clients drifting apart.
- **React + WebSocket in production on a national news site** — a real-time crypto price feed that
  ran on RPP Noticias, one of Peru's largest, released in coordination with their own engineering
  team. Someone else's review process, release window and infrastructure.
- **Three.js and react-three-fiber** — see ArchiVR below.

---

### On AI, I am on both sides of it

I helped build **Hermes**, an agent that lives in Microsoft Teams, grounded on our official
product documentation, that resolves around **90% of recurring incidents** on two product lines
autonomously and reviews pull requests.

I use Claude Code, Cursor and Copilot daily — and the part that matters is the review, not the
generation. I read what they produce the way I read a junior's pull request, and I run my own
AI-assisted work through a written verification loop. That loop is how I caught requirements a
model reported as finished and had hallucinated.

---

### The one thing here that is entirely mine

**[ArchiVR](https://archivr-2c65c.web.app/)** — a 3D experience that runs in your browser with no
install, built with **Three.js** and **react-three-fiber**. Mechanics, interface and deployed
build, end to end. It grew out of my thesis on gamifying architectural spatiality: understanding
space by moving through it rather than looking at a render.

### Why the rest of this profile is quiet

**The code I am proudest of is not mine to publish** — it belongs to the companies I built it for.
So what is left here is mostly coursework from when I was learning, and I have left it visible
rather than tidied away. It is where I started, not where I am.

---

### Stack

**Backend**

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET_6/7/8-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-5C2D91?style=flat-square&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![REST](https://img.shields.io/badge/REST_/_OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white)

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)

**Data**

![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![T-SQL](https://img.shields.io/badge/T--SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

**Security, delivery and quality**

![Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![OAuth2](https://img.shields.io/badge/OAuth2_/_JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azuredevops&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)
![xUnit](https://img.shields.io/badge/xUnit-512BD4?style=flat-square&logo=dotnet&logoColor=white)

---

### Certifications

AWS Cloud Practitioner (CLF-C02) and Solutions Architect – Associate (SAA-C03) — **in progress**,
exams scheduled for September and October 2026. Azure Fundamentals (Codigo Facilito, 2026) ·
Unit Testing with C#/.NET (Platzi, 2025) · AI Development (BigSchool, 2026).

BSc in Computer and Systems Engineering, Universidad de San Martin de Porres, 2020–2024.

---

<p align="center">
  <a href="https://www.linkedin.com/in/rodrigo-rafael-serrato-gomez">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:ing_rodrigo_serrato@outlook.com">
    <img src="https://img.shields.io/badge/Email-0078D4?style=for-the-badge&logo=microsoftoutlook&logoColor=white" alt="Email" />
  </a>
  <a href="https://archivr-2c65c.web.app/">
    <img src="https://img.shields.io/badge/ArchiVR-live_demo-FF6B35?style=for-the-badge" alt="ArchiVR live demo" />
  </a>
</p>
