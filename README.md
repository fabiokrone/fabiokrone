<div align="center">

# Fabio Krone

**Full-stack engineer shipping AI for the Brazilian public sector**
Founder @ [TermoCerto](https://termocerto.com.br) · Santa Catarina, Brazil

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/fabiokrone)
[![Email](https://img.shields.io/badge/-Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:fabiokrone10@gmail.com)
[![Website](https://img.shields.io/badge/-termocerto.com.br-1A3C6E?style=for-the-badge&logo=google-chrome&logoColor=white)](https://termocerto.com.br)

</div>

---

## About

I build software for Brazilian municipalities — the kind of infrastructure that touches real public servants, real payrolls, and real procurement processes. My work sits at the intersection of **full-stack engineering, applied AI, and public-sector compliance**.

- Technical advisor to **8 municipalities** in Santa Catarina (payroll, HR, compliance)
- Systems **serving 550+ public servants** in production
- Founder & principal engineer of **[TermoCerto](https://termocerto.com.br)** — AI platform for public procurement under Lei 14.133/2021
- Specialization in **Cybersecurity** (UNIBF, in progress) · Background in **Data Science** (Ada Tech)
- **Portuguese** (native) · **English** (fluent) · **German** (professional)

---

## Currently shipping

### [TermoCerto](https://termocerto.com.br) — AI platform for public procurement &nbsp; `Live in production`

End-to-end SaaS that turns a procurement request into a **defensible dossier** (DFD + ETP + TR + Pesquisa de Preços + Justificativa) under Brazil's new procurement law (Lei 14.133/2021). Web + WhatsApp interfaces.

<details>
<summary><b>Why this problem is hard</b></summary>
<br>

Brazilian public procurement requires every document to cite the right statute, every price reference to be traceable, and every methodology decision to be auditable by TCU (the federal audit court). A hallucinated citation is a legal risk. A wrong median is a nullified tender.

The platform integrates **5 government data sources** (PNCP, Portal de Compras Públicas, TCE-SC via Qlik Sense WebSocket, Compras.gov, internal pgvector of 33k+ contracts), runs a **14-family extractor pipeline** (IT hardware, furniture, vehicles, toner, paper, cleaning services, etc.) with deterministic regex-based spec extraction, applies **tri-state comparability** (match/mismatch/unknown), then an IQR-based benchmark engine to produce legally defensible price medians with a 95% t-Student confidence interval.

Document generation uses **Anthropic Claude** with a versioned RAG of **325 chunks** of Brazilian procurement law (Lei 14.133 + 6 SEGES/ME Normative Instructions + TCU súmulas and acórdãos). Every LLM call is logged with tokens, cost and RAG context for full auditability.

</details>

**Engineering snapshot:**
- **613 commits** in the last 2 months · single-engineer development
- **962 automated tests** · 97% coverage on end-to-end audit suite
- **5 government data sources** integrated · **14 product families** supported
- **325-chunk legal RAG** with reranker · multi-tenant PostgreSQL with Row-Level Security
- Measured unit economics: **~US$0.40 per generated dossier** in LLM cost
- **INPI-registered software** (process nº 512026002577-0) · **ABES** affiliation in progress

**Stack:**
![Python](https://img.shields.io/badge/Python_3.12-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_14-000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-4169E1?style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=flat-square&logo=minio&logoColor=white)
![Claude](https://img.shields.io/badge/Anthropic_Claude-6B4FBB?style=flat-square&logo=anthropic&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)

> Source is closed (commercial SaaS). Live product at [termocerto.com.br](https://termocerto.com.br) · demo available on request.

---

## Other work

| Project | Description | Stack |
|---|---|---|
| **Folha Pro** | Municipal payroll & HR platform — payroll runs, benefits, tax calculations, eSocial/RAIS/DIRF compliance. Serving 8 municipalities and 550+ public servants. | React · FastAPI · Supabase |
| **PontoAgent** | Time-tracking agent with PL/pgSQL analytics for municipal attendance control. | PostgreSQL · PL/pgSQL |

---

## Tech

<div align="center">

**Backend** &nbsp;
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/-SQLAlchemy-D71F00?style=flat-square&logo=python&logoColor=white)
![Celery](https://img.shields.io/badge/-Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

**Frontend** &nbsp;
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/-Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/-shadcn%2Fui-000?style=flat-square&logo=shadcnui&logoColor=white)

**Data** &nbsp;
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/-pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Supabase](https://img.shields.io/badge/-Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white)
![MinIO](https://img.shields.io/badge/-MinIO-C72E49?style=flat-square&logo=minio&logoColor=white)

**AI / ML** &nbsp;
![Claude](https://img.shields.io/badge/-Anthropic_Claude-6B4FBB?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/-OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![RAG](https://img.shields.io/badge/-RAG_%2B_Reranker-6B4FBB?style=flat-square)

**Infra** &nbsp;
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Railway](https://img.shields.io/badge/-Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white)
![Cloudflare](https://img.shields.io/badge/-Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

</div>

---

## Domain expertise

![Lei 14.133/2021](https://img.shields.io/badge/Lei_14.133%2F2021-Nova_Lei_de_Licitações-1A3C6E?style=flat-square)
![IN SEGES/ME 65/2021](https://img.shields.io/badge/IN_SEGES%2FME_65%2F2021-Pesquisa_de_Preços-1A3C6E?style=flat-square)
![TCU](https://img.shields.io/badge/TCU-Jurisprudência_%26_Auditoria-1A3C6E?style=flat-square)
![TCE/SC](https://img.shields.io/badge/TCE%2FSC-Transparência-1A3C6E?style=flat-square)
![eSocial](https://img.shields.io/badge/eSocial-RAIS_%C2%B7_DIRF_%C2%B7_SEFIP-1A3C6E?style=flat-square)
![PNCP](https://img.shields.io/badge/PNCP-Portal_Nacional_de_Contratações-1A3C6E?style=flat-square)

---

## Education

- **Specialization in Cybersecurity** — UNIBF · *in progress*
- **Data Science Specialization** — Ada Tech (Let's Code), São Paulo · 2021–2022
- **B.Sc. Information Systems** — UNOESC, Santa Catarina · 2008–2013

---

<div align="center">

### Open to partnerships, consulting and roles

Especially at the intersection of **AI, public sector, and regulated domains.**

[![LinkedIn](https://img.shields.io/badge/-Let's_connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/fabiokrone)
[![Email](https://img.shields.io/badge/-Get_in_touch-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:fabiokrone10@gmail.com)

</div>
