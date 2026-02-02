## Task: Build peer comps + relative valuation (ASX:WWI)

### Why this matters
`ANALYSIS.md` currently leaves the **peer set** and **peer-multiple triangulation** as **TBD**. A comps table is the fastest way to sanity-check the DFS/NAV-style anchor and to quantify how much of WWI’s pricing is “developer discount” vs “structural dilution/jurisdiction risk”.

### Dependencies
- Completed: `001`–`006` (outline, announcements timeline/cash runway, project portfolio/metrics, scenario valuation, management/governance, ownership/insider activity).
- No other swarm tasks in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- **Peer set selection** (10–20 companies) with a short rationale per peer, split into buckets:
  - **AU-listed gold developers nearing first gold** (closest stage comps)
  - **AU-listed SA/SSA jurisdiction gold developers/producers** (jurisdiction discount comps)
  - **AU-listed high-dilution “serial raisers” vs self-funders** (cap-structure comps)
  - Optional: **Wits/SA basin-adjacent** or similar underground reef-style operations (if any clean comps exist)
- **Comps table** in a new markdown file `peers.md` (create if missing) with at least:
  - Ticker/company
  - Stage (explorer/developer/producer), jurisdiction(s)
  - Market cap, EV (or a clear proxy if EV not reliably computable)
  - Resource/Reserve (oz Au) and grade (where available)
  - Key study metric (NPV/IRR/AISC) if published
  - Funding status (cash, debt, recent raise/dilution notes)
  - Multiples: EV/oz (resource and reserve), EV/NPV (if NPV available)
  - Source links (ASX/SEDAR/EDGAR/annual reports; secondary market data clearly labelled)
- **Relative valuation triangulation** added to:
  - `valuation.md`: a section “Peer multiples cross-check” with explicit assumptions + caveats
  - `ANALYSIS.md`: fill the “Peer set” section and add a short “What comps imply vs current price” paragraph
- **Citations**:
  - Add any new primary sources to `sources.md` (peer annual reports, technical reports, ASX announcements).
  - If using market-data snapshots (e.g., Google Finance), mark them as **secondary** and include **as-of date**.

### Constraints / quality bar
- Prefer **primary** filings for resources/reserves and study metrics; avoid promotional decks unless they link to the filing.
- Avoid forcing precision: if EV is unreliable, compute a **range** or document why EV is omitted.
- Keep comps “apples-to-apples”: flag major differences (open pit vs underground, jurisdiction, by-products, processing, royalties/streams).

### Suggested workflow
1. Draft candidate peers by stage + jurisdiction; narrow to a defendable list.
2. For each peer, capture: latest resource/reserve statement, latest cash + debt, and most recent study economics (if any).
3. Compute multiples in a consistent way; document FX assumptions and date-stamps.
4. Update `valuation.md` and `ANALYSIS.md` with the key takeaways and the main caveats.

### Notes / expected outcome
This section should answer: **“If WWI executes its ramp, what peer multiple could it converge to, and how sensitive is per-share value to dilution vs multiple expansion?”**

### Completion notes (b11afd72)
- Created `peers.md` with an 11-name peer set, grouped into stage + jurisdiction + cap-structure buckets, and added an initial comps table (market cap + EV proxy + EV/oz + EV/NPV where available) with explicit caveats.
- Updated `valuation.md` with a “Peer multiples cross-check” section (explicit EV proxy math + interpretation).
- Updated `ANALYSIS.md` “Peer set” section and added a short “What comps imply vs current price” paragraph.
- Updated `sources.md` with new peer sources (primary PDFs where available; TradingView market-cap snapshots clearly labelled secondary).
- Notes:
  - Some peer technical metrics were only accessible via company website summaries during this pass (flagged as secondary in `sources.md`).
  - Theta (TGM) issued a later announcement warning investors not to rely on certain forward-looking production/forecast info in its FS announcement; this is explicitly flagged in `peers.md` and `sources.md`.

