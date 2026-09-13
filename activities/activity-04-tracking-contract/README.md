# Activity 04 — Campaign taxonomy and tracking contract


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 30 minutes | **Mapping:** LO1; K2 K3 K4 K5 A1 A2


## Goal

Standardise UTM and campaign identifiers across paid social, search and email exports.


## What you will produce

tracking-contract.csv; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

campaign_id, utm_source, utm_medium, utm_campaign, currency, timezone


## Mechanism

A shared identifier connects platform exports without treating channel labels as reliable keys. Normalisation maps display values into a controlled vocabulary while preserving raw evidence.

Teach the legacy GTM coverage floor through data-layer event contracts, event names and UTM fields. Cowork analyses exported tracking evidence; this course does not claim Cowork automatically installs a website tag.


## Detailed procedure

1. Download or copy the complete activity-04-tracking-contract folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Create output/normalisation-map.csv with raw_value,canonical_value,reason. Map Instagram to instagram,paid social to paid_social and Bottle Launch to bottle_launch.

5. Build campaign-date-channel composite keys in a spreadsheet. Count duplicate keys before and after correction; never deduplicate solely by display name. Preserve raw columns beside normalised columns.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: A shared identifier connects platform exports without treating channel labels as reliable keys. Normalisation maps display values into a controlled vocabulary while preserving raw evidence. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request tracking-contract.csv in output/. Use the exact fields campaign_id, utm_source, utm_medium, utm_campaign, currency, timezone where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 2 duplicates / 20 rows × 100 = 10%; campaign-date-channel grain must be unique. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: “Instagram” and “instagram” split the same source into two reporting categories. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Apply a documented lowercase mapping, preserve raw values, then retest category and key counts. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Add a mapping table for new channels rather than changing historical campaign keys. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Duplicate key rate = duplicate primary-key rows / total rows × 100

2 duplicates / 20 rows × 100 = 10%; campaign-date-channel grain must be unique.


## Acceptance checks

- Normalised UTM fields use the approved taxonomy.

- Raw values remain available for audit.

- No duplicate campaign-date-channel key survives the accepted output.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** “Instagram” and “instagram” split the same source into two reporting categories.

**Recovery:** Apply a documented lowercase mapping, preserve raw values, then retest category and key counts.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture