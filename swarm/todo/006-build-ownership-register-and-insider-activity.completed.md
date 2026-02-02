---
id: 006
title: Build ownership / register concentration + insider activity (Appendix 3Y/3X + substantial holders)
status: completed
created: 2026-02-02
depends_on:
  - 001-build-initial-asx-wwi-deep-dive-outline.completed
  - 002-build-asx-announcement-timeline-and-cash-runway.completed
  - 005-build-management-governance-and-alignment.completed
---

## Goal

Build a **primary-source-backed** view of:
- **who owns WWI** (register concentration + substantial holders),
- **how ownership has changed** (substantial holder notices),
- and **what insiders have done** (director/KMP filings like Appendix 3Y / 3X / 3Z).

This closes a key gap in the deep dive: **alignment, liquidity/overhang, and control risk** beyond the FY2025 annual report snapshot.

## Deliverables

1. Create a new file `ownership.md` containing:
   - **Substantial holder timeline** (date, holder, %/shares before/after, change driver if disclosed, link).
   - **Director/KMP dealing timeline** from Appendix 3Y / 3X / 3Z (date, person, instrument, buy/sell, size, price, context).
   - **Register concentration** snapshots where available (e.g., Top 20 % from annual report(s) / any other primary filings).
   - A short **interpretation section** focused on investor-relevant signals:
     - potential overhang (custodians/nominees vs beneficial owners)
     - liquidity implications of concentrated register
     - repeated participation of insiders in raises (or lack thereof)
     - red flags (pledges, unusual option term changes, related-party placements, etc. — only if evidenced in filings)

2. Update `sources.md`:
   - Add a dedicated subsection for **director dealings** (Appendix 3Y/3X/3Z) and **substantial holder notices** with citation-format entries.

3. Update `ANALYSIS.md`:
   - Expand **1) Company snapshot → Major shareholders / register concentration** with dated, sourced bullets.
   - Add 2–4 items to **11) Risk register** related to ownership/control/liquidity (with leading indicators).

## Primary sources (must use)

- ASX historical announcements feed for WWI (to locate the relevant filings):
  - Appendix 3Y / 3X / 3Z (director interests & changes)
  - “Change of substantial holding” / “Becoming a substantial holder” notices
- FY2025 Annual Report already captured (Top 20 snapshot + any substantial holder disclosed there)

## Constraints / caveats

- Treat custodian/nominee lines in Top 20 as **not necessarily beneficial ownership**; be explicit about this limitation.
- Keep the output **auditable**: every row in a timeline must link to a primary document.
- Don’t “backfill” with guesses (e.g., don’t infer reasons for trades unless disclosed).

## Acceptance criteria

- `ownership.md` exists and contains at least:
  - 1 table for substantial holders
  - 1 table for director/KMP dealings
  - 1 short interpretation section with clearly-labeled evidence vs inference
- `sources.md` includes citations for each table entry (or at minimum the set of filings used).
- `ANALYSIS.md` reflects the latest sourced ownership facts and adds ownership-related watch-items.

## Notes

- Prefer the most recent ~24 months, but capture older filings if they explain a major holder’s entry/exit.
- If the volume is large, start with:
  - filings around major placements (Sep 2025, Jan 2026),
  - and any notices involving known disclosed holders (e.g., Wingfield Durban Deep LP from FY2025 annual report).

## Completion notes (2026-02-02)

- Created `ownership.md` with:
  - substantial holder timeline (incl. Wingfield Durban Deep LP Form 603 + FY2025 annual report snapshot),
  - director dealings timeline (Aug 2025 placement participation; Dec 2025 performance-right issue; Jan 2026 vesting/exercise),
  - register concentration snapshot (Top 20 % from FY2025 annual report),
  - interpretation section with evidence vs inference.
- Updated `sources.md` with dedicated citations for director dealings and substantial holder notice.
- Updated `ANALYSIS.md` ownership bullets + added ownership/liquidity risks and pointed “director dealings” to `ownership.md`.

