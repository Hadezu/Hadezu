# Working software, visible workflows

[Back to portfolio](../README.md) · [Discuss your workflow](mailto:ivan@matiushkin.com)

## Operations Desk

**For a company that needs requests, accountable decisions and a searchable record.** The running demonstration follows the same request from employee to manager. All shown data is synthetic.

### Create the request
![Employee enters a synthetic equipment request with an amount and business reason](../assets/operations-create.png)

### Review with a reason
![Manager reviews the submitted request and enters a decision comment](../assets/operations-review.png)

### Keep the decision and its history together
![Approved request with the manager comment and created, submitted and approved activity entries](../assets/operations-decision.png)

[Try the workflow](https://operations-desk-reliability.vanya-matyushkin.workers.dev/) · [Release verification](https://github.com/Hadezu/operations-desk-reliability/blob/main/docs/RELEASE.md)

## Atomic CRM

**For a team that wants to inspect imported contacts before creating them.** The extension adds CSV preview, duplicate classification and explicit row selection to Marmelab's Atomic CRM.

CSV → preview → duplicate review → selected records → per-record result.

![Actual Atomic CRM extension: six reviewed records, duplicate and invalid classifications, two rows selected before creation](../assets/crm-import-review.png)

The image shows the preview stage. The complete creation and repeat-import journey is documented in the [browser verification](https://github.com/Hadezu/atomic-crm-import-review/blob/main/docs/import-review-verification.md). This is the extension's recorded FakeRest demonstration.

## FastAPI delivery

**For a company connecting systems where an interrupted request must remain investigable.** The extension uses a persistent delivery record and a receipt-aware synthetic partner.

![Event reception, durable persistence, leased processing and confirmation, with duplicate, lost-response and worker-stop paths](../assets/fastapi-delivery.svg)

[Implementation and setup](https://github.com/Hadezu/fastapi-webhook-reliability) · [Verification](https://github.com/Hadezu/fastapi-webhook-reliability/blob/main/docs/VERIFICATION.md)

## Apply a similar pattern to your business

Approval portals, controlled imports and recoverable integrations can be combined or developed as standalone products. Describe the people, systems and outcome involved; scope and acceptance follow from that workflow.

[Discuss a project](mailto:ivan@matiushkin.com) · [Image provenance](visual-evidence.md)
