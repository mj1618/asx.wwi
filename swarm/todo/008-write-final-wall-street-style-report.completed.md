## Task: Write the final “Wall Street-style” WWI deep-dive report (ASX:WWI)

### Goal
Produce a single, readable, decision-support **final report** that directly answers `README.md` using the already-built primitives:
`ANALYSIS.md`, `announcements.md`, `valuation.md`, `peers.md`, `ownership.md`, and `sources.md`.

### Why this matters
Right now the repo contains strong building blocks, but not a clean “hand to an investor” memo that:
- summarises the **most important things to know**
- states a **forward price view** (as ranges + probabilities)
- states the **chance the stock doesn’t go up over the next couple of years** (and why)

### Dependencies
- Completed: `001`–`007`
- No other swarm tasks in progress (no `.processing.md` files in `./swarm/todo/`).

### Deliverables (definition of done)
- Create a new markdown file: `report.md`
  - **Executive summary (one page)**:
    - what WWI is, what it owns, what the market is pricing (as-of date)
    - 5–10 “most important” points (facts + implications)
  - **Business + assets**:
    - WBP/Qala Shallows: where the value is, gating milestones, key unknowns
    - non-core/optionality (Mt Cecilia, Derewo) framed honestly
  - **Financing + dilution**:
    - runway framing, what “success” looks like from a funding perspective
    - dilution/overhang watch-items (options/warrants/convertibles)
  - **Management/governance + alignment**:
    - high-signal positives + red flags (related-party spend, structure), with citations
  - **Valuation & scenarios**:
    - bull/base/bear outcomes and **probability weights**
    - explicit **2-year downside probability** and what would change it
    - clearly state “price targets” as **ranges** and link to `valuation.md`
  - **Peer comps cross-check**:
    - 5–8 bullet conclusions from `peers.md` (don’t duplicate tables; link instead)
  - **Catalysts + what to monitor**:
    - a short “watchlist” (quarterly indicators, ASX forms, operational KPIs)
  - **Risks**:
    - a compact risk matrix (likelihood/impact, top 8–12 items) and leading indicators
  - **Appendix**:
    - “Key sources” section that points to `sources.md` and the most important primary links
- Update `ANALYSIS.md` only if needed to keep it the “best summary” (e.g., add a pointer to `report.md`, or tighten any stale “TBD” labels that are now resolved by tasks `005`–`007`).

### Constraints / quality bar
- Keep it **investor-readable**: aim for ~3–8 pages equivalent; avoid duplicating tables already in the repo.
- Every material claim should be traceable to a citation in `sources.md` or a clearly-labelled secondary snapshot with an **as-of date**.
- Avoid “precision theatre”: use ranges, explicitly label assumptions, and separate facts vs inference.

### Notes
- This task is primarily synthesis/writing; no code/tests expected unless a small tooling script is genuinely helpful (only add tooling if it reduces future maintenance burden).

### Completion notes (b11afd72)
- Created **`report.md`** as the single investor-ready memo synthesising `ANALYSIS.md`, `valuation.md`, `announcements.md`, `peers.md`, `ownership.md`, and `sources.md`.
- Included explicit **bull/base/bear** ranges with probability weights and an explicit **2-year downside probability** with leading indicators to update it.
- Updated **`ANALYSIS.md`** to point readers to `report.md` as the “hand-to-an-investor” deliverable.

