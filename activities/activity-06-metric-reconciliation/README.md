# Activity 06 — Paid campaign metric reconciliation


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO2; K4 K5 K6 A3 A4


## Goal

Reconcile spend, clicks, orders and revenue before comparing channels and recommending budget changes.


## What you will produce

reconciled-metrics.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

channel, spend_sgd, clicks, orders, revenue_sgd, roas


## Mechanism

Aggregation occurs at a declared grain; ratios are recomputed from summed numerators and denominators. Attribution is a reporting model and does not prove causal lift.

Check attribution window, reporting period, timezone and whether revenue includes refunds or tax. Different platform definitions can produce compatible file formats but incompatible business metrics.


## Detailed procedure

1. Download or copy the complete activity-06-metric-reconciliation folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Use Search,Social and Email rows only;exclude the Total row from resumming. Sum spend1200+900+150=2250,revenue2400+1200+1800=5400 and orders40+20+30=90.

5. Calculate each channel CPA and ROAS. Recompute portfolio ROAS5400/2250=2.40 and portfolio CPA2250/90=25.00. Contrast the incorrect mean(2+1.3333+12)/3≈5.1111.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Aggregation occurs at a declared grain; ratios are recomputed from summed numerators and denominators. Attribution is a reporting model and does not prove causal lift. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request reconciled-metrics.csv in output/. Use the exact fields channel, spend_sgd, clicks, orders, revenue_sgd, roas where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: Search ROAS = 2400 / 1200 = 2.00; CPA = 1200 / 40 = SGD 30.00. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The report averages channel ROAS values and produces 5.11 instead of the correct portfolio ROAS 2.40. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Calculate portfolio ROAS from total revenue divided by total spend, then reconcile all channel sums. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Record the revenue definition and attribution window in the output metadata. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

ROAS = attributed revenue / advertising spend; CPA = spend / orders

Search ROAS = 2400 / 1200 = 2.00; CPA = 1200 / 40 = SGD 30.00.


## Acceptance checks

- Total spend is SGD 2,250 and attributed revenue SGD 5,400.

- Portfolio ROAS is 2.40 rather than an unweighted average.

- Zero-order campaigns display CPA as N/A, never zero.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The report averages channel ROAS values and produces 5.11 instead of the correct portfolio ROAS 2.40.

**Recovery:** Calculate portfolio ROAS from total revenue divided by total spend, then reconcile all channel sums.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture