## Task: Build an ongoing monitoring dashboard + post–first-gold update (ASX:WWI)

### Goal
Create a lightweight, repeatable **update protocol** so this repo stays current as WWI moves through **first gold + ramp** and issues new quarterlies / Appendix 5Bs / capital-structure notices.

### Why this matters
The current analysis/report snapshot is **as-of 2026-02-02** and is dominated by forward-looking “first gold Mar 2026” and ramp-risk framing. The highest-value next increment is a structured process to:
- ingest new primary documents quickly,
- update cash/runway + cap-structure dilution math,
- update the scenario probabilities and “2-year downside probability” based on real milestone outcomes.

### Dependencies
- Completed: `001`–`008`
- Ensure no other swarm tasks are in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- Create `monitoring.md` with a **repeatable checklist** that answers:
  - what to check (ASX announcements, quarterlies, Appendix 5B, Appendix 2A/3B/3G, Form 603/604, director 3Y/3X),
  - how often (weekly / monthly / quarterly),
  - what key numbers to extract (cash, burn, quarters of funding, shares/options/warrants, facility movements, related-party payments),
  - where to record updates (which repo files, and in what format).
- Update these files to the new “as-of” date (based on the latest available primary docs):
  - `announcements.md`: extend the timeline from **2026-02-02 → latest**
  - `sources.md`: add citations for every new primary document used (clearly label any secondary market snapshots)
  - `ownership.md`: add any new director interest notices and any new/change substantial holder notices (603/604), with dates and key deltas
  - `ANALYSIS.md`: refresh the “best summary” sections that are materially affected:
    - cash/runway table (Appendix 5B)
    - cap structure snapshot (Appendix 2A / 3G)
    - catalysts table (update which milestones were met/missed)
    - scenario probabilities + 2-year downside probability (update rationale)
  - `report.md`: update “as-of date”, market snapshot numbers, and the “what would change probability” leading indicators if the new evidence warrants it
- Add a short **changelog section** (one place only) noting what changed since the prior as-of date and why it matters.

### Constraints / quality bar
- Prefer **primary sources** (ASX PDFs, audited reports). Secondary snapshots must be clearly labeled with **as-of date**.
- Keep changes tight and investor-readable; avoid duplicating tables across multiple files.
- When updating probabilities, state the **new evidence** that justified the change (avoid “vibes-based” adjustments).

### Notes / expected outcome
This task should make future updates “mechanical”: new filings come in → update a small set of tables and the probability framing → keep `ANALYSIS.md`/`report.md` current without redoing the entire deep dive.

### Completion notes (what I changed)
- Added `monitoring.md` with a repeatable weekly/monthly/quarterly checklist and a post–first gold update template, and pointed core docs at it.
- Fixed the ASX announcements “year view” URLs in `announcements.md` and `sources.md` so the canonical index link works.
- Added a single changelog entry in `ANALYSIS.md` (and made `ANALYSIS.md` the single source of truth for changelog going forward).

