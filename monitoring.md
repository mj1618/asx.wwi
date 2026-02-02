# ASX:WWI — Ongoing monitoring + post–first gold update protocol

*As-of date: **2026-02-02** (latest primary document captured in this repo: **WBP JORC MRE update**, 2026-02-02)*  
*Purpose: make updates “mechanical” as new filings arrive.*

## What this is
This repo’s deep dive is a snapshot anchored to primary documents captured in `sources.md`. This file defines a repeatable, lightweight **update protocol** so that when WWI releases new:
- quarterlies + Appendix 5B,
- capital-structure notices (Appendix 2A/3B/3G),
- substantial holder notices (603/604),
- director interest notices (3X/3Y/3Z),
- “first gold” / ramp milestone updates,

…you can update the analysis without redoing the entire deep dive.

## The update loop (10–30 minutes when practiced)

### Inputs (what to check)
- **ASX announcements index** (canonical list; then open the relevant PDFs):
  - Current year: `https://www.asx.com.au/asx/v2/statistics/announcements.do?by=asxCode&asxCode=WWI&timeframe=Y&year=2026`
  - Prior year: `https://www.asx.com.au/asx/v2/statistics/announcements.do?by=asxCode&asxCode=WWI&timeframe=Y&year=2025`
- **Company investor materials** (secondary): `https://westwitsmining.com/presentations/` (use as pointers; verify numbers in ASX filings).

### Outputs (where to record updates)
- `sources.md`: add citations for every new primary document used (link + date + claim supported).
- `announcements.md`: add *material* items to the curated timeline (quarterlies/5Bs, raises, cap-structure changes, major ops/technical updates).
- `ownership.md`: add any new director interest notices (3X/3Y/3Z) and substantial holder changes (603/604).
- `ANALYSIS.md`: refresh the “best summary” tables/sections that are materially affected (cash/runway, cap-structure snapshot, catalysts, scenario probabilities).
- `report.md`: update the investor-facing memo **only** if the new evidence changes the thesis/probabilities/critical watch-items.

## Cadence

### Weekly (5–10 minutes)
- Scan the ASX announcements index for new items since the last update.
- If there are new *material* filings:
  - capture the PDF link in `sources.md` with date and 1-line “supports” text
  - add the item(s) to `announcements.md`
  - update any obvious “leading indicator” deltas in `ANALYSIS.md` (cash/runway/cap-structure/catalysts).

### Monthly (15–30 minutes)
- Review whether any new disclosures should change:
  - funding/dilution risk framing,
  - timeline confidence (“first gold” date confidence, ramp assumptions),
  - governance watch-items (related-party payments trend).
- Ensure `report.md` still matches the current evidence set (as-of date, catalysts, downside probability rationale).

### Quarterly (30–60 minutes; triggered by Quarterly + Appendix 5B)
When a new Quarterly + Appendix 5B lands, do the following extraction and updates.

## Quarterly extraction checklist (Appendix 5B + quarterly narrative)

### Numbers to extract (put into `ANALYSIS.md`)
From Appendix 5B / quarterly cashflow report:
- **Quarter end date**
- **Ending cash**
- **Net cash from operating activities**
- **Net cash from investing activities**
- **Net cash from financing activities**
- **Estimated quarters of funding available** (Appendix 5B item 8.7)
- **Related-party payments** (Appendix 5B item 6.1) + any narrative breakdown
- **Financing facilities**: drawn vs undrawn, changes in the quarter, and any equity-linked sweeteners (warrants/options)

From the quarterly narrative:
- **Operational milestone status**:
  - first gold (achieved? date? conditions?)
  - ore mined / stockpiled / delivered to processing (tonnes, grade if disclosed)
  - processing / toll-treatment status (start date, constraints, changes)
  - ramp commentary vs plan (throughput, reconciliation, delays)
- **Guidance / targets** (if any) and explicit caveats
- **Material risks/events** (permitting, regulatory, safety, community, funding)

### Where this gets updated
- `ANALYSIS.md`:
  - cash/runway table row (new quarter)
  - runway estimate paragraph (update 8.7 and any simple heuristics)
  - risk register watch-items if something changed (e.g., quarters-of-funding falls < 2)
- `report.md`:
  - only update if the new quarter changes the thesis or scenario probabilities

## Capital structure update checklist (Appendix 2A / 3B / 3G / cleansing notices)

### What to extract
- **Ordinary shares on issue (quoted)**
- **Quoted options** (count, ticker, key terms if relevant)
- **Unquoted options / warrants / performance rights** (counts; any large new tranches)
- **Convertibles** (existence + any conversion/terms updates)
- **New issuance reason**: placement/employee incentives/financier fees/escrow release/etc.

### Where this gets updated
- `ANALYSIS.md` “Capital structure + dilution risk” section: update the snapshot numbers and any material new overhang.
- `announcements.md`: add the Appendix 2A/3B/3G row(s) when they are tied to a meaningful event (raise, large issuance, term reset).

## Ownership + insider activity checklist (Forms 603/604; Appendix 3X/3Y/3Z)

### What to extract
- **Substantial holder**:
  - holder name
  - effective date
  - shares and voting power (prior → after)
  - notes about derivatives/associates if disclosed
- **Director/KMP interest notices**:
  - person
  - instrument (shares/options/performance rights)
  - buy/sell/issue/expiry/transfer
  - quantity and consideration
  - context (placement participation, vesting, incentive issue)

### Where this gets updated
- `ownership.md` tables (keep them auditable, link every row to the filing).
- If insider activity is *material* (large net sell-down or large new incentive issuance), reflect it in:
  - `ANALYSIS.md` governance/dilution watch-items
  - `report.md` (only if it changes the investor lens).

## Post–first gold update template (what to look for and how to react)

### “First gold” proof points (highest signal)
When “first gold” is announced, immediately capture:
- **Date achieved** (and whether it is a “first pour” vs “commercial production” milestone)
- **Processing pathway** (toll-treatment terms/partner unchanged? any amendments?)
- **Ore delivered / processed** (tonnes; grade/recovery if disclosed)
- **Commercial terms** (who owns dore; payability; payment timing; penalties; transport/insurance)
- **Any change in schedule** for ramp and steady-state targets

### Ramp leading indicators (next 1–3 quarters)
- Evidence of **repeatability**: successive quarter-on-quarter improvement, not one-off success.
- Evidence of **grade reconciliation**: commentary on variance vs plan and reasons.
- Evidence of **cash burn compression**: operating + investing outflows down; quarters-of-funding up (or stabilising without dilution).
- Evidence of **funding discipline**: fewer discounted placements; fewer equity-linked sweeteners to financiers.

### How to update probabilities (avoid “vibes-based”)
Only change scenario probabilities in `ANALYSIS.md` when the new evidence clearly moves one of these:
- **Schedule confidence**: first gold achieved vs delayed; clear reasons and revised dates.
- **Operational quality**: throughput/grade/recovery stability vs noisy/negative commentary.
- **Funding path**: runway stabilising vs shortening; raise terms improving vs worsening.
- **Governance optics**: related-party payments trend and disclosure quality.

Document the exact evidence (filing/date) that justified the probability change.

## Changelog policy (single source of truth)
Keep **one** changelog only: `ANALYSIS.md` contains the short “since last as-of” summary entry whenever the repo is updated.

