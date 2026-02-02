## Task: Resolve remaining TBDs + tighten the investor summary (ASX:WWI)

### Goal
Eliminate the remaining **“TBD” placeholders** in the investor-facing summary artifacts by filling (or explicitly bounding) missing items using **primary-source-backed** data and clearly marked assumptions.

### Why this matters
The repo is largely complete, but a handful of “TBDs” remain in `ANALYSIS.md` and `peers.md` that weaken the “hand-to-an-investor” quality bar. Closing them improves:
- the **auditability** of key metrics (EV, dilution, governance signals),
- the **comparability** against peers (comps table gaps),
- and the “what the market is missing” framing (variant view).

### Dependencies
- Completed: `001`–`011`
- No other swarm tasks in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- Update `ANALYSIS.md` to remove/resolve these items:
  - **Enterprise value (EV)**: add an explicit EV estimate and formula (EV \(=\) market cap + debt − cash), with the “as-of” date and clear caveats (debt definition, cash timing, off-balance-sheet / finance leases if any).
  - **Variant view**: replace the placeholder with 3–6 concise bullets that articulate *why* WWI might be mispriced vs consensus, tied to explicit evidence and “what would falsify this view.”
  - **Director dealings signals + constraints**: add a short framework section that explains how to interpret Appendix 3Y/3X activity for this name (placement participation vs market buying; incentive vesting; nominee opacity), pointing to `ownership.md`.
  - **Risk register**: replace “Likelihood/Impact/Mitigants = TBD” with qualitative rankings (Low/Med/High) and practical mitigants / leading indicators consistent with the monitoring protocol.

- Update `peers.md` to resolve the remaining peer-table “TBD” cells (notably **RMS** and **GMD**) using primary sources where possible:
  - Fill **resource / reserve** numbers and the metric lens you’re using (EV/oz resource, EV/oz reserve, EV/NPV if study exists).
  - Add **primary citations** for the resource/reserve/study claims to `sources.md` (PDF links preferred; company website pages only as pointers, marked as secondary).
  - If a primary source cannot be captured quickly, replace “TBD” with “not captured in repo; next doc to pull: <title/link>”.

- Keep `report.md` unchanged unless closing these TBDs changes any key investor-facing conclusions (thesis, probabilities, downside framing); if it does, update with a short “as-of” note.

### Constraints / quality bar
- **Primary-source first**: do not invent numbers; if uncertain, explicitly label assumptions and point to the missing document.
- **Auditability**: every new numeric claim should be traceable via `sources.md` and/or an ASX PDF.
- **Consistency**: EV, share counts, and cash/debt definitions must match across `ANALYSIS.md`, `valuation.md`, and `report.md` (or differences must be explicitly justified).

### Notes / expected approach
- Start by enumerating remaining `TBD` occurrences (repo-wide) and close them one-by-one, prioritizing `ANALYSIS.md` then `peers.md`.
- For EV: use the repo’s stated market cap snapshot + latest quarter cash + disclosed drawn facilities, and clearly label this as an *approximate* EV.
- For peer “TBDs”: prefer the latest ASX releases / annual reports / JORC PDFs for resources/reserves; keep citations tight and dated.

