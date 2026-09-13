# Activity 10 — Social content repurposing and asset QA


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 30 minutes | **Mapping:** LO2; K4 K5 K6 A3 A4


## Goal

Repurpose an approved campaign brief into three channel drafts with asset, claim and accessibility checks.


## What you will produce

asset-manifest.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

asset_id, channel, format, claim_ids, alt_text, status


## Mechanism

One approved source brief feeds channel-specific output contracts. A manifest joins copy, visual assets, claim provenance, accessibility and approval state.

Supplied SVG concepts are original synthetic training assets. They are not final commercial creative, real platform screenshots or evidence of live publication.


## Detailed procedure

1. Download or copy the complete activity-10-social-assets folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Open assets/bottle-concept.svg and any supplied imagegen image. Record the visual colour/cap as concept attributes rather than verified SKU facts.

5. Produce oneInstagram,oneLinkedIn and oneemail draft. Build an asset manifest with asset_id,channel,format,claim_ids,alt_text,status;reject A04and write meaningful alt text for every accepted draft.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: One approved source brief feeds channel-specific output contracts. A manifest joins copy, visual assets, claim provenance, accessibility and approval state. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request asset-manifest.csv in output/. Use the exact fields asset_id, channel, format, claim_ids, alt_text, status where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 17 valid fields / 18 required = 94.44%; the missing alt text blocks acceptance. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: An attractive variant uses an unapproved environmental claim and an image without meaningful alt text. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Replace the claim with ledger-backed facts and write descriptive alt text before moving the asset into review. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Regenerate only affected variants when an approved claim or price changes. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Asset completeness = valid required manifest fields / total required fields × 100

17 valid fields / 18 required = 94.44%; the missing alt text blocks acceptance.


## Acceptance checks

- Three drafts match their declared channel contracts.

- Every factual claim uses valid claim IDs.

- Each asset has descriptive alt text and a human review state.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** An attractive variant uses an unapproved environmental claim and an image without meaningful alt text.

**Recovery:** Replace the claim with ledger-backed facts and write descriptive alt text before moving the asset into review.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture