# Peer comps + relative valuation — ASX:WWI (West Wits Mining)

> Not financial advice. Working notes intended to be **directional**, not “precision theatre”.

## Method + caveats

### Market cap / EV snapshot (secondary)
- **Market cap source**: TradingView “Key stats” **market capitalisation** for each ticker — *as-of 2026-02-02* (secondary market-data snapshot).
- **EV**: where **net cash / net debt** was not readily available from a primary filing within this task, EV is shown as an **EV proxy** (\(\approx\) market cap). If net cash / debt is available, EV proxy adjusts for it.

### Technical metrics (prefer primary)
- For **resources/reserves/grades**, prefer **JORC / annual report / ASX announcement PDFs**.
- For **study economics (NPV/IRR/AISC)**, prefer **ASX technical releases**; company website summaries are used where primary docs were inaccessible in-session.

### “Apples-to-apples” warnings (read before using multiples)
- **EV/oz (Resource)** is highly sensitive to **resource quality** (category, depth, metallurgy, mining method, strip ratio, recovery, capex intensity) and is often **misleading** across different deposit styles.
- **EV/oz (Reserve)** is more “apples-to-apples” but still sensitive to **margin** (AISC), **mine life**, and **jurisdiction discount**.
- **EV/NPV** is only comparable when the **discount rate, gold price deck, ownership %, and included resource categories** are aligned. Treat cross-company EV/NPV as a **rough** triangulation only.

## Peer set selection (11 peers)

### Bucket A — AU-listed gold developers / new producers (near first gold / early ramp)
- **BGL (Bellevue Gold)**: underground, high-grade, early producer; useful “quality producer” multiple anchor.
- **MEK (Meeka Metals)**: developer→producer transition with published DFS economics and a large-share-count cap-structure (dilution lens).
- **OBM (Ora Banda)**: WA producer / ramp story; useful for “ramp + capital discipline” comparison.
- **STN (Saturn Metals)**: open-pit / heap-leach style development path; useful low-grade bulk tonnage reference.
- **GMD (Genesis Minerals)**: consolidation-driven developer/producer build-out; included as a large-cap “developer rerate” example (technical metrics not captured in this pass).

### Bucket B — AU-listed gold exposure in South Africa / Sub‑Saharan Africa (jurisdiction discount lens)
- **TGM (Theta Gold Mines)**: South Africa developer with **BEE ownership** complexity (good jurisdiction + structure analogue to WWI).
- **WAF (West African Resources)**: Burkina Faso producer; good “SSA but de-risked producer” anchor.
- **PRU (Perseus Mining)**: multi-mine West Africa producer; “self-funding” counterexample vs serial raisers.
- **RSG (Resolute Mining)**: Africa-focused producer + developer pipeline; Doropo DFS provides a project-NPV reference.

### Bucket C — Cap-structure lens (serial raisers vs self-funders)
- **High dilution / frequent capital activity tends to depress EV/NPV convergence** even when the asset is “good”.
- Use **TGM / MEK / WWI** as the “dilution + funding risk” lens vs **PRU / CMM** as “self-funding / balance sheet strength” lens.

## Comps table (snapshot)

**Units**: market cap / EV proxy in **A$ million**, resources/reserves in **Moz Au**.  
**Market cap source** (all rows): TradingView “Market capitalization” — *2026-02-02*.

| Ticker | Company | Stage | Jurisdiction(s) | Market cap (A$m) | EV proxy (A$m) | Resource (Moz @ grade) | Reserve (Moz @ grade) | Key study / cost metric (if published) | Multiples (EV/oz; EV/NPV) | Sources |
|---|---|---|---|---:|---:|---|---|---|---|---|
| **WWI** | West Wits Mining | developer → first gold (target Mar 2026) | South Africa (WBP/Qala), Australia (Mt Cecilia) | ~351.6 | ~348.0 | **Attrib**: 5.36 (74% × 7.244Moz @ 4.0g/t) | **Attrib**: 0.284 (74% × 0.384Moz reserve) | DFS anchor: **post‑tax NPV7.5 = US$500m** (All Resources; includes Inferred); AISC **US$1,289/oz** (DFS) | EV/Res **~A$65/oz** (attrib); EV/Resv **~A$1,225/oz** (attrib); EV/NPV7.5 **~0.66** (before haircuts) | `valuation.md` + `ANALYSIS.md` (repo primary/secondary citations) |
| **BGL** | Bellevue Gold | early producer | Australia (WA) | 2,790 | 2,738 | 3.10 @ 8.9 g/t | 1.29 @ 4.7 g/t | FY25 AISC **A$2,422/oz**; cash **A$151.6m**, bank debt **A$100m** (net cash ~A$51.6m) | EV/Res **~A$883/oz**; EV/Resv **~A$2,123/oz** | **[Annual Report 2025](https://bellevuegold.com.au/wp-content/uploads/2025/08/Annual-Report-2025.pdf)** — 2025-08; **[TradingView BGL](https://www.tradingview.com/symbols/ASX-BGL/)** — 2026-02-02 |
| **OBM** | Ora Banda Mining | producer / ramp | Australia (WA) | 2,230 | 2,230 | 2.00 @ 2.5 g/t | 0.276 @ 1.9 g/t | DFS exists (site states DFS dated 30 Jun 2020); metrics not captured in this pass | EV/Res **~A$1,115/oz**; EV/Resv **~A$8,080/oz** *(flag: verify market cap / net debt; this looks like an outlier)* | **[OBM homepage](https://orabandamining.com.au/)** — 2026-02-02; **[TradingView OBM](https://www.tradingview.com/symbols/ASX-OBM/)** — 2026-02-02 |
| **CMM** | Capricorn Metals | producer | Australia (WA) | 6,750 | 6,750 | 6.6 (total resources) | 4.0 (reserves) | Producer (Karlawinda); project metrics not captured in this pass | EV/Res **~A$1,023/oz**; EV/Resv **~A$1,688/oz** | **[CMM homepage](https://capmetals.com.au/)** — 2026-02-02; **[TradingView CMM](https://www.tradingview.com/symbols/ASX-CMM/)** — 2026-02-02 |
| **PRU** | Perseus Mining | producer (multi-mine) | Ghana, Côte d’Ivoire (+dev Tanzania) | 8,160 | 8,160 | 7.8 (M&I resources, 30 Jun 2025) | 5.0 (P&P reserves, 30 Jun 2025) | FY25 AISC **US$1,235/oz** | EV/Res **~A$1,046/oz**; EV/Resv **~A$1,632/oz** | **[PRU operations](https://perseusmining.com/our-operations/)** — 2026-02-02; **[TradingView PRU](https://www.tradingview.com/symbols/ASX-PRU/)** — 2026-02-02 |
| **WAF** | West African Resources | producer | Burkina Faso | 4,220 | 4,220 | 12.8 (resources) | 6.1 (ore reserves) | Website-stated 10y plan + peak production; detailed metrics not captured in this pass | EV/Res **~A$330/oz**; EV/Resv **~A$692/oz** | **[WAF homepage](https://www.westafricanresources.com/)** — 2026-02-02; **[TradingView WAF](https://www.tradingview.com/symbols/ASX-WAF/)** — 2026-02-02 |
| **RSG** | Resolute Mining | producer + dev pipeline | Mali, Senegal (+dev Côte d’Ivoire) | 2,790 | ~2,596 *(mcap less net cash disclosure)* | — | Doropo ore reserve: 2.50Moz @ 1.31 g/t (project, 100% basis) | Doropo DFS: post-tax **NPV5% US$1.457bn**, IRR **49%**, AISC **~US$1,406/oz** (project, 100% basis). Net cash **US$136.6m** (company, end Q3). | EV/Resv (Doropo) **~A$1,038/oz**; EV/NPV5 (Doropo, USD→AUD @1.42) **~1.25** *(not apples-to-apples; company has other assets)* | **[Doropo DFS Update](https://www.rml.com.au/wp-content/uploads/2025/12/20251215-RSG-ASX-Doropo-DFS-Update.pdf)** — 2025-12-15; **[TradingView RSG](https://www.tradingview.com/symbols/ASX-RSG/)** — 2026-02-02 |
| **TGM** | Theta Gold Mines | developer | South Africa | 219.78 | 219.78 | \~6.1 (company-stated) | FS “ore reserve plan” references 514koz (plan basis; see FS) | FS announcement reported NPV/IRR/AISC, but company subsequently issued a **retraction** warning investors not to rely on the base-case target/forecast financial information. Treat any EV/NPV from this FS as **unreliable** until replaced by a compliant update. | EV/Res **~A$36/oz** | **[Optimised FS announcement](https://announcements.asx.com.au/asxpdf/20250930/pdf/06py58b65624xd.pdf)** — 2025-09-30; **[Funding + retraction note](https://announcements.asx.com.au/asxpdf/20251007/pdf/06q716kbl7m10v.pdf)** — 2025-10-07; **[TGM site](https://thetagoldmines.com/)** — 2026-02-02; **[TradingView TGM](https://www.tradingview.com/symbols/ASX-TGM/)** — 2026-02-02 |
| **STN** | Saturn Metals | developer (PFS in progress) | Australia (WA) | 248.43 | 248.43 | 2.239 @ 0.51 g/t (Apollo Hill) | — | PFS + inaugural reserve targeted late CY2025 (per update) | EV/Res **~A$111/oz** | **[Apollo Hill MRE update](https://saturnmetals.com.au/wp-content/uploads/2025/07/250718-Apollo-Hill-Gold-Resource-Update-July-2025-2.24Moz.pdf)** — 2025-07-18; **[TradingView STN](https://www.tradingview.com/symbols/ASX-STN/)** — 2026-02-02 |
| **MEK** | Meeka Metals | developer → producer (first gold Jul 2025) | Australia (WA) | 692.28 | 692.28 | 1.2 @ 3.0 g/t (Murchison) | — | DFS2.0 (Dec 2024): NPV8% **A$616m**, IRR **180%**, FCF **A$1b** (website-stated; primary PDF link timed out in-session) | EV/Res **~A$577/oz**; EV/NPV8 **~1.12** *(treat cautiously until primary DFS PDF captured)* | **[MEK site](https://meekametals.com.au/)** — 2026-02-02; **[TradingView MEK](https://www.tradingview.com/symbols/ASX-MEK/)** — 2026-02-02 |
| **RMS** | Ramelius Resources | producer | Australia (WA) | 9,090 | 9,090 | 12.0 @ 1.8 g/t *(Total Mineral Resources, 30 Jun 2025)* | 2.4 @ 1.3 g/t *(Total Ore Reserves, 30 Jun 2025)* | Resources & Reserves Statement (FY25) | EV/Res **~A$758/oz**; EV/Resv **~A$3,788/oz** | **[Resources & Reserves Statement 2025](https://www.rameliusresources.com.au/wp-content/uploads/bsk-pdf-manager/2025/10/2025-Resources-and-Reserves-Statement.pdf)** — 2025-10-01; **[TradingView RMS](https://www.tradingview.com/symbols/ASX-RMS/)** — 2026-02-02 |
| **GMD** | Genesis Minerals | developer/producer build-out | Australia (WA) | 4,940 | 4,940 | 14.7 @ 2.2 g/t *(Group total resources)* | 3.7 @ 2.1 g/t *(Group total reserves)* | Resources & Reserves Statement (Apr 2025) | EV/Res **~A$336/oz**; EV/Resv **~A$1,335/oz** | **[Reserves rise to 3.7Moz underpinning ASPIRE 400 strategy](https://gmd.live.irmau.com/pdf/bed52b2a-c39d-4921-97a4-05a96d96ddb8/Reserves-rise-to-37Moz-underpinning-ASPIRE-400-strategy.pdf)** — 2025-04; **[TradingView GMD](https://www.tradingview.com/symbols/ASX-GMD/)** — 2026-02-02 |

## Takeaways for WWI (relative valuation lens)

- **Resource-scale EV/oz can look “cheap” for WWI** if you use the global WBP resource (especially including Inferred), because ounces are large. The **more honest cross-check** is whether those ounces are **convertible** (reserve + schedule + funding + jurisdiction + dilution).
- **Reserve-based EV/oz** puts WWI closer to producer-like territory (because the reserve is small vs EV), which is consistent with the market saying: “we’ll pay for near-term ounces, not the whole 7.24Moz story yet.”
- **Jurisdiction + cap-structure matters**: South Africa developers (e.g. TGM) can trade at very low EV/oz until financing + permitting + construction credibility are clear; WWI’s repeated equity issuance and large option/warrant stack increases the “developer discount”.

