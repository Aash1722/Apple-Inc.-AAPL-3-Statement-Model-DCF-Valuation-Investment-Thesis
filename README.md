# Apple Inc. (AAPL) — 3-Statement Model, DCF Valuation & Investment Thesis

A clean, interview-ready financial model for Apple Inc., built from primary SEC/company filings.
Model date: **21 September 2026** · Share price used: **$336.13** (18 September 2026 close).

The goal is a model that can be explained and defended in a 15–20 minute conversation, not one that
looks sophisticated. Every forecast driver sits in one place, every formula links to another cell,
and the balance sheet balances in every year.

---

## Files

| File | What it is |
|---|---|
| `Apple_3_Statement_DCF_Model.xlsx` | The model: assumptions, three linked statements, UFCF, DCF, WACC, sensitivity, valuation summary |
| `Apple_Valuation_Research_Summary_and_Interview_Guide.docx` | Research summary (business, drivers, assumptions, DCF output, risks), formula-by-formula explanations, and 28 interview Q&As |
| `Apple_AAPL_Investment_Thesis.docx` | Two-page investment thesis with a stated view, bull/bear cases, catalysts and monitorables |
| `README.md` | This file |

---

## Headline output (base case)

| Metric | Value |
|---|---:|
| PV of FY2027E–FY2031E UFCF | $569.0B |
| PV of terminal value (74% of EV) | $1,616.2B |
| Enterprise value | $2,185.2B |
| + Cash & securities / − Debt | +$146.5B / −$84.3B |
| Equity value | $2,247.4B |
| Diluted shares | 14.668B |
| **Implied share price** | **$153.22** |
| Current share price | $336.13 |
| Upside / (downside) | (54.4%) |
| WACC / terminal growth | 9.59% / 3.0% |
| Sensitivity range (WACC 8.5–10.5%, g 2.0–4.0%) | $123 – $215 |

Reverse DCF: today's price needs roughly **7% perpetual growth** at a 9.6% WACC, or a **~6.0% WACC**
at 3% growth. That gap is the analytical point of the exercise — it shows what the market is
assuming, not that the market is wrong.

---

## Workbook structure

| Tab | Contents |
|---|---|
| **Cover** | Purpose, tab index, colour code, conventions, sources |
| **Assumptions** | Every forecast driver (growth, margins, opex, tax, D&A, CapEx, SBC, working capital, capital allocation) plus market inputs for the DCF. Historical columns are calculated from the statements; forecast columns are the inputs you change |
| **Income Statement** | Revenue → gross profit → EBIT → net income, FY2022A–FY2031E, with EBITDA memo |
| **Balance Sheet** | Simplified balance sheet with a balance check row and NWC / net cash memos |
| **Cash Flow Statement** | CFO / CFI / CFF, ending cash, FCF memo, and a cash-tie check against the balance sheet |
| **UFCF** | EBIT × (1 − t) + D&A − CapEx − ΔNWC for FY2026E (base) and FY2027E–FY2031E |
| **DCF** | Discounting, Gordon Growth terminal value, EV → equity value → implied price, plus sanity checks and the reverse DCF |
| **WACC** | CAPM cost of equity, after-tax cost of debt, market-value weights |
| **Sensitivity Analysis** | Implied share price across WACC (8.5–10.5%) × terminal growth (2.0–4.0%) |
| **Valuation Summary** | One-page output, key assumptions and interpretation |

---

## Conventions

- **Colour code:** blue = hard-coded input · black = formula on the same sheet · green = link to
  another sheet · yellow fill = key assumption or key output. **Only edit blue cells.**
- **Units:** $ in billions unless a cell says otherwise. Shares in billions.
- **Fiscal year:** ends the last Saturday of September (FY2025 ended 27 Sep 2025).
- **Historical period:** FY2022A–FY2025A from audited results. **FY2026E** combines nine months
  reported (to 27 Jun 2026) with Q4 guidance — it is an estimate, not an actual.
- **Valuation date:** FY2026 year-end (26 Sep 2026), so the five discounted years are
  FY2027E–FY2031E at t = 1…5, end-of-year convention. No stub period.
- **"Cash"** means cash & equivalents *plus* current and non-current marketable securities — Apple
  manages these as one liquidity pool. The EV → equity bridge uses the **latest reported** balance
  sheet (27 Jun 2026), not a forecast balance sheet.
- **Share-based compensation** is added back in operating cash flow (non-cash) but **not** added
  back in UFCF — it is a real cost to shareholders through dilution. This is the conservative
  treatment and a good interview talking point.
- No circular interest calculation: other income/(expense) is set to zero in the forecast because
  Apple's interest income and interest expense roughly offset.

---

## Key assumptions

| Driver | Base case | Logic |
|---|---|---|
| Revenue growth | 14.6% FY26E → 6.0% FY27E → 3.5% FY31E | Tough comps after the iPhone 17 cycle, then a mature-company fade (4.6% CAGR FY26E–FY31E) |
| Gross margin | 48.7% FY26E → 47.5% FY27E → 48.5% FY31E | FY26 flattered by ~1–2pp of one-off tariff refunds; then ~25bp/yr of Services mix |
| R&D / SG&A | 9.6% / 6.2% of revenue | R&D rising with AI investment (6.7% in FY22 → 9.3% in 9M FY26) |
| Tax rate | 17.0% | 9M FY26 effective rate 17.6%; global minimum tax |
| D&A / CapEx | 2.8% / 3.0% of revenue | CapEx above D&A for AI infrastructure, so PP&E grows |
| Working capital | Held at FY2025 ratios (NWC ≈ −12.5% of revenue) | Negative NWC: growth *releases* cash |
| WACC | 9.59% | Rf 5.0% + 1.10 β × 4.25% ERP; ~98% equity-financed |
| Terminal growth | 3.0% | Long-run nominal economic growth |

**What moves the answer:** WACC ±1pp ≈ −13% / +18% · terminal growth +0.5pp ≈ +6% ·
revenue growth +1pp/yr ≈ +5% · gross margin +1pp ≈ +3% · CapEx +0.5pp ≈ −2% · tax +2pp ≈ −2%.

---

## Sources

| Input | Source |
|---|---|
| FY2022–FY2023 statements | [Apple FY23 Q4 consolidated financial statements](https://www.apple.com/newsroom/pdfs/fy2023-q4/FY23_Q4_Consolidated_Financial_Statements.pdf) |
| FY2024–FY2025 statements | [Apple FY25 Q4 consolidated financial statements](https://www.apple.com/newsroom/pdfs/fy2025-q4/FY25_Q4_Consolidated_Financial_Statements.pdf) |
| 9M FY2026 results, latest balance sheet, share count | [Apple FY26 Q3 consolidated financial statements](https://www.apple.com/newsroom/pdfs/fy2026q3/FY26_Q3_Consolidated_Financial_Statements.pdf) |
| Q4 FY2026 guidance (revenue +9–11%, GM 47–48%) | Apple Q3 FY26 earnings call, 30 July 2026 |
| Risk-free rate (~5.0%) | US Treasury / FRED series DGS10, 18–21 September 2026 |
| Equity risk premium (4.25%) | Damodaran implied US ERP, 4.23% at 1 January 2026 (damodaran.com) |
| Share price ($336.13) | Yahoo Finance, 18 September 2026 close |
| Beta (1.10) | **Estimate — verify before presenting** (see below) |

---

## Before you present it

1. **Re-check beta** on Bloomberg or Yahoo Finance (5-year monthly vs S&P 500). I could not find a
   clean current figure; 1.10 is the working assumption and it flows straight into WACC.
2. **Refresh the share price, the 10-year Treasury yield and the ERP** if more than a few days have
   passed — all three are on the Assumptions and WACC tabs.
3. **Run the checks:** `Balance Sheet` row 23 (balance check) and `Cash Flow Statement` row 30 (cash
   tie) must be zero in every year.
4. **Spot-check the history** against the filings: FY2025 revenue $416.2B, EBIT $133.1B, net income
   $112.0B, total assets $359.2B, CFO $111.5B.

## Updating after the next earnings release

1. Add the reported year as a new historical column (or replace FY2026E once the 10-K lands in
   late October 2026) and paste the actuals into the blue cells of the three statements.
2. Update the valuation inputs on **Assumptions** rows 33–47 with the new balance sheet, share
   count and market price.
3. Roll the forecast forward one year and re-check that the forecast formulas are identical across
   every projection column — a single edited cell mid-row is the most common silent error.

---

## Deliberate simplifications

Kept out on purpose, and worth naming if asked "what would you improve?":

- End-of-year discounting rather than mid-year convention (mid-year would add roughly 5%).
- Company-wide revenue forecast, not a segment build (iPhone vs Services).
- No debt schedule, no deferred tax schedule, no scenario toggles, no macros or VBA.
- Other non-current assets and liabilities held flat.
- Trading comps omitted: I did not have reliable current multiples for Microsoft, Alphabet and Meta,
  and an unsourced comps table is worse than none.

---

*Prepared as an analytical and interview-preparation exercise from public filings. Not investment
advice.*
