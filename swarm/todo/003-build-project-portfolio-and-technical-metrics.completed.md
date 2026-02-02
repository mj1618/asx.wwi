## Task: Build project portfolio factsheets + key technical metrics (WWI)

### Goal
Populate `ANALYSIS.md` with a **primary-source-based** project/asset inventory for ASX:WWI, including each flagship project’s:
- location/jurisdiction
- ownership/JV terms (WWI % interest)
- stage (exploration / development / production)
- current resource/reserve metrics (JORC where available)
- near-term work program + dated catalysts
- key project-specific risks and gating items

### Why
We have cash/runway + capital structure (`ANALYSIS.md`) and a curated announcements timeline (`announcements.md`), but the deep-dive still can’t progress to **valuation, peer comps, or scenario probabilities** until we nail down **what WWI actually owns and what each asset contains** (resource, grade, confidence, development status, critical path).

### Deliverables
- Update `ANALYSIS.md`:
  - Fill **1) Company snapshot** (primary assets/projects, jurisdictions, stage).
  - Fill **3) Asset/Project inventory** with a repeatable template per project.
  - Fill **5) Catalysts + timeline** with at least 5–10 dated items tied to filings.
  - Add/expand **citations log** with the key PDFs used for every number/claim.
- Update `sources.md`:
  - Add direct links to the **latest investor presentation/corporate deck** (if published).
  - Add links to any **technical study** documents referenced (scoping/PFS/DFS), if they exist.
- Optional (if it materially improves clarity):
  - Add a new section to `announcements.md` listing the **highest-signal technical/project** announcements (resource updates, production guidance, permitting) with one-line “why it matters”.

### Primary sources to start with (already captured)
- **2.2Moz Increase to WBP Global JORC Mineral Resource Estimate to 7.24Moz Gold** — *2026-02-02* — extract: resource totals, grade, Measured/Indicated/Inferred breakdown, and any project context/assumptions.
  - PDF: `https://announcements.asx.com.au/asxpdf/20260202/pdf/06vvhp4zxswsgh.pdf`
- Latest quarterlies already linked in `sources.md` (for project status and work program narrative).

### Method / Extraction checklist
- For each project mentioned in filings:
  - Identify project name(s) and aliases (e.g., “WBP”, “Qala Shallows”, any uranium projects).
  - Capture: jurisdiction, tenure status, ownership %, key counterparties (if any).
  - Capture: latest resource/reserve table(s) and date + competent person statement reference.
  - Capture: development status (mining method, processing route, throughput, guidance), if provided.
  - Capture: explicit upcoming milestones (drilling, studies, permitting, construction, production ramp).
- Keep every extracted number tied to a **single primary PDF** with date.

### Constraints / Notes
- Use **primary sources only** for technical numbers (JORC tables, study metrics, ownership terms).
- If investor decks/websites are used, treat them as **secondary** and cross-check in ASX PDFs where possible.
- Do not speculate on economics if no study exists; instead list “TBD” and note missing source.

### Dependencies
- `001-build-initial-asx-wwi-deep-dive-outline.completed.md` (done)
- `002-build-asx-announcement-timeline-and-cash-runway.completed.md` (done)

### Completion notes
Completed on 2026-02-02.

- Updated `ANALYSIS.md` with a primary-source-based project portfolio:
  - WBP (South Africa): tenure/ownership, updated global JORC MRE (7.24Moz @ 4.0g/t), and Qala Shallows near-term production milestones.
  - Mt Cecilia (WA): ownership status post Rio Tinto farm-in lapse + key drilling intercepts as summarised in the latest quarterly.
  - Derewo (Indonesia): disclosed interests + current “divest / no activity” status.
- Added a dated catalysts table (next 6/12/24 months) tied to ASX PDFs.
- Expanded `sources.md` with links to company-hosted corporate presentations/webinars (secondary) and ensured the key JORC resource update ASX PDF is captured under technical documents.
- Added a “highest-signal technical/project announcements” quick index to `announcements.md` for faster navigation.

