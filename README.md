# Ivan Matiushkin

### Software for business processes that need a better tool.

I build internal applications, connect systems, work with business data and improve existing software. Independent contractor in Poland, working directly with clients remotely.

[Explore the portfolio](https://work.matiushkin.com/en) · [Po polsku](https://work.matiushkin.com/) · [Describe your problem](https://work.matiushkin.com/en/contact)

**You do not need a technical specification or an introductory call.** Describe what happens today and what needs to change. If I sent you an example by email, replying there is enough.

---

## Start with a working example

### 01 / A request needs a clear owner and a recorded decision

**Operations Approval Desk** — submit a request, switch to its reviewer and inspect the decision history. Try an outdated decision: it cannot overwrite the approved version. Real Django/PostgreSQL, with an isolated synthetic workspace.

[Try live — EN](https://operations-approval-desk.onrender.com/demo/en/) · [Wypróbuj — PL](https://operations-approval-desk.onrender.com/demo/pl/) · [Code and verification](https://github.com/Hadezu/operations-approval-desk) · [Internal application development](https://work.matiushkin.com/en/services/internal-applications)

No account needed. The guided demo switches synthetic roles; it does not demonstrate customer identity onboarding. Free hosting may take about a minute to wake up. The repository also includes local authenticated workflows.

### 02 / An existing application needs a safer import

**Atomic CRM import review** — my extension to Marmelab's CRM adds a read-only CSV preview, duplicate/conflict review, explicit row selection and per-record outcomes. Inspect the walkthrough or run the extension locally; Marmelab's hosted demo is the upstream CRM, not my extension.

[Project walkthrough](https://github.com/Hadezu/atomic-crm-import-review/blob/main/CASE-STUDY.md) · [Code and tests](https://github.com/Hadezu/atomic-crm-import-review) · [Improve existing software](https://work.matiushkin.com/en/services/software-improvements)

---

## Selected implementations

Choose the task, then inspect one relevant project. **Live example**, **local implementation**, **offline report** and **code change** are different kinds of evidence.

### Connect systems and recover from failures

- **[FastAPI webhook reliability](https://github.com/Hadezu/fastapi-webhook-reliability)** · Local implementation. PostgreSQL inbox/outbox, duplicate handling and recovery after lost responses or process crashes; an attributed extension to the Full Stack FastAPI Template.
- **[OAuth Connection Recovery](https://github.com/Hadezu/oauth-connection-recovery)** · Local implementation. PKCE, encrypted token storage and explicit reconnection after ambiguous renewal, against a local OAuthLib provider.

[Relevant service: API integration](https://work.matiushkin.com/en/services/api-integration) · [Related interactive example: Data Bridge](https://work.matiushkin.com/en/data-bridge)

### Move data and explain differences

- **[PostgreSQL Import Rehearsal](https://github.com/Hadezu/postgres-import-rehearsal)** · Local implementation + downloadable review. Inspect an import plan, apply it to a real database and try guarded undo after later changes.
- **[Reconciliation Evidence Workbench](https://github.com/Hadezu/reconciliation-evidence-workbench)** · Offline reports. Compare CSV/XLSX files and inspect exact amounts, ambiguous records and portable HTML/Excel evidence.

[Relevant service: migration and reconciliation](https://work.matiushkin.com/en/services/data-migration) · [Related interactive example: Revenue BI](https://work.matiushkin.com/en/proof/revenue-bi)

### Improve existing code and evaluate changes

- **[Resilience4j retry review](https://github.com/Hadezu/resilience4j-retry-review)** · Scoped code change. A reproduced scheduled-retry failure, a bounded Java fix and regression tests against the unchanged upstream baseline.
- **[LLM Extraction Release Gate](https://github.com/Hadezu/llm-extraction-release-gate)** · Offline evaluation evidence. Compare extraction versions and block critical regressions. Recorded real-model failures remain visible; this proves the evaluation tool, not a production-ready extractor.

[Relevant service: improve existing software](https://work.matiushkin.com/en/services/software-improvements) · [Related interactive example: AI workflow lab](https://work.matiushkin.com/en/proof/ai-automation)

### Inspect the interface itself

**[Portfolio source](https://github.com/Hadezu/work-portfolio)** · Reproducible source distribution. React/TypeScript, bilingual interfaces, Three.js and interactive business demonstrations. Read its local/production boundaries; the live website may include later changes than the published source snapshot.

---

## What the evidence means

Independent work with synthetic/test data, **not client deployments**. Upstream authors retain credit and my contributions are explicitly identified. No client ROI, vendor certification, production-scale reliability or real-employee adoption is implied. OAuth uses a local provider; approvals do not execute external operations; the AI gate does not establish model quality.

## How we start

Describe the process or existing software problem. I review fit and unknowns, then propose a practical next step. Scope, access, acceptance criteria, price and timing are agreed before paid work. A first stage is a way to start, not a limit on project size; detailed design and prototyping are separately scoped.

I use Codex to assist development and verify the results through code review, builds, tests and browser checks. AI-tool and data-access constraints are agreed before working with client code.

[Describe your problem](https://work.matiushkin.com/en/contact) · [ivan@matiushkin.com](mailto:ivan@matiushkin.com)

Independent contractor · Poland / remote collaboration. Contracts and payments can be handled through Useme where compatible with the client; Useme is an intermediary, not my company.
