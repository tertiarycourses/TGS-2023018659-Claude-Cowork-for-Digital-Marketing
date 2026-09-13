# Activity 12 — Integration regression tests and recovery


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO2; K5 K6 K7 A3 A4


## Goal

Execute a fixture-based regression checklist and diagnose a failing integration without altering raw source evidence.


## What you will produce

regression-evidence.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

test_id, expected, observed, severity, recovery, status


## Mechanism

Expected values act as test oracles. A failure trace links input version, integration rule, observed output and a narrowly scoped recovery action.

A test that merely confirms a file exists misses semantic failures. Use independently calculated totals, row counts, permission checks and excluded-customer fixtures as acceptance evidence.


## Detailed procedure

1. Download or copy the complete activity-12-regression-recovery folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Record T01–T04initial observations before repairs. Two Pass and two Critical Fail imply50%pass rate and release blocked.

5. Replace the incorrect ROAS5.11with independently verified2.40and restore SYN001-only consent eligibility. Rerun all four tests and retain separate initial and corrected evidence tables.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Expected values act as test oracles. A failure trace links input version, integration rule, observed output and a narrowly scoped recovery action. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request regression-evidence.csv in output/. Use the exact fields test_id, expected, observed, severity, recovery, status where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 2 / 4 initial tests pass = 50%; two critical failures block release regardless of appearance. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: A polished report passes visual review but fails aggregation and consent fixtures. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Block release, isolate the smallest failing input, fix the relevant contract and rerun every affected test. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Retain each failure as a permanent regression fixture so later Skill or schema changes cannot reintroduce it. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Release readiness = all critical tests pass AND unresolved defects = 0

2 / 4 initial tests pass = 50%; two critical failures block release regardless of appearance.


## Acceptance checks

- Initial failures are retained in the evidence log.

- Corrected totals give ROAS 2.40 and the segment contains SYN001 only.

- Retest date, version and fixture filenames are recorded.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** A polished report passes visual review but fails aggregation and consent fixtures.

**Recovery:** Block release, isolate the smallest failing input, fix the relevant contract and rerun every affected test.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture