# CLAUDE.md — Claude Cowork for Digital Marketing

## What this is

Courseware for the WSQ course **Claude Cowork for Digital Marketing**
(`TGS-2023018659`, TSC System Integration ICT-DIT-3016-1.1), Tertiary
Infotech Academy Pte Ltd (UEN 201200696W). Two days, 16 hours: 13.5 h
training + 2.5 h assessment (WA 3:30–4:30 PM, PP 4:30–6:00 PM, Day 2).

Since v10.0 the course follows **Multi AI Agents Workflow for Content
Creation** (`TGS-2023036153`, Claude Edition v3.7): the same use case
(Horizon Wealth Planning, a fictitious Singapore financial-planning firm),
the same 15 labs, the same charcoal/cream/orange deck and overview slides —
mapped to this course's TSC:

| LO | Topic | K | A | Labs |
|---|---|---|---|---|
| LO1 | T1 Components, compatibility and integration | K1–K3 | A1, A2 | 1–5 (compatibility matrix in Lab 4) |
| LO2 | T2 Testing integrations and troubleshooting | K4–K6 | A3, A4 | 6–12 |
| LO3 | T3 Versioning, change proposals, best practices | K7 | A5 | 13–15 (versions 1.0/1.1 + change proposal in Lab 14) |

Everything learners receive is **generated**. Never hand-edit `courseware/`,
`labs/` or `docs/prompts/` — fix the source in `build/` and rebuild.

## Build (build/ is private, git-ignored)

```
cd build
python3 build_deck.py                      # deck + slide_map.json
python3 qa_deck.py ../courseware/*.pptx    # must be 0 issues
python3 build_docs.py                      # LP, LG (+ .md); asserts lab slots = lab minutes
python3 build_labs.py                      # labs/ (15 folders + horizon-studio)
python3 build_assessment.py                # assessment/ — WA 7 SAQ (K1-K7), PP 5 tasks (A1-A5)
python3 build_prompts_page.py              # docs/prompts/ (GitHub Pages)
cd ../courseware && soffice --headless --convert-to pdf "Claude Cowork for Digital Marketing-v<V>.pptx"
```

Then render every page and look (house rule), and run /courseware-qa.

- `build/variant.py` — title, code, version, date, TSC, output folders.
- `build/v3_content.py` — the slide sequence and the SCHEDULE.
- `build/v3_labs.py` — the 15 labs; `build/team.py` — the six agents;
  `build/hz_data.py` — the business and its synthetic data.
- `build/build_assessment.py` — WA/PP and answer keys; every question cites
  slides by title, so a renamed slide fails the build.

## Boundaries

- **Never delete files without asking** (workspace AGENTS.md). Superseded
  versions are moved to `courseware/archive/`, `assessment/archive/` and
  `archive/` — all git-ignored.
- `assessment/`, `reference/`, `build/`, `course_application/` and `.env`
  are private. Answer keys never leave the repo.
- The public Horizon website and the Prompts page are served from `docs/`
  on GitHub Pages.
