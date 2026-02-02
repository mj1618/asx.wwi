## Task: Model convertible notes + financing facilities dilution mechanics (ASX:WWI)

### Goal
Close the remaining “per‑share dilution mechanics” gap by building an **auditable** model of:
- **Convertible notes** (terms + conversion scenarios → shares),
- **Financing facilities** (drawn/undrawn + any equity-linked sweeteners like warrants/options),
and then wiring those mechanics into `valuation.md`, `ANALYSIS.md`, and (only if needed) `report.md`.

### Why this matters
The repo currently uses a **“fully diluted ex‑convertibles”** share count and explicitly notes that **convertible notes exist** but are **not fully modelled**. In a transition-to-producer window, convertibles and facility-linked equity can be first‑order drivers of:
- true fully diluted share count,
- financing runway / covenant risk,
- and per‑share upside/downside in the scenario table.

### Dependencies
- Completed: `001`–`010`
- No other swarm tasks in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- Update `sources.md` with citations for every primary document used to extract terms, including (at minimum):
  - 2024-10-29 quarterly + Appendix 5B (convertible note disclosure),
  - FY2025 annual report notes relevant to convertibles/financial instruments (if terms disclosed),
  - any later quarterlies/appendices that amend CN or facility terms,
  - any Appendix 2A / 3B / 3G documents that quantify CN counts, warrants, or new equity-linked instruments.

- Create a new file `financing.md` (or extend an existing file if a better home exists) with **auditable tables**:
  - **Convertible notes table** (one row per note):
    - issuer / holder (if disclosed), issue date, face value, coupon/fees, maturity, security, conversion price or formula, conversion conditions, any attached options, and primary source links.
  - **Facilities table** (one row per facility/provider):
    - provider, type (loan / facility), drawn vs undrawn, interest, maturity, key covenants (only if disclosed), equity-linked features (warrants/options), and primary source links.

- Update `valuation.md`:
  - Add an explicit **“Fully diluted incl. convertibles”** share-count section:
    - show base + options/warrants/perf rights + **CN conversion shares** under at least two scenarios (e.g., “at stated conversion price” and “worst-case max shares if formula-based”, only where disclosure supports it).
  - Recompute the simple NPV-per-share anchors under:
    - basic,
    - FD ex‑CNs (current),
    - FD incl‑CNs (new).

- Update `ANALYSIS.md`:
  - In **Capital structure + dilution risk**: replace “convertible notes exist” with:
    - the CN terms summary (one paragraph) plus a pointer to `financing.md`,
    - updated fully diluted share count range that includes CN conversion where supportable.
  - In the **scenario table**: ensure per-share ranges are consistent with the updated denominators (or explicitly state why not).
  - Add a short **changelog** entry describing the update and the evidence set used.

- Update `report.md` **only if** the CN/facility modelling changes:
  - the per-share scenario ranges materially, or
  - the 2-year downside probability / dilution-risk framing.

### Constraints / quality bar
- **Primary-source first**: do not infer terms that aren’t disclosed; if terms are missing, record “not disclosed in captured filings” and list the next document to pull.
- **Auditability**: every table row must link to a primary PDF.
- **Keep it mechanical**: future updates should be “add a row / update a row” when a new filing lands.

### Notes / expected approach
- Start from the repo’s current references:
  - `ANALYSIS.md` cashflow table notes CNs in Q3 2024 and CN count in Appendix 2A (2026-01-27).
  - `sources.md` already tags the 2024-10-29 quarterly as containing CN disclosure (A$1.5m CNs + 37.5m options).
- Then search forward in later quarterlies/appendices for:
  - conversion/repayment events,
  - term amendments,
  - new CN issuance,
  - facility restructures and any new equity-linked sweeteners.

---

### Completion note (2026-02-02)

Completed the deliverables using primary filings through the Dec 2025 quarter and Jan 2026 Appendix 2A:

- Added **`financing.md`** with auditable tables for:
  - **Convertible notes** (A$1.5m originally; conversion formula; maturity; options in lieu of interest; and **A$50k / 2 notes outstanding** as at 31 Dec 2025 quarter end).
  - **Facilities**: SA **ZAR 875m** IDC+Absa facility; **Nebari US$35m** facility (Tranche 1 drawn Nov 2025) including **166,933,764 warrants** and disclosed **US$0.0288** exercise price; **Absa 100,386,000 options** (A$0.0185 strike, 5-year).
  - Interim loan mechanics (repayable in shares at A$0.022).
- Updated **`valuation.md`** to include **FD incl. CN conversion** denominator (~4.985b) and show CN conversion share math.
- Updated **`ANALYSIS.md`** to replace “CNs exist” with a term summary, point to `financing.md`, and add an explicit **FD incl. CNs** denominator.
- Updated **`sources.md`** with new primary citations for Nebari/Absa/syndicated facility docs and expanded support statements for quarterlies.
- Updated **`announcements.md`** to include key financing announcements (credit approval, syndicated facility execution, Nebari facility, Absa options, Nebari drawdown notice).
- Updated **`report.md`** to remove the “convertibles not modelled” caveat and point to `financing.md`.

