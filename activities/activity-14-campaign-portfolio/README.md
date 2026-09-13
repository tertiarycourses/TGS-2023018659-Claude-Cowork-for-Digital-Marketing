# Activity 14 — Integrated campaign evidence portfolio


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 40 minutes | **Mapping:** LO3; K1 K2 K3 K4 K5 K6 K7 A1 A2 A3 A4 A5


## Goal

Integrate a compatibility plan, tested metrics, draft content and a change proposal into one reviewable marketing evidence portfolio.


## What you will produce

portfolio-manifest.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

deliverable, input_version, rule_version, test, approval, release_state


## Mechanism

A release manifest joins separate marketing artifacts into a coherent integration evidence chain. The portfolio shows compatibility, tests, troubleshooting and a reasoned change proposal.

Evaluate both marketing usefulness and integration correctness. A compelling narrative cannot override failed totals, unsupported claims or missing permission evidence.


## Detailed procedure

1. Download or copy the complete activity-14-campaign-portfolio folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Join the four portfolio deliverables to their input_version,rule_version,test,approval and release_state. Check that each has all required links.

5. Reconcile all draft states,dates and currencies. Write one bounded recommendation with supporting metric evidence and one clear uncertainty statement;keep all external publication disabled.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: A release manifest joins separate marketing artifacts into a coherent integration evidence chain. The portfolio shows compatibility, tests, troubleshooting and a reasoned change proposal. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request portfolio-manifest.csv in output/. Use the exact fields deliverable, input_version, rule_version, test, approval, release_state where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 4 fully linked deliverables / 4 deliverables = 100%; no live campaign publishing is performed. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The final recommendation mixes different dates, currencies and approval states across deliverables. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Reconcile the release manifest, block inconsistent deliverables and request owner review before any real-world action. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Recommend one bounded improvement with owner, risk, test plan and rollback trigger. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Portfolio traceability = deliverables with input + rule + test links / deliverables × 100

4 fully linked deliverables / 4 deliverables = 100%; no live campaign publishing is performed.


## Acceptance checks

- All four deliverables identify inputs, rules, tests and approval states.

- Recommendation distinguishes observed evidence from hypotheses.

- No live send, ad spend, account change or campaign publication occurs.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The final recommendation mixes different dates, currencies and approval states across deliverables.

**Recovery:** Reconcile the release manifest, block inconsistent deliverables and request owner review before any real-world action.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture