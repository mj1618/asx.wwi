## Task: Build ASX announcement timeline + cash runway table (WWI)

### Goal
Pull the last ~24 months of ASX:WWI primary filings and turn them into a structured, cited timeline and a cash/runway + dilution risk snapshot that can be dropped into `ANALYSIS.md`.

### Why
The deep-dive outline is ready (`ANALYSIS.md` + `sources.md`). The next bottleneck is **primary-document extraction**: dates, cash balances, quarterly burn, and capital raises. Without this, any valuation or scenario probabilities will be guesswork.

### Deliverables
- Update `sources.md` with **direct links + dates** to:
  - ASX announcements feed (or search page) for WWI
  - Last 8 quarterly reports / Appendix 5B cashflow reports (minimum)
  - Any capital raise announcements + Appendix 2A share issue notices in the period
- Add a new file `announcements.md` containing an **announcement timeline table**:
  - Date (AEST), headline, category (quarterly/cap raise/project/other), key extracted numbers, and citation link
  - Cover last 24 months (or as far back as practical if the feed is constrained)
- Update `ANALYSIS.md` by filling (with citations):
  - **Latest quarter ending cash**
  - **Last 4–8 quarters**: net cash burn trend (operating + exploration/investing)
  - **Simple runway estimate** (cash / avg quarterly net outflow)
  - **Capital structure notes**: recent placements/issues, basic share count (as-of latest filing), and obvious option/warrant overhang if disclosed

### Constraints / Notes
- Use **primary sources** only for numbers (ASX PDFs, audited/half-year/quarterly filings).
- For each extracted number, include a citation in the format defined in `sources.md`.
- If ASX document links are unstable, include both the ASX landing page link and any stable PDF link you can obtain.

### Dependencies
- `001-build-initial-asx-wwi-deep-dive-outline.completed.md` (done).
- Requires web access to ASX/company filings.

### Completion notes
- Added `announcements.md` with a curated, cited timeline for the last ~24 months (quarterlies/Appendix 5B, major placements, and key project/resource updates).
- Updated `sources.md` with:
  - ASX announcements search entry point for WWI
  - Direct stable `announcements.asx.com.au/asxpdf/...` links for the last 8 quarterly/5B reports
  - Capital raise announcements and Appendix 2A/3B/3G capital structure filings (with dates and “supports” notes)
- Updated `ANALYSIS.md` with:
  - Last 8 quarters of Appendix 5B cashflow lines (operating/investing/financing + ending cash)
  - Runway estimates (including the company’s reported “estimated quarters of funding available”)
  - Capital structure snapshot (basic shares, quoted/unquoted options, warrants, performance rights) from the latest Appendix 2A

