# Activity 11 — Experiment design and performance evidence


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO2; K4 K5 K6 K7 A3 A4


## Goal

Evaluate synthetic landing-page variants while controlling denominator choice and avoiding causal overclaims.


## What you will produce

experiment-evidence.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

variant, visitors, orders, conversion_rate, revenue_sgd, decision


## Mechanism

An experiment contract defines assignment, exposure, primary metric and stopping rules before examining outcomes. A metric change alone does not establish causality.

Seasonality, allocation imbalance, repeat visitors and multiple comparisons can explain apparent improvements. Keep the decision proportionate to the evidence and record the next verification requirement.


## Detailed procedure

1. Download or copy the complete activity-11-experiment-design folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Use the two A/B rows;do not include the Difference summary as a third variant. Calculate40/1000and50/1000.

5. Write both absolute difference1percentage point and relative lift25%. Inspect whether random assignment,exposure parity and uncertainty evidence exist;where absent explicitly withhold causal and significance claims.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: An experiment contract defines assignment, exposure, primary metric and stopping rules before examining outcomes. A metric change alone does not establish causality. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request experiment-evidence.md in output/. Use the exact fields variant, visitors, orders, conversion_rate, revenue_sgd, decision where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: A = 40 / 1000 = 4%; B = 50 / 1000 = 5%; relative lift = 25%, absolute difference = 1 percentage point. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The report states “B causes 25% more sales” from observational counts without randomisation evidence. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Report observed relative lift, identify allocation and uncertainty limits, and recommend a controlled follow-up. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Add allocation and exposure diagnostics to the integration plan before making an automated budget recommendation. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

CVR = orders / visitors; relative lift = (CVR_B − CVR_A) / CVR_A

A = 40 / 1000 = 4%; B = 50 / 1000 = 5%; relative lift = 25%, absolute difference = 1 percentage point.


## Acceptance checks

- Absolute percentage-point difference and relative lift are distinguished.

- Visitors, not clicks or impressions, are the declared denominator.

- No statistical significance claim is made without a valid analysis.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The report states “B causes 25% more sales” from observational counts without randomisation evidence.

**Recovery:** Report observed relative lift, identify allocation and uncertainty limits, and recommend a controlled follow-up.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture