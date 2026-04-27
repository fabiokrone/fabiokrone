# Fabio Krone

Full-stack engineer building AI products for the Brazilian public sector. Founder of [TermoCerto](https://termocerto.com.br). Based in Santa Catarina, Brazil.

[LinkedIn](https://linkedin.com/in/fabiokrone) · [Email](mailto:fabiokrone10@gmail.com) · [termocerto.com.br](https://termocerto.com.br)

---

## About

I build software for Brazilian municipalities — payroll systems, HR platforms, and procurement tools that operate under federal regulation and state-level audit. My work sits at the intersection of full-stack engineering, applied AI, and public-sector compliance.

Currently:

- Technical advisor to eight municipalities in Santa Catarina (payroll, HR, procurement compliance).
- Systems serving 550+ public servants in production.
- Founder and principal engineer of TermoCerto, an AI platform for procurement under Brazil's Law 14.133/2021.

Languages: Portuguese (native), English (fluent), German (professional).

---

## Currently shipping

### TermoCerto — AI platform for public procurement

End-to-end SaaS that turns a procurement request into a defensible dossier — scope definition, preliminary technical study, statement of work, and price research with full justification — under Brazil's procurement law (Law 14.133/2021). Available as a web application and through a WhatsApp interface.

The problem is harder than it looks. Brazilian public procurement requires every document to cite the correct statute, every reference price to be traceable to its source, and every methodological choice to be defensible before federal and state audit courts. A hallucinated citation is a legal risk; a wrong median is a nullified tender. Generic AI assistants fail this bar by default.

The platform integrates five government data sources (PNCP, the federal procurement portal, TCE-SC via Qlik Sense WebSocket, Compras.gov, and an internal pgvector store of 33,000+ contracts), runs a fourteen-family extractor pipeline with deterministic regex-based specification matching, applies a tri-state comparability judge (match / mismatch / unknown), and produces legally defensible price medians with a 95% Student-t confidence interval over the IQR-filtered sample.

Document generation is built on Anthropic Claude with a versioned RAG index of 325 chunks covering Law 14.133/2021, six SEGES/ME normative instructions, and Federal Audit Court precedents. Every model call is logged with token usage, cost, and retrieved context, so any decision the system makes can be reconstructed for audit.

**Selected technical details**

- Multi-tenant PostgreSQL with row-level security; Celery for asynchronous processing; pgvector for semantic retrieval.
- 962 automated tests with 97% coverage on the end-to-end audit suite — the suite that mirrors the audit court review path.
- Measured unit economics: roughly US$0.40 in LLM cost per generated dossier.
- Single-engineer development from the ground up.

Built with Python 3.12, FastAPI, Celery, PostgreSQL 16, pgvector, Redis, MinIO, Next.js 14, TypeScript, Tailwind CSS, Anthropic Claude, deployed on Railway behind Cloudflare.

Source is closed (commercial SaaS). The product is live at [termocerto.com.br](https://termocerto.com.br); a guided demo is available on request.

---

## Other work

**Folha Pro.** Municipal payroll and HR platform — payroll runs, benefits administration, tax calculations, and eSocial / RAIS / DIRF compliance. In production across eight municipalities, serving 550+ public servants. React, FastAPI, Supabase.

**PontoAgent.** Time-tracking system with PL/pgSQL analytics for municipal attendance control. PostgreSQL with stored procedures for shift validation, exception detection, and consolidated reporting.

---

## Domain background

Brazilian public administration, with depth in Law 14.133/2021 (federal procurement), Normative Instruction SEGES/ME 65/2021 (price research methodology), eSocial and adjacent labor reporting (RAIS, DIRF, SEFIP), and audit-court practice at federal level (TCU) and state level (TCE-SC). Technical writing in Portuguese for legal-administrative audiences.

---

## Education

- Specialization in Cybersecurity — UNIBF (in progress).
- Data Science Specialization — Ada Tech (Let's Code), São Paulo, 2021–2022.
- B.Sc. in Information Systems — UNOESC, Santa Catarina, 2008–2013.

---

Open to consulting, partnerships, and roles where AI meets regulated public-sector domains. Reach out via [LinkedIn](https://linkedin.com/in/fabiokrone) or [email](mailto:fabiokrone10@gmail.com).
