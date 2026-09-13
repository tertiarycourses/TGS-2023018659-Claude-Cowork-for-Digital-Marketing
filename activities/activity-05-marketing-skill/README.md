# Activity 05 — Reusable marketing Skill contract


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO1; K2 K3 K4 K5 A1 A2


## Goal

Author a portable campaign-analysis Skill package with a SKILL.md and reference files, then validate its instructions against fixtures.


## What you will produce

skills/campaign-analysis/SKILL.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

test_id, fixture, rule, expected, observed, result


## Mechanism

A Skill is a directory of instructions and optional resources. Its name and description support discovery; its detailed instructions encode a repeatable marketing procedure.

The supplied package is a learner-authored portable example. Cowork packaging and import controls may differ by enabled product surface; use current official instructions and validate the actual available workflow.


## Detailed procedure

1. Download or copy the complete activity-05-marketing-skill folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Read skills/campaign-analysis/SKILL.md. Confirm YAML opening and closing---lines and nonempty name/description. Inspect every reference for credentials or changing facts.

5. Run the four supplied S01–S04fixtures manually against the instruction contract. Missing spend must be flagged;zero conversions yield N/A;USD blocks SGD-only analysis;unsupported claims are rejected. Run python3 -m zipfile -c campaign-analysis.zip skills/campaign-analysis from this activity folder;inspect ZIP contains campaign-analysis/SKILL.md and references/. Use Customize > Skills > + > + Create skill > upload if enabled. If admin disables import,attach instructions as a labelled fallback;do not claim installed execution.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: A Skill is a directory of instructions and optional resources. Its name and description support discovery; its detailed instructions encode a repeatable marketing procedure. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and author skills/campaign-analysis/SKILL.md with YAML name and description metadata plus instructions for inputs,outputs,rules and references. Record test_id,fixture,rule,expected,observed,result in a separate fixture-evidence.csv;these are not Skill frontmatter fields.

10. Independently check the worked example: 4 passes / 4 fixtures = 100%; this tests the package contract, not vendor execution availability. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: A reused Skill embeds last month’s price in its instructions and ignores the current source file. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Move changeable facts into reference inputs and require the Skill to read the current approved ledger. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Bump the Skill version when metric logic changes and rerun all fixtures. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Regression pass rate = passed fixtures / executed fixtures × 100

4 passes / 4 fixtures = 100%; this tests the package contract, not vendor execution availability.


## Acceptance checks

- SKILL.md has name and description metadata.

- Rules declare input/output contracts, missing-data handling and approval boundaries.

- Four fixtures pass before the Skill is offered for reuse.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** A reused Skill embeds last month’s price in its instructions and ignores the current source file.

**Recovery:** Move changeable facts into reference inputs and require the Skill to read the current approved ledger.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture