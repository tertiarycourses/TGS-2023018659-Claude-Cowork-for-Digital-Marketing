# Activity 13 — Versioning, approval and change control


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 30 minutes | **Mapping:** LO3; K7 A5


## Goal

Propose and evidence an integration-plan change with version identifiers, approval gates and rollback criteria.


## What you will produce

change-proposal.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

version, change, test_evidence, owner, state, rollback


## Mechanism

Input, mapping, Skill and report versions form an evidence bundle. Human approval changes release state; regeneration alone does not authorise external publication.

Track what changed, why, who owns it and what evidence supports acceptance. Propose changes within the selected-component integration plan, matching A5 rather than claiming an enterprise architecture redesign.


## Detailed procedure

1. Download or copy the complete activity-13-version-control folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Compare versions1.0,1.1,1.2and2.0. Identify which areRetired,Candidate,Review andPlanned;do not label Candidate as Approved.

5. Draft a bounded change proposal for one observed defect. Record affected interface,old/new rule,owner,test IDs,rollback trigger and acceptance state. Restore the last accepted mapping if any critical retest fails.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Input, mapping, Skill and report versions form an evidence bundle. Human approval changes release state; regeneration alone does not authorise external publication. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request change-proposal.md in output/. Use the exact fields version, change, test_evidence, owner, state, rollback where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 3 retested rules / 3 affected rules = 100%; approval remains a separate requirement. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: A new Skill overwrites the previous report without recording which inputs or rules changed. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Keep versioned inputs and outputs, record the change rationale and tests, and restore the last accepted version if critical checks fail. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Introduce a versioned release manifest linking source hashes, Skill version, regression results and approver. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Change coverage = affected rules with retests / affected rules × 100

3 retested rules / 3 affected rules = 100%; approval remains a separate requirement.


## Acceptance checks

- Change proposal cites an observed defect and affected interface.

- Version log lists author, date, evidence and approval state.

- Rollback criteria restore an accepted mapping and preserve raw inputs.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** A new Skill overwrites the previous report without recording which inputs or rules changed.

**Recovery:** Keep versioned inputs and outputs, record the change rationale and tests, and restore the last accepted version if critical checks fail.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture