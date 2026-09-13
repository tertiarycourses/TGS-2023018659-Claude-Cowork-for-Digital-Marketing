# Activity 02 — Brand context and grounded campaign brief


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 30 minutes | **Mapping:** LO1; K1 K2 K3 A1 A2


## Goal

Build a source-grounded campaign brief for a synthetic Singapore reusable-bottle brand without fabricating claims.


## What you will produce

campaign-brief.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

claim_id, approved_claim, source_file, source_section, approval, expiry


## Mechanism

A claim ledger binds each generated fact to an approved source and approval state. Instructions govern style; source files govern factual truth.

Separate source facts from creative hypotheses. Mark persona assumptions as hypotheses, maintain expiry dates, and preserve an approval record before external publication.


## Detailed procedure

1. Download or copy the complete activity-02-brand-context folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Create a claims table from assets/claim-ledger.csv. Search every draft factual sentence for price, capacity, delivery and environmental assertions.

5. Keep C01,C02,C03;reject C99. Mark persona and campaign-positioning ideas as hypotheses. Independently compare every approved price and threshold with assets/brand-source.md.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: A claim ledger binds each generated fact to an approved source and approval state. Instructions govern style; source files govern factual truth. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request campaign-brief.md in output/. Use the exact fields claim_id, approved_claim, source_file, source_section, approval, expiry where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 9 sourced claims / 10 factual claims = 90%; remove the unsupported claim to reach 100%. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The draft transforms “stainless steel” into “clinically proven healthier”. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Remove the unsupported health claim and trace every factual phrase to an approved source. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Version the claim ledger when price or delivery policy changes; regenerate affected campaign variants. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Grounding coverage = sourced factual claims / total factual claims × 100

9 sourced claims / 10 factual claims = 90%; remove the unsupported claim to reach 100%.


## Acceptance checks

- Every factual claim has file and section provenance.

- Unsupported C04 never appears in the final draft.

- The output preserves SGD 32 and the SGD 60 delivery threshold.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The draft transforms “stainless steel” into “clinically proven healthier”.

**Recovery:** Remove the unsupported health claim and trace every factual phrase to an approved source.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture