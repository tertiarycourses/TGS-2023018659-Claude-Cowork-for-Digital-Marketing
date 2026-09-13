# Activity 08 — SEO content brief and evidence audit


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 30 minutes | **Mapping:** LO2; K4 K5 K6 A3 A4


## Goal

Create an SEO brief from synthetic keyword and page data while separating search intent, product facts and editorial assumptions.


## What you will produce

seo-content-brief.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

keyword, intent, volume, difficulty, target_page, priority


## Mechanism

Intent mapping links query evidence to an appropriate page and conversion goal. A brief contract separates title, headings, factual sources and internal-link targets.

Synthetic volumes are practice inputs, not current keyword research. Cowork can organise and draft from evidence; human editorial review and current analytics remain necessary.


## Detailed procedure

1. Download or copy the complete activity-08-seo-brief folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Classify each keyword into commercial,informational or offer mismatch using the supplied intent field. Exclude free water bottle from the paid product brief even though volume1200is highest.

5. Calculate900/(35+1)=25for the internal prioritisation heuristic. Draft title,H1,H2,source-backed facts and approved target links. Label volume values synthetic and never promise ranking.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Intent mapping links query evidence to an appropriate page and conversion goal. A brief contract separates title, headings, factual sources and internal-link targets. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request seo-content-brief.md in output/. Use the exact fields keyword, intent, volume, difficulty, target_page, priority where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: 900 × 1.0 / (35 + 1) = 25.00; the score is an internal planning heuristic, not a search-engine ranking formula. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: The highest-volume keyword is selected even though the brand sells a paid product. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Apply intent and offer compatibility before ranking by volume; exclude the “free” query from the paid product brief. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Update the brief when target-page inventory changes and rerun broken-link and claim checks. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Planning score = volume × relevance weight / (difficulty + 1)

900 × 1.0 / (35 + 1) = 25.00; the score is an internal planning heuristic, not a search-engine ranking formula.


## Acceptance checks

- Commercial and informational queries receive distinct target pages.

- Product claims trace to the source ledger.

- No guaranteed ranking or fabricated search statistics appear.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** The highest-volume keyword is selected even though the brand sells a paid product.

**Recovery:** Apply intent and offer compatibility before ranking by volume; exclude the “free” query from the paid product brief.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture