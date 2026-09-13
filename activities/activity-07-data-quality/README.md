# Activity 07 — Marketing data quality and error diagnosis


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO2; K4 K5 K6 K7 A3 A4


## Goal

Diagnose deliberate schema, duplicate, currency and date defects in a dirty campaign export.


## What you will produce

validation-errors.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

row_id, defect, raw_value, expected_rule, action, status


## Mechanism

Schema validation detects structural errors; semantic checks detect impossible or incompatible values. A correction copy and a retest trace preserve the evidence chain.

Use a minimal failing row to isolate the problem. Distinguish permission failures, file-read failures, field mismatches and valid-looking metric inconsistencies before changing the integration plan.


## Detailed procedure

1. Download or copy the complete activity-07-data-quality folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Read the defect ledger row by row. Distinguish the currency source correction from the duplicate correction and missing-value flag.

5. Create separate raw_value,correction,evidence,status fields. R02andR07 remain Open until corrected source evidence exists;R04isFixed only with duplicate evidence;R09remains missing,N/A.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Schema validation detects structural errors; semantic checks detect impossible or incompatible values. A correction copy and a retest trace preserve the evidence chain. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request validation-errors.csv in output/. Use the exact fields row_id, defect, raw_value, expected_rule, action, status where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 4 defective rows / 12 checked rows = 33.33%; two source corrections remain open. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The agent silently fills missing orders with the median and makes CPA look precise. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Restore the missing state, label affected calculations N/A and document whether a source correction is required. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Add pre-analysis validation and preserve a regression fixture for each repaired defect. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Defect rate = defective rows / checked rows × 100

4 defective rows / 12 checked rows = 33.33%; two source corrections remain open.


## Acceptance checks

- Each deliberate defect has a row-level error log.

- Raw export is unchanged.

- Retest evidence distinguishes repaired, quarantined and unresolved defects.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The agent silently fills missing orders with the median and makes CPA look precise.

**Recovery:** Restore the missing state, label affected calculations N/A and document whether a source correction is required.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture