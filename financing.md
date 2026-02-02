# Financing + dilution mechanics (convertibles + facilities) — ASX:WWI

*As-of date for this repo snapshot: **2026-02-02***  
*Not financial advice. This is a mechanical extraction of disclosed terms with explicit “unknowns”.*

## 1) What this file covers (and what it doesn’t)

This file documents (with primary-source links) the **equity-linked** parts of WWI’s financing stack that can change per‑share outcomes:

- **Convertible notes** (conversion formula → shares)
- **Facilities/loans** where **warrants/options** are issued to lenders (equity-linked sweeteners)

It intentionally avoids “interpretation” and focuses on auditable terms. For valuation impact, see `valuation.md`.

## 2) Convertible notes (CN) — terms + conversion mechanics

### 2.1 Summary (high-signal)

- WWI disclosed **A$1.5m** convertible note financing in the Sep 2024 quarter, with each note **A$25,000** face value.
- Conversion is **holder‑elected** with a price that is either **A$0.02** or (post 17 Jan 2025) **80% of the 15‑day VWAP**, whichever is lower.
- Notes are described as **unsecured** and (in later 5B text) **interest free**, with **unlisted options issued in lieu of interest**.
- By the Dec 2025 quarter filing, WWI disclosed that **A$1.45m** of CNs had been converted to ordinary shares prior to the reporting date, leaving **A$50k** (2 notes) outstanding.

Primary sources:
- **[Quarterly Activity Report (Reporting Period 1 July – 30 September 2024) + Appendix 5B](https://announcements.asx.com.au/asxpdf/20241029/pdf/069qs5cqm29q1b.pdf)** — *2024-10-29*
- **[Quarterly Activities and Cashflow Reports (Reporting Period 1 April – 30 June 2025) + Appendix 5B](https://announcements.asx.com.au/asxpdf/20250728/pdf/06m6tpt15hlnml.pdf)** — *2025-07-28*
- **[Quarterly Activities and Cashflow Reports (Reporting Period 1 July – 30 September 2025) + Appendix 5B](https://announcements.asx.com.au/asxpdf/20251029/pdf/06r62jp33jfwb3.pdf)** — *2025-10-29*
- **[Quarterly Activity Report (Reporting Period 1 October – 31 December 2025) + Appendix 5B](https://announcements.asx.com.au/asxpdf/20260123/pdf/06vj8v3nlt4skk.pdf)** — *2026-01-23*
- **[Appendix 2A - Application for quotation of securities (post-placement capital snapshot)](https://announcements.asx.com.au/asxpdf/20260127/pdf/06vlw4ggk8lrk8.pdf)** — *2026-01-27*

### 2.2 Convertible notes table (auditable)

| Instrument | Disclosed face value | Count / status (as disclosed) | Conversion price / formula | Maturity | Interest / fees | Equity sweetener | Security | Primary source |
|---|---:|---|---|---|---|---|---|---|
| Convertible notes (WWI) | A$1.5m total; **A$25k per note** | **58 CNs** referenced in later 5B narrative; **A$1.45m converted prior to 31 Dec 2025**; **A$50k outstanding (2 CNs)** | **A$0.02** until **17 Jan 2025**; thereafter **min(A$0.02, 0.8 × 15‑day VWAP)**; conversion at election of noteholder | **16 Oct 2026** | Described as **interest free** (later 5B); earlier text describes options “in lieu of interest” | **25 unlisted options per A$1 subscribed**; total **37.5m** options; exercise **A$0.023**; expiry **36 months from issue date** | Unsecured | Sep 2024 quarterly + 5B (issue + formula + options); Jun 2025 / Sep 2025 / Dec 2025 quarterlies + 5B (maturity + conversions/outstanding) |

Notes:
- The **exact conversion date(s)** and **exact VWAP inputs** for each conversion are not fully enumerated in the quarterly narrative; only some conversion outcomes are disclosed (e.g., Sep 2025 quarter).
- The repo treats the **remaining CN dilution** as small as of the latest captured quarter because only **A$50k** remained outstanding (see Section 2.3).

### 2.3 CN conversion → shares (mechanics)

Given principal \(P\) and conversion price \(C\), shares issued on conversion are:

\[
\text{Shares} = P / C
\]

For the **remaining disclosed principal** (A$50,000 outstanding as at 31 Dec 2025 quarter-end):

| Scenario | Assumed conversion price | Implied new shares (A$50k / price) | Notes |
|---|---:|---:|---|
| Cap price | A$0.0200 | **2,500,000** | Price cap applies if \(0.8\times\)VWAP \(\ge\) A$0.02 |
| Discounted example | A$0.0170 | **2,941,176** | Illustrative price consistent with “discounted to VWAP” mechanics disclosed in Sep 2025 quarter narrative |

## 3) Facilities / loans — terms + equity-linked sweeteners

### 3.1 Facilities table (auditable)

| Provider / instrument | Type | Size (headline) | Drawn / timing (as disclosed) | Interest | Tenor / maturity | Key security / covenants (only if disclosed) | Equity-linked features | Primary source |
|---|---|---:|---|---|---|---|---|---|
| IDC + Absa | Senior syndicated project loan facility (South Africa) | **ZAR 875m** (~US$50m) | Drawdown progressive (per announcement); facility documents executed | Variable, linked to **JIBAR** | Total tenor **~5 years** (24m availability then 36m repayment) | Not detailed in announcement | **Absa received options in lieu of fees** (see next row) | **[West Wits signs senior loan facility agreements for ZAR 875M](https://announcements.asx.com.au/asxpdf/20250630/pdf/06l7ykg0762w1j.pdf)** — *2025-06-30* |
| Absa Bank Limited | Fee settlement equity | N/A | Issued Nov 2025 to settle **ZAR 7,656,250** fees (~A$680k) | N/A | Options expire **5 years** from issue | N/A | **100,386,000 unlisted options**, strike **A$0.0185** | **[Senior Bank Lender Takes Options in Lieu of Fees](https://announcements.asx.com.au/asxpdf/20251110/pdf/06rqg7sxcfljv1.pdf)** — *2025-11-10* |
| Nebari Natural Resources Credit Fund II LP | Debt facility (scalable; Tranches 1–3) | **US$35.0m** total; **US$12.5m** Tranche 1 | Tranche 1 drawn down **Nov 2025** | **3m SOFR (min 4%) + 8.5% p.a.** | **48 months** from each tranche drawdown | First-ranking fixed & floating security over WWI + SA subs (as described) | **Warrants equal to 35% of principal / strike** (see Section 3.2) | **[WWI Signs Agreements for USD 12.5M Loan Facility](https://announcements.asx.com.au/asxpdf/20250929/pdf/06pszf4qwx7k6k.pdf)** — *2025-09-29*; **[Quarterly (Dec 2025) + 5B](https://announcements.asx.com.au/asxpdf/20260123/pdf/06vj8v3nlt4skk.pdf)** — *2026-01-23* |
| WWI “Interim Loan” (lender not named in 5B narrative) | Short-term loan | **A$550k** | **A$450k** advanced by 30 Jun 2025 quarter-end | **10% p.a.** (capitalised) | **6 months** | Unsecured | Company-elected repayment **in cash or shares @ A$0.022** | **[Quarterly (Jun 2025) + 5B](https://announcements.asx.com.au/asxpdf/20250728/pdf/06m6tpt15hlnml.pdf)** — *2025-07-28* |

### 3.2 Nebari warrants — mechanics + dilution

Per the Nebari facility announcement, warrants are issued on funding of each tranche, with:

- **Warrant count**: \(\text{Warrants} = 35\% \times \text{principal} / \text{strike}\)
- **Strike**: **30% premium** to a defined “Base Price” reference (see Annexure B in the 2025-09-29 announcement; tranche‑specific VWAP references)
- **Term**: **4 years** from issuance (each tranche)

Tranche 1 drawdown disclosure:
- On Tranche 1 drawdown, WWI disclosed it would issue **166,933,764 warrants** to Nebari (via Nebari Partners GP III LLC as GP).
- The Dec 2025 quarterly later discloses these warrants had an exercise price of **US$0.0288** and a **four-year term**.

Primary sources:
- **[WWI Signs Agreements for USD 12.5M Loan Facility](https://announcements.asx.com.au/asxpdf/20250929/pdf/06pszf4qwx7k6k.pdf)** — *2025-09-29* (facility + warrant terms annexures)
- **[Issue of Facility Drawdown Notice to Nebari](https://announcements.asx.com.au/asxpdf/20251117/pdf/06s27367gxhymy.pdf)** — *2025-11-17* (Tranche 1 drawdown notice; warrant count)
- **[Quarterly (Dec 2025) + 5B](https://announcements.asx.com.au/asxpdf/20260123/pdf/06vj8v3nlt4skk.pdf)** — *2026-01-23* (exercise price disclosure; confirms tranche drawdown timing)

## 4) How this flows into “fully diluted” share counts

- The repo’s **“FD ex‑CNs”** share count already includes the **options** and **warrants** disclosed in Appendix 2A (quoted options + unquoted options + unquoted warrants + performance rights).
- The **incremental missing piece** was the **CN conversion shares**, which (as of the latest quarter captured) are small because only **A$50k** remained outstanding.

For the valuation denominator updates, see `valuation.md` (section on per-share denominators).

