# Visual evidence and provenance

Reviewed 23 October 2026. Screenshots are unretouched application captures; diagrams summarize inspected implementation and records.

| Asset | Source and method | Evidence scope |
|---|---|---|
| operations-register.png | Live Operations Desk, captured through browser screenshot API on 23 October 2026 | Synthetic isolated demo register |
| operations-create.png | Same session; equipment request titled Customer support workstation | Filled creation form before saving |
| operations-review.png | Same request, submitted as employee and reviewed as manager | Decision comment before approval |
| operations-decision.png | Same request after approval | Approved state and three activity entries |
| crm-import-review.png | Unchanged copy of Atomic CRM extension docs/images/contact-review.png; recorded October 2026 FakeRest demonstration | Real extension preview with synthetic contacts; not an upstream-only screenshot |
| tradebot-scale.svg | Identical copy of TradeBot showcase assets/engineering-scale.svg | Documented protocol and saved 20 October 2026 private acceptance |
| fastapi-delivery.svg | FastAPI extension README and docs/VERIFICATION.md | Inbox/outbox, leases and synthetic partner receipt contract |
| delivery-process.svg | Proposed collaboration in delivery-method.md | Proposed process, rather than a claim of completed client engagements |

The served Operations Desk build revision was not exposed in the captured workflow; it is not inferred from an older release record. Screenshots establish the observed UI on the capture date. Release test counts come from the separately linked release evidence. The Atomic image's exact capture revision was not independently established; the verification document records its upstream baseline and subsequent browser checks.

TradeBot metric meanings and historical/private scope are specified in its [engineering evidence record](https://github.com/Hadezu/tradebot-ai-research-showcase/blob/main/docs/engineering-scale.md). Counts are not profitability or production uptime measures.

All SVG assets use explicit backgrounds, system fonts and embedded vector shapes, with no external resources. The original product interfaces retain their own visual identities. The editorial diagrams use navy, teal and white to distinguish system structure from application evidence.
