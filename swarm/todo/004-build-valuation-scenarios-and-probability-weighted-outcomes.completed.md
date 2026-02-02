---
id: 004
title: Build valuation scenarios + probability-weighted outcomes
status: completed
depends_on:
  - 002-build-asx-announcement-timeline-and-cash-runway.completed
  - 003-build-project-portfolio-and-technical-metrics.completed
created: 2026-02-02
---

## Goal

Produce a **transparent, assumption-driven valuation** for WWI with **bull/base/bear scenarios** and a **probability-weighted outcome** view that ties back to funding/dilution and project milestones.

This should directly support the README request: “prediction of the price going forward”, and “likelihood of different outcomes / chance it doesn’t go up in the next couple of years.”

## Scope

- Build a compact, auditable valuation narrative (not a giant spreadsheet) that:
  - Connects **projects → milestones → capex/opex → funding → dilution → value per share**
  - Expresses outcomes as **ranges** and **probabilities**, not a single point estimate
- Peer comps only where they are meaningful (stage/commodity/jurisdiction), with clear caveats.

## Non-goals

- Not a recommendation / advice; keep to research-style framing.
- No “precision theater” (don’t claim accuracy beyond the quality of public inputs).

## Inputs to gather (sources.md updates likely)

- Latest capital structure: shares on issue, options, performance rights, convertibles (if any)
- Latest cash + burn + committed spend; upcoming funding triggers (from task 002)
- Project economics signals from task 003:
  - Resource/grade/geometry, mining method assumptions, metallurgy/recovery signals
  - Any published study numbers (scoping/PFS/DFS) if they exist
- Commodity assumptions: base-case gold price, FX, inflation (range)
- Cost benchmarks: typical AISC / capex ranges for comparable deposit types (range)

## Deliverables

1. `ANALYSIS.md` update with a new section:
   - **Scenario table** (bull/base/bear) including:
     - key milestones and timelines
     - funding needed and dilution assumptions
     - implied valuation range and per-share range
     - principal failure modes
   - **Probability-weighted outcomes** (explicit weights + rationale)
   - **2-year downside probability** narrative aligned to milestones and funding risk

2. `sources.md` updated with:
   - capital structure references
   - any economic study links / announcements used
   - peer references (only if used)

3. (Optional) `valuation.md` with the long-form reasoning if `ANALYSIS.md` would become too dense.

## Acceptance criteria

- Every numeric conclusion is traceable to an assumption + source (or clearly labeled as an estimate).
- Explicitly models **dilution** and how it changes per-share outcomes.
- Clearly separates:
  - what the company has published (facts)
  - what is inferred (assumptions)
  - what is unknown (key uncertainties)

## Execution plan (suggested)

- Reconcile cap structure from latest filings/announcements; build fully diluted share count range.
- Translate project status into milestone-driven scenario timelines (per task 003 + announcements).
- Create simple valuation frameworks suitable for early-stage mining:
  - EV/oz (with stage discount)
  - risked NPV (coarse, with wide bands)
  - “funding path” sanity check (runway vs milestones)
- Assign probabilities and justify them using observed risks (permitting, funding, technical, jurisdiction).
- Update `ANALYSIS.md` and `sources.md`; keep the summary readable.

## Completion notes (2026-02-02)

- Updated `ANALYSIS.md` with:
  - a bull/base/bear scenario table including milestone-driven narratives, dilution assumptions, valuation ranges, and a 2-year downside probability framing.
  - current-market context for share price / market cap (explicitly marked as secondary-source snapshot).
- Updated `sources.md` with the primary DFS technical release link and the market/FX snapshot references.
- Updated `announcements.md` to include the **2025-07-23** DFS update (NPV/IRR/AISC/peak funding + sensitivities) as a high-signal technical milestone.
- Added `valuation.md` to keep the “math and assumptions” auditable without bloating `ANALYSIS.md`.

