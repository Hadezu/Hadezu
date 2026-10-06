# Ivan Matiushkin

**Custom software, internal applications and improvements to existing systems.**

Independent developer in Poland, working remotely. Bring a manual process, a missing tool or a problem in existing software. I assess the task, agree a practical first stage and deliver changes with tests and handover instructions. Larger projects can grow through agreed stages.

[Portfolio](https://work.matiushkin.com/en) · [Portfolio po polsku](https://work.matiushkin.com/) · [Describe your task](mailto:ivan@matiushkin.com)

## Watch a working example

Choose the task closest to yours. These links open a recorded demonstration inside the repository README; no installation is needed to watch.

| What you need | Start here |
| --- | --- |
| An internal application | [Approval workflow](https://github.com/Hadezu/operations-approval-desk#watch-the-demonstration) |
| A dependable API integration | [Webhook recovery](https://github.com/Hadezu/fastapi-webhook-reliability#watch-the-demonstration) |
| A controlled database import | [PostgreSQL import rehearsal](https://github.com/Hadezu/postgres-import-rehearsal#watch-the-demonstration) |
| An explanation of reporting differences | [CSV/XLSX reconciliation](https://github.com/Hadezu/reconciliation-evidence-workbench#watch-the-demonstration) |

## Find evidence for your task

| Your task | Working evidence | What to inspect |
| --- | --- | --- |
| Build an internal application | [Operations Approval Desk](https://github.com/Hadezu/operations-approval-desk) | Django/PostgreSQL, real login, scoped records, approval conflicts and history |
| Extend an existing application | [Atomic CRM import review](https://github.com/Hadezu/atomic-crm-import-review/blob/main/CASE-STUDY.md) | My extension to Marmelab's CRM: preview, conflicts and selective contact import |
| Fix existing backend code | [Java retry failure](https://github.com/Hadezu/resilience4j-retry-review) | A scoped Resilience4j patch with reproduction and regression tests |
| Connect systems and recover failed deliveries | [FastAPI webhook reliability](https://github.com/Hadezu/fastapi-webhook-reliability) | Extension to the upstream template: PostgreSQL inbox/outbox, duplicates, lost responses and process crashes |
| Handle connected-account authorization | [OAuth Connection Recovery](https://github.com/Hadezu/oauth-connection-recovery) | PKCE, encrypted tokens and reconnection after ambiguous renewal against a local provider |
| Import into an existing database | [PostgreSQL Import Rehearsal](https://github.com/Hadezu/postgres-import-rehearsal) | Reviewed plans, real database writes, replay protection and guarded undo |
| Reconcile files and explain reporting differences | [Reconciliation Evidence Workbench](https://github.com/Hadezu/reconciliation-evidence-workbench) | CSV/XLSX, exact amounts, ambiguous records and portable HTML/Excel evidence |
| Evaluate AI workflow changes | [LLM Extraction Release Gate](https://github.com/Hadezu/llm-extraction-release-gate) | Per-case regressions and release decisions; raw real-model failures remain visible |
| Build a web interface or interactive component | [Portfolio source](https://github.com/Hadezu/work-portfolio) · [Live examples](https://work.matiushkin.com/en) | React/TypeScript, bilingual interface, Three.js and interactive business demonstrations |

Each project includes scope, setup and verification information. These are **independent implementations with synthetic/test data, not paid client deployments**. Upstream authors retain credit; my extensions and fixes are identified explicitly. Repository evidence supports the mechanisms implemented, not every requirement of a larger role.

## Starting a project

You do not need to know the technology in advance. Describe what happens now, what should change and who will use the result. No introductory call or finished specification is required.

A first stage could be a usable workflow, a feature in your application, a reproducible bug fix, an integration or a data-processing task. It is a starting point, not a limit on project size. We agree access, scope, acceptance criteria, price and timing before paid work. Detailed architecture and prototypes are separately scoped.

## How I work with AI

I use Codex to help explore codebases, implement changes and develop tests. I review changes and check results through appropriate builds, automated checks and browser testing. AI-tool and data-access constraints are agreed before working with client code. AI assistance is not itself evidence that a result is correct.

## Evidence boundaries

- The CRM and FastAPI applications build on attributed open-source projects; I did not author their entire upstream feature sets.
- OAuth uses a local test provider, not an approved Google/Meta connector. Webhook guarantees depend on the documented partner contract.
- The approval app uses real authentication with synthetic accounts; it does not perform external financial or warehouse actions.
- The AI release gate demonstrates evaluation. Its recorded Qwen candidate was blocked, not declared production-ready.
- No client references, vendor certifications, production-scale reliability or experience with every framework are implied.

**Have a task that does not fit the examples?** [Describe it](mailto:ivan@matiushkin.com). I will assess the fit and what needs to be clarified.

Independent contractor · Poland / remote collaboration  
Contracts and payments can be handled through Useme where compatible with the client; Useme is an intermediary, not my company.  
[work.matiushkin.com](https://work.matiushkin.com)
