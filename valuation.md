# Valuation (working notes) — ASX:WWI (West Wits Mining)

> Not financial advice. This is a transparent, assumption-driven research note.

## 1) Key valuation anchor (primary source)

WWI published an updated DFS for Qala Shallows (part of WBP) on **2025-07-23**.

From the **Base Case (All Mineral Resources; includes Inferred)** the DFS reports:
- **Post-tax NPV7.5**: **US$500m**
- **Post-tax IRR**: **81%**
- **Peak funding**: **US$44m**
- **LOM AISC**: **US$1,289/oz**
- **Gold price deck** (Bloomberg consensus for first 3 years; long-term **US$2,850/oz**)
- **Gold-price sensitivity (post-tax NPV7.5)**: **US$194m @ US$1,850/oz** up to **US$1,111m @ US$4,850/oz**

Primary source:
- **[Updates to Qala Shallows DFS provide improved results for Witwatersrand Basin Project](https://announcements.asx.com.au/asxpdf/20250723/pdf/06m1rzxy01hc14.pdf)** — *2025-07-23*

## 2) Ownership adjustment (project → WWI attributable)

WWI’s disclosed interest in WBP tenements is **74%** (local minority held by Lilitha Resources Pty Ltd).

Primary source:
- **[Quarterly Activity Report (Reporting Period 1 October – 31 December 2025) + Appendix 5B](https://announcements.asx.com.au/asxpdf/20260123/pdf/06vj8v3nlt4skk.pdf)** — *2026-01-23*

So an “attributable NPV” estimate (before any corporate-level adjustments) is:

\[
\text{Attributable NPV (USD)} \approx 0.74 \times 500m = 370m
\]

## 3) FX conversion (USD → AUD)

For a spot-style conversion (used only to express results in AUD per share), use:
- AUD/USD ≈ **0.7043** (so USD→AUD ≈ **1 / 0.7043 = 1.42**)

Secondary source:
- **[Google Finance — AUD/USD](https://www.google.com/finance/quote/AUD-USD)** — *2026-02-02*

So:

\[
370m\ \text{USD} \times 1.42 \approx 525m\ \text{AUD}
\]

## 4) Per-share denominator (basic vs fully diluted)

Basic shares on issue (quoted ordinary) as at **2026-01-27**:
- **4,319,419,767**

Dilutive instruments disclosed on the same date (counts only; strike/expiry vary by class):
- Quoted options: 319,597,085
- Unquoted options: 171,088,599
- Unquoted warrants: 166,933,764
- Performance rights: 5,000,000
- (Convertible notes exist; conversion outcomes are not fully captured in this simple tally)

Primary source:
- **[Appendix 2A - Application for quotation of securities (WWI ordinary shares)](https://announcements.asx.com.au/asxpdf/20260127/pdf/06vlw4ggk8lrk8.pdf)** — *2026-01-27*

A simple “fully diluted (ex-CNs)” share count is:

\[
4.319b + 0.320b + 0.171b + 0.167b + 0.005b \approx 4.982b
\]

## 5) What the simple NPV-per-share implies (not risk-adjusted)

If you naively capitalise the DFS post-tax NPV7.5 (All Resources) as “equity value” (it’s closer to a project value anchor and omits many real-world frictions), you get:

- **Basic**: \(525m\ AUD / 4.319b \approx 0.122\ AUD/share\)
- **FD (ex-CNs)**: \(525m\ AUD / 4.982b \approx 0.105\ AUD/share\)

This is **not** a prediction; it’s a sanity-check anchor to compare against market price once you apply:
- execution / schedule risk (first gold + ramp)
- financing structure (debt service and covenants)
- further dilution (if ramp-up underdelivers)
- jurisdictional / permitting / social licence risk
- the fact that DFS “All Resources” case includes Inferred resources (explicitly flagged in the DFS)

## 6) Scenario ranges used in `ANALYSIS.md`

To avoid “precision theatre”, the scenario valuation in `ANALYSIS.md`:
- uses the DFS NPV7.5 as the *starting* anchor,
- applies **wide haircut ranges** for “market discount to NPV” depending on de-risking state,
- and models **share count expansion** (dilution) as a first-class driver of per-share outcomes.

Secondary market snapshot used only for context:
- **[Google Finance — ASX:WWI quote](https://www.google.com/finance/quote/WWI:ASX)** — *2026-02-02*

## 7) Peer multiples cross-check (sanity check)

This is a **triangulation tool**, not a standalone valuation method. See `peers.md` for the peer list, sources, and caveats.

### WWI quick multiples (as-of the repo’s current snapshot)
- **EV (proxy)**: \(\approx\) market cap + debt − cash \(\approx 351.6 + 18.7 - 22.2 \approx A\$348m\) (cash/debt per Dec 2025 quarterly; market cap per Google Finance snapshot).
- **EV / attributable global resource (JORC MRE)**: \(\approx A\$348m / (0.74 \times 7.244Moz) \approx A\$65/oz\).
- **EV / attributable DFS reserve**: \(\approx A\$348m / (0.74 \times 384koz) \approx A\$1,225/oz\).
- **EV / attributable DFS NPV7.5 (headline)**: \(\approx A\$348m / A\$525m \approx 0.66\).

### How to interpret the peer cross-check for WWI
- Treat **EV/oz (Resource)** as a **discount-to-conversion** signal (how much the market doubts conversion to cashflow), not “cheapness”.
- Treat **EV/oz (Reserve)** as the “near-term cashflow credibility” signal (how much the market is paying for *mineable ounces*).
- For WWI, the practical question is whether a **producer rerate** (higher EV/NPV) happens *before* dilution dominates per-share outcomes; this is tightly linked to **first gold + ramp** and **funding strategy**.

