# Activity 09 — Lifecycle email segmentation and consent


**Course:** Claude Cowork for Digital Marketing | TGS-2023018659 | v8.0

**Time:** 35 minutes | **Mapping:** LO2; K4 K5 K6 K7 A3 A4


## Goal

Design an abandoned-cart email draft using a synthetic consent-safe segment and explicit suppression rules.


## What you will produce

email-draft.md; test-evidence.csv; integration-notes.md; change-proposal.md


## Workflow

![Synthetic training workflow](workflow.png)


## Tools and boundaries

Claude Cowork access through a currently supported surface; desktop for local-folder access. A spreadsheet or text editor is sufficient for independent verification. Optional connector paths are design exercises unless an authorised sandbox is available. This activity is self-contained; no live customer, ad or email account is required.


## Input contract

customer_id, consent, cart_age_hours, purchased, suppressed, eligible


## Mechanism

Event predicates determine timing; consent and suppression determine eligibility. A segment preview provides evidence before any independently approved campaign send.

The training predicate is a synthetic internal contract, not a vendor-specific segmentation API. Separate business timing assumptions from the legal and account-specific conditions used by a real organisation.


## Detailed procedure

1. Download or copy the complete activity-09-lifecycle-email folder. Keep input/ unchanged and create a separate output/ folder for your work.

2. Read assets/brand-source.md, assets/claim-ledger.csv and input/mock-data.csv. Check the campaign period, SGD currency and synthetic identifiers before analysis.

3. Open workflow.png and read the input contract. Record the responsible owner and read-only boundary in output/integration-notes.md.

4. Create five Boolean columns: consent_yes,cart_age_at_least24,not_purchased,not_suppressed,eligible. Evaluate all five customer rows.

5. SYN001must be the only eligible row. Record the distinct exclusion reason for SYN002–SYN005. Keep output a draft with placeholder addresses;do not connect or send through an email service.

6. In an available Claude Cowork surface, start a new task. For local-folder access use the desktop workflow documented by Anthropic; choose only this activity folder. For web/cloud work upload the relevant synthetic files through the supported interface.

7. Copy Prompt 1 from prompts.pdf. Attach the mock-data.csv, approved brand sources and the activity guide. Ask Claude to explain any missing or incompatible fields before generating conclusions.

8. Compare the proposed plan with this activity mechanism: Event predicates determine timing; consent and suppression determine eligibility. A segment preview provides evidence before any independently approved campaign send. Reject any proposed send, publication, credential change or live account action.

9. Copy Prompt 2 and request email-draft.md in output/. Use the exact fields customer_id, consent, cart_age_hours, purchased, suppressed, eligible where applicable. Preserve raw values and distinguish course contract fields from vendor schemas.

10. Independently check the worked example: Only SYN001 is eligible in the five-row fixture: 1 / 5 = 20%. Use a spreadsheet or hand calculation. Record observed values alongside expected values in output/test-evidence.csv.

11. Inject or inspect the deliberate failure: A natural-language segment includes customers who withdrew consent. Use Prompt 3 to isolate a minimal failing row or source claim. Do not permit silent corrections to the raw source.

12. Apply the bounded recovery: Treat consent and suppression as hard gates, recompute the preview and retain exclusion evidence. Save a new correction copy, record what changed and rerun the affected checks.

13. Complete each acceptance check below and record pass/fail, filename, rule version and date. Keep failed evidence rather than deleting it.

14. Write output/change-proposal.md: Version consent and suppression rules separately from subject-line experiments. Include owner, affected interface, test plan and rollback trigger.

15. Use Prompt 4 to obtain a concise review memo with source links, unresolved limits and an explicit Draft or Candidate state. Human review is required before any real campaign action.

16. Submit only the activity outputs, test evidence and change proposal to the trainer. Do not submit real customer data, credentials, copyrighted reference ebooks or live-account exports.


## Worked verification

Separate worked-example fixtures: worked-checks.csv(A01),claim-audit.csv(A02),source-campaigns.csv and analytics-campaigns.csv(A03),raw-tracking.csv(A04),dirty-export.csv(A07),initial-asset-manifest.csv(A10). These support the worked calculations; mock-data.csv may be a summary/error ledger rather than the raw input.

Eligibility = consent AND cart_age ≥ 24 AND NOT purchased AND NOT suppressed

Only SYN001 is eligible in the five-row fixture: 1 / 5 = 20%.


## Acceptance checks

- Only SYN001 enters the segment preview.

- No real email addresses or live sending credentials are used.

- The output remains a draft and includes an unsubscribe-placeholder review note.

- Raw input remains unchanged; each result names its evidence file.


## Troubleshooting

**Failure:** A natural-language segment includes customers who withdrew consent.

**Recovery:** Treat consent and suppression as hard gates, recompute the preview and retain exclusion evidence.


## Completion boundary

A generated artifact or fixture pass does not prove a live connector, campaign send, website tag installation or external publication. Record the exact work you performed.


## Prompt pack

Use prompts.pdf; prompts.md contains the same editable text.


## Sources

- Anthropic Cowork product: https://claude.com/product/cowork

- Anthropic Skills: https://support.claude.com/en/articles/12512176-what-are-skills

- MCP architecture: https://modelcontextprotocol.io/docs/learn/architecture