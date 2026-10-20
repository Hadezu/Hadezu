# Ivan Matiushkin

**Software Development, Integrations & Automation**  
*Internal business applications, API workflows, and data processing — delivered through deliberate AI-driven engineering.*

[Interactive Portfolio](https://work.matiushkin.com/en) · [Wersja polska](https://work.matiushkin.com/) · [Services](https://work.matiushkin.com/en/services/internal-applications) · [LinkedIn](https://www.linkedin.com/in/ivan-matiushkin-809694442/) · [Contact: ivan@matiushkin.com](mailto:ivan@matiushkin.com) · Poland (Remote)

---

## What I Deliver

I build practical software solutions for companies looking to automate operations, connect systems, or build custom operational tooling:

- **Internal Business Applications:** Multi-role operational dashboards, request review queues, and approval workflows.
- **API & Webhook Integrations:** Fault-tolerant webhook handlers, transactional inbox/outbox patterns, and synchronization pipelines.
- **Data Workflows & Protection:** Pre-import validation, duplicate/conflict prevention, and automated discrepancy reconciliation.
- **Extending Existing Systems:** Adding features, audit trails, and reliability checks to existing codebases without breaking upstream logic.

---

## Selected Work & Executable Proof

> **Independent Demonstrations:** The repositories below are independent portfolio proofs and open-source extensions built with synthetic/test data. They demonstrate implemented software mechanisms and verification discipline, not paid client deployments.

### 1. Operations Desk — Multi-Tenant Approval System
**Full-stack business application with concurrency control and audit trails.**
- **[Try the Live Interactive Demo](https://operations-desk-reliability.vanya-matyushkin.workers.dev)** *(Instant browser access; switch between Employee, Manager, and Observer roles; visitor-isolated workspace)*
- **Problem:** When multiple managers review requests concurrently, stale decisions can silently overwrite newer updates, or repeated submissions can trigger duplicate actions.
- **Solution:** A complete Next.js, Node.js/Fastify, PostgreSQL/Prisma, and Redis/BullMQ internal tool featuring tenant isolation, role-based access, idempotency keys, and crash-resilient worker recovery.
- **Verification Boundaries:** 
  - *Public Web Demo:* Hosted on Cloudflare Workers with a real Neon PostgreSQL database, demonstrating an interactive approval scenario across three synthetic roles in the browser.
  - *Local & CI Suite:* 40 automated API/database assertions and 5 worker-recovery scenarios tested in Docker Compose and GitHub Actions.
- **Links:** [Live Demo](https://operations-desk-reliability.vanya-matyushkin.workers.dev) · [Inspect Repository](https://github.com/Hadezu/operations-desk-reliability) · [Proof Manifest](https://operations-desk-reliability.vanya-matyushkin.workers.dev/proof/)

### 2. Atomic CRM — Contact Import Review Extension
**Extending an existing open-source application to prevent data corruption.**
- **Problem:** Standard CSV imports in CRM systems often create duplicates or silently overwrite valid contacts without giving operators a chance to review conflicts.
- **Solution:** Extended Marmelab's open-source **Atomic CRM** (React / TypeScript) with a pre-commit review flow: preview parsed records, classify duplicates/conflicts, and select eligible rows before any write occurs.
- **Verification:** Step-by-step verification protocol and unit tests demonstrating row-by-row decisions on synthetic data.
- **Links:** [Read Case Study](https://github.com/Hadezu/atomic-crm-import-review/blob/main/CASE-STUDY.md) · [Inspect Changes](https://github.com/Hadezu/atomic-crm-import-review/commit/9453b46c52b0610042a1aa48cd2a8e9cf1aa3785) · [Verification Protocol](https://github.com/Hadezu/atomic-crm-import-review/blob/main/docs/import-review-verification.md)

### 3. Catalog Webhook Reliability — FastAPI Extension
**Fault-tolerant API event processing and recovery under network failure.**
- **Problem:** A partner accepts an event, but the HTTP response drops in transit. Naive retries can result in duplicate inventory updates or conflicting entity states.
- **Solution:** Extended the Full Stack FastAPI Template with signed catalog events, a transactional PostgreSQL inbox/outbox pattern, durable idempotency keys, and an operator recovery console.
- **Verification:** Automated CI workflow and runnable Docker Compose environment testing ambiguous network retries, stale arrivals, and worker failovers.
- **Links:** [Inspect Repository](https://github.com/Hadezu/fastapi-webhook-reliability) · [Automated CI Proof](https://github.com/Hadezu/fastapi-webhook-reliability/actions) · [Architecture Docs](https://github.com/Hadezu/fastapi-webhook-reliability/blob/main/docs/ARCHITECTURE.md)

### 4. Reconciliation Evidence Workbench
**Automated data comparison and discrepancy audits for business operations.**
- **Problem:** Discrepancies between billing exports, partner databases, or migration files often get lost in untracked spreadsheets.
- **Solution:** Offline Python/DuckDB tool that compares disparate CSV/XLSX exports, isolates unmatched or conflicting rows, and generates interactive HTML audit reports and review workbooks with cryptographic checksums.
- **Verification:** Executable test suite verifying that no comparison records are silently dropped, producing reproducible checksum outputs.
- **Links:** [Inspect Repository](https://github.com/Hadezu/reconciliation-evidence-workbench) · [PostgreSQL Import Rehearsal](https://github.com/Hadezu/postgres-import-rehearsal)

### 5. TradeBot Research Engine (Showcase)
**Demonstration of system scale, multi-month development, and verification discipline.**
- **Context:** An ongoing private research project exploring market dynamics, risk attribution, and failure-tolerant execution across extended development cycles.
- **Engineering Proof:** Demonstrates managing a complex, multi-component codebase using AI agents over months. Historical private acceptance records document 280 passing verification checks.
- **Verification Boundaries:** The public showcase includes an independent, zero-dependency 7-test runnable demo verifying a synthetic artifact receipt and gating contract. *These 7 public tests demonstrate the gating mechanism only and do not test or validate the private trading system.*
- **Boundary:** Core trading rules and execution remain private. Consistent trading profitability has not been proven.
- **Links:** [View TradeBot Showcase](https://github.com/Hadezu/tradebot-ai-research-showcase) · [Architecture & Case Studies](https://github.com/Hadezu/tradebot-ai-research-showcase/blob/main/docs/architecture.md) · [Independent Demo](https://github.com/Hadezu/tradebot-ai-research-showcase/tree/main/demo)

---

## AI-Driven Development — My Core Advantage

I build working software products with AI coding agents as my primary development tools.

By deliberately orchestrating **ChatGPT**, **Codex**, and **Antigravity**, I bridge the gap between operational objectives and verified, working software:

- **Product Direction & Solution Planning:** I define product goals, articulate technical requirements, and explore solution approaches and trade-offs with ChatGPT.
- **Agentic Implementation:** I direct AI coding tools to generate application logic, boilerplate, database schemas, and automated test harnesses.
- **Evaluation & Decision Making:** I review execution reports, inspect automated test evidence, and evaluate results against business constraints to decide what to advance, iterate, or discard.

**Data Governance & Code Privacy:** AI tool usage, source code access, and confidential data handling rules are explicitly agreed upon before starting any engagement. Depending on project requirements, work is conducted within local-only environments or customer-approved toolchains with defined data boundaries.

---

## Ways to Collaborate

I work in two formats:

- **B2B Contracts:** Developing complete custom applications, long-term technical engagements, or focused integration modules. Every project starts with agreed scope, timeline, budget, and testable acceptance criteria.
- **Remote Roles:** Full-time or contract roles in AI-assisted product development, internal tooling, and automation. Ready to complete a realistic, time-boxed trial task.

### Starting a Discussion
You don't need a formal 30-page specification, an introductory call, or to share sensitive company data to start a conversation:
- Send a brief summary of the problem, workflow, or feature you need.
- Include an interface screenshot (free of sensitive business or personal data), API reference, or a sample file with **synthetic data** (dummy records) or **anonymized data** (scrubbed of confidential information). *Please do not send sensitive or production customer data.*

We can review the requirements, identify edge cases, and define clear acceptance criteria before any commitment.

---

## Contact & Links

- **Email:** [ivan@matiushkin.com](mailto:ivan@matiushkin.com)
- **LinkedIn:** [Ivan Matiushkin](https://www.linkedin.com/in/ivan-matiushkin-809694442/)
- **Interactive Portfolio:** [work.matiushkin.com/en](https://work.matiushkin.com/en) (English) · [work.matiushkin.com](https://work.matiushkin.com/) (Po polsku)
- **Services Overview:** [Internal Applications](https://work.matiushkin.com/en/services/internal-applications)
- **Location:** Poland (Remote / Central European Time)
