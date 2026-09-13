# Activity 03 — Connector and MCP compatibility design


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO1; K2 K3 K4 K5 A1 A2


## Goal

Design a read-only connector integration and inspect supplied MCP-style teaching traces without connecting a live account.


## What you will produce

connector-integration-plan.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

source, transport, auth_owner, allowed_action, returned_fields, gate


## Mechanism

MCP separates the client from a server exposing tools and resources. A connector adds account-specific authorization; possession of a connection does not imply every property is accessible.

Inspect server documentation and administrator controls for the actual connector. Sample trace names in this activity are explicitly synthetic and are not commands to call a vendor service.


## Detailed procedure

1. Download or copy the complete activity-03-mcp-compatibility folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Read input/mock-data.csv and connector-trace.json. Identify client, server, source account, allowed action and returned fields. Label the trace synthetic.

5. For an optional authorised sandbox only: confirm administrator-approved account, property and read scope using the current connector documentation. Cancel if a requested write scope exceeds the plan. Otherwise use the supplied local export and record fallback.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: MCP separates the client from a server exposing tools and resources. A connector adds account-specific authorization; possession of a connection does not imply every property is accessible. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request connector-integration-plan.md in output/. Use the exact fields source, transport, auth_owner, allowed_action, returned_fields, gate where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 4 matched / 5 source campaign IDs = 80%; one missing ID is a compatibility error. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: A connector lists reporting tools but the source account grants no access to the required property. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Check account identity, permitted property and read scope; obtain administrator correction before retrying. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Replace a missing connector with a schema-compatible local export while documenting the reduced automation. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Join coverage = matched campaign IDs / source campaign IDs × 100

4 matched / 5 source campaign IDs = 80%; one missing ID is a compatibility error.


## Acceptance checks

- Interface plan identifies owner, transport and access boundary.

- Read actions are separated from send/publish actions.

- Missing campaign_id is logged rather than silently discarded.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** A connector lists reporting tools but the source account grants no access to the required property.

**Recovery:** Check account identity, permitted property and read scope; obtain administrator correction before retrying.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture