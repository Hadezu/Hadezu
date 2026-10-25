# Software capabilities and engineering evidence

[Back to profile](../README.md) · [Portfolio](https://work.matiushkin.com/en) · [Discuss requirements](https://work.matiushkin.com/en/contact)

Find the implementation closest to your requirement, inspect its results and use the evidence to define the next project. This index supports technical discussions, RFP/RFQ responses and supplier reviews.

Reviewed on **23 October 2026**. Links connect capabilities to source, execution records and documented scope. Dates refer to the original recorded checks. Repository workflows provide repeatable verification; temporary CI artifacts may expire.

## Match a requirement to a concrete example

| Customer task | Relevant project and implemented capability | Evidence to inspect | Boundary |
|---|---|---|---|
| Internal application with roles and organization separation | [Operations Desk](https://github.com/Hadezu/operations-desk-reliability): Next.js/TypeScript UI, shared authorization, PostgreSQL transactions, audit and concurrent decisions | [Live approvals](https://operations-desk-reliability.vanya-matyushkin.workers.dev/), [proof page](https://operations-desk-reliability.vanya-matyushkin.workers.dev/proof/), [release record](https://github.com/Hadezu/operations-desk-reliability/blob/main/docs/RELEASE.md), 7 Oct 2026 | Synthetic roles. Static Next.js export; no SSR/OIDC or PostgreSQL RLS claim. |
| Background work that can recover after interruption | [Operations Desk](https://github.com/Hadezu/operations-desk-reliability): Fastify/Prisma, transactional outbox, Redis/BullMQ, failed-job replay | Docker setup and worker recovery suite linked in README; release records five recovery scenarios | Worker is local/CI, not hosted in the public demo. Tested idempotency is not universal exactly-once delivery. |
| Review queue with preserved decisions | [Operations Approval Desk](https://github.com/Hadezu/operations-approval-desk): Django/PostgreSQL, exact-version decisions, scoped accounts and evidence export | [Guided EN demo](https://operations-approval-desk.onrender.com/demo/en/), [PL demo](https://operations-approval-desk.onrender.com/demo/pl/), [verification](https://github.com/Hadezu/operations-approval-desk/blob/main/docs/VERIFICATION.md), 5 Oct 2026 | Separate from the TypeScript Operations Desk. Hosted synthetic role switching; free hosting may wake slowly. Approval does not execute an external operation. |
| Add a safer import to existing software | [Atomic CRM extension](https://github.com/Hadezu/atomic-crm-import-review): React/TypeScript CSV preview, duplicate/conflict classification and selected-row creation | [Case study](https://github.com/Hadezu/atomic-crm-import-review/blob/main/CASE-STUDY.md), [verification](https://github.com/Hadezu/atomic-crm-import-review/blob/main/docs/import-review-verification.md), 4–6 Oct 2026 | Marmelab owns the upstream CRM. Local FakeRest example; no live Supabase proof or global multi-user uniqueness guarantee. Wider historical upstream suite had unrelated failures. |
| Connect systems despite duplicate or lost messages | [FastAPI extension](https://github.com/Hadezu/fastapi-webhook-reliability): signed events, PostgreSQL inbox/outbox, leases, retries and controlled replay | [Verification](https://github.com/Hadezu/fastapi-webhook-reliability/blob/main/docs/VERIFICATION.md), 5–6 Oct 2026; real database/HTTP tests and Compose instructions | Extends the Full Stack FastAPI Template. Synthetic partner must implement the stated receipt contract. No vendor certification or SLA. |
| Explain discrepancies between exports | [Reconciliation Workbench](https://github.com/Hadezu/reconciliation-evidence-workbench): Python/DuckDB comparison of mapped CSV/XLSX, ambiguous groups, HTML/Excel review | [Verification](https://github.com/Hadezu/reconciliation-evidence-workbench/blob/main/docs/VERIFICATION.md), [offline evidence release](https://github.com/Hadezu/reconciliation-evidence-workbench/releases/tag/v0.1.0) | Synthetic examples; not a financial audit. Mappings, currencies and matching rules must fit the actual data. |
| Review and apply a database import | [PostgreSQL Import Rehearsal](https://github.com/Hadezu/postgres-import-rehearsal): reviewed plan, transactional apply, repeat-safe receipts, guarded undo | [Verification](https://github.com/Hadezu/postgres-import-rehearsal/blob/main/docs/verification.md), Docker demo and database snapshots | Extends the Chinook schema. Bounded importer, not proof of a production migration or universally safe rollback. |
| Recover an authorization connection | [OAuth Connection Recovery](https://github.com/Hadezu/oauth-connection-recovery): PKCE, encrypted token storage, renewal ownership and reconnection | [Verification](https://github.com/Hadezu/oauth-connection-recovery/blob/main/docs/VERIFICATION.md), local provider demo and captured report | Real local OAuthLib provider with synthetic accounts, not a certified connector to a named vendor. |
| Evaluate an AI extraction change | [LLM Extraction Release Gate](https://github.com/Hadezu/llm-extraction-release-gate): per-case comparison, evidence and critical-regression veto | [Verification](https://github.com/Hadezu/llm-extraction-release-gate/blob/main/docs/VERIFICATION.md), published control and real-model outputs | Recorded real-model candidate failed acceptance. Demonstrates the evaluation tool, not a production-ready extractor. |
| Repair a bounded defect in an existing codebase | [Resilience4j retry review](https://github.com/Hadezu/resilience4j-retry-review): Java scheduled-retry failure fix with regressions | [Verification](https://github.com/Hadezu/resilience4j-retry-review/blob/main/docs/verification-20261005.md), baseline and patched CI comparison | Attributed independent extension of Resilience4j; not an accepted upstream release or proof of broad Java delivery experience. |
| Develop a complex research product over iterations | [TradeBot showcase](https://github.com/Hadezu/tradebot-ai-research-showcase): connected research, compatibility, model admission and recoverable artifacts | [Capability register](https://github.com/Hadezu/tradebot-ai-research-showcase/blob/main/docs/implemented-capabilities.md), [cases](https://github.com/Hadezu/tradebot-ai-research-showcase/blob/main/docs/engineering-case-studies.md), [verification](https://github.com/Hadezu/tradebot-ai-research-showcase/blob/main/docs/verification.md), standalone synthetic demo | Private source. Recorded 20 Oct 2026 acceptance: 280 passed, 2 skipped, not publicly reproducible. Seven public demo tests do not validate the private platform. Profitability unproven. |
| Interactive web interface | [Portfolio source](https://github.com/Hadezu/work-portfolio): bilingual React/TypeScript interface, Three.js and business demonstrations | [Website](https://work.matiushkin.com/en), source README and local setup | Published source snapshot may lag the website. Synthetic examples; local contact delivery and live inference disabled. |

TradeBot's documented research protocol covers 9 markets and 21 native strategies. These describe research scope, not successful markets, validated strategies or customer deployments. Its source and private acceptance were inspected during the 20 October showcase review; they were not rerun or newly certified for this index.

## Proposed workflow expansion (25 October 2026)

| Customer task | Demonstration | What to inspect | What remains project-specific | First paid stage |
|---|---|---|---|---|
| Association membership and dues | [Association Operations](https://github.com/Hadezu/operations-desk-reliability/blob/codex/commercial-operations-expansion/docs/ASSOCIATION.md) | DE/PL import review, preserved revisions, payment allocation and automated checks | Identity onboarding, accounting rules, live bank/DATEV integration | One member export and billing period |
| Limited-resource bookings | [Booking & Payment Reliability](https://github.com/Hadezu/operations-desk-reliability/blob/codex/commercial-operations-expansion/docs/BOOKING.md) | Concurrent holds, duplicate/out-of-order simulator events, cancel/refund and API restart | Real provider, taxes/pricing, shared inventory scale | One resource type and provider sandbox contract |
| Application handover and restore | [Delivery & Recovery Evidence](https://github.com/Hadezu/operations-desk-reliability/blob/codex/commercial-operations-expansion/docs/DELIVERY-RECOVERY.md) | Reproducible setup, actual logical restore and failed-migration rollback | Off-host backups, production recovery targets and support agreement | Test environment and restore rehearsal |

These are feature-branch additions pending owner review, with local runnable demonstrations. No production or commercial client deployment is claimed. Existing profile PR #11 remains independent; this section does not change its proposed introduction.

## Build a requirement-to-acceptance plan

For each actual requirement, identify the relevant example, the tested revision/date and what still needs project-specific implementation or validation. Avoid converting a similar demo into a claim that the customer's requirement is already met.

A practical response can record:

| Requirement | Existing evidence | Proposed deliverable and acceptance | Remaining dependency |
|---|---|---|---|
| Example: repeated input must not create a second record | Webhook duplicate-processing tests | Implement against the client's documented API; agree repeat, conflict and lost-response tests | Destination API semantics and sandbox access |

This is an illustrative response structure, not a bid, quote or contractual promise.

## Acceptance and handover to agree

Before implementation, agree the data/API contract, roles, environments, failure behavior and observable results. Record changed requirements and their cost/time impact before expanding scope. AI tools, code access and sensitive-data handling require explicit agreement.

The proposed handover can include source and third-party notices, setup/migration instructions, example configuration without secrets, test commands and results tied to a revision, deployment responsibilities, and known limitations. Select the actual deliverables in the contract. Support scope, response times and warranties are not implied by a portfolio example.

## Evidence scope and procurement documents

The projects are independent implementations and attributed open-source extensions with synthetic/test examples. TradeBot adds a private research case with a separately runnable public example. Recorded checks establish the behaviors and environments stated in each project. Customer references, contractual delivery history, production service commitments and formal qualification documents are assessed separately for each procurement procedure; they are not evidenced by this portfolio.

For a first discussion, send the problem or requirement list to [ivan@matiushkin.com](mailto:ivan@matiushkin.com). Use synthetic or properly anonymized samples. A formal specification is not required to begin.
