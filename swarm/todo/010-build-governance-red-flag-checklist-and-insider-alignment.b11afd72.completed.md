## Task: Build a governance red-flag checklist + insider alignment dashboard (ASX:WWI)

### Goal
Close the remaining “governance + alignment” gaps by creating an **auditable**, easy-to-update dashboard that turns scattered disclosures into:
- a **quarterly related-party payments trend** (Appendix 5B item 6),
- a **substantial holder change timeline** (Forms 603/604),
- an **insider dealing / incentive issuance summary** (Appendix 3X/3Y/3Z),
and then wiring the highest-signal takeaways back into `ANALYSIS.md` (and `report.md` only if it materially changes the thesis).

### Why this matters
WWI is in a capital-markets-dependent transition-to-producer window where **governance optics + dilution mechanics** can meaningfully affect cost of capital and per‑share outcomes. Today, the repo has good qualitative notes, but not a single “dashboard” that is both **traceable** and **mechanical to update**.

### Dependencies
- Completed: `001`–`009`
- No other swarm tasks in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- Update `ownership.md` to include:
  - **Quarterly related-party payments trend** table:
    - One row per quarter (at least the last 8 quarters already captured in `sources.md`), with:
      - quarter end date
      - Appendix 5B item 6.1 total (A$)
      - short note for any material drivers (only if explicitly disclosed)
      - primary citation link (the ASX PDF containing the Appendix 5B)
  - **Substantial holder timeline** expanded to cover the last ~24 months:
    - Add any Forms **603/604** discovered in the ASX feed and record:
      - holder, effective date, prior → after voting power, notes, and source link
    - If no 603/604s exist in the period, explicitly state “none found” with the date range checked and the ASX announcement index link used.
  - **Insider / director / KMP dealing summary** improvements:
    - Ensure Appendix 3X/3Y/3Z rows are complete for the last ~12–24 months of material changes (focus on:
      - placement participation,
      - performance rights grants/vesting,
      - option/warrant issues to KMP/associates,
      - net selling if present).

- Update `sources.md`:
  - Add citations for every new primary doc used (especially any newly added 603/604 or missing 3X/3Y/3Z items).

- Update `ANALYSIS.md`:
  - Refresh the governance/dilution “watch-items” with the new hard data:
    - trend of related-party payments (direction + magnitude),
    - any new substantial holder dynamics or overhang risk evidence,
    - any notable insider selling/buying/incentive cadence.
  - Add a short changelog entry describing the update and the evidence set used.

- Update `report.md` **only if** the new evidence changes:
  - the scenario probabilities,
  - the 2-year downside probability framing,
  - or the top governance risks / cost-of-capital narrative.

### Constraints / quality bar
- **Auditability first**: every row must link to a primary PDF, and any inference must be labelled as inference.
- **Don’t duplicate**: keep detailed tables in `ownership.md`; keep `ANALYSIS.md` to the “best summary”.
- **Mechanical updates**: structure tables so future updates are “add a row, add a citation”.

### Completion notes
(Completed 2026-02-02.)

- Added an **Appendix 5B item 6 related-party payments trend table** to `ownership.md` (last 8 quarters, with **primary ASX PDF links** and explicit **A$’000 units**).
- Expanded the **substantial holder section** in `ownership.md` with an explicit statement that **no Form 603/604 filings were identified** in the **ASX 2024–2026 year-view announcement indices** (links captured), and retained the historical Form 603 + FY2025 annual report snapshot.
- Updated `sources.md` to:
  - add ASX year-view index citations (2024/2025/2026),
  - mark director interest + substantial holder checks as complete (with the “none found” note for 2024–2026),
  - and update the quarterly Appendix 5B citations to explicitly include **item 6 (6.1/6.2)** support.
- Updated `ANALYSIS.md` to reflect the new hard data (step-up in item 6.1 during Sep/Dec 2025 quarters) and added a changelog entry.
- Updated `report.md` governance watch-items to include the **Sep 2025 (A$357k)** and **Dec 2025 (A$607k)** Appendix 5B item 6.1 values (points to `ownership.md` for the table).

