# HUL Forecast vs Actual Variance Analysis and DCF Valuation

I built this as a self-study project to practise FP&A work on a real company. It uses only public data from Hindustan Unilever's annual reports.

![HUL FY2026 Forecast vs Actual](chart.png)

## Part 1: FY2026 forecast vs actual

I forecast HUL's FY2026 revenue and EBITDA using only FY2022 to FY2025 data, then compared it with what HUL actually reported for FY2026 and worked out the variances.

How I did it:
- Revenue: I grew each of the four segments (Home Care, Beauty & Personal Care, Foods, Others) at its average growth rate for FY2023 to FY2025.
- Costs: I used the FY2022 to FY2025 average operating cost as a percentage of revenue.
- EBITDA is revenue minus operating costs.
- Variance is actual minus forecast, in rupees and percent, marked favourable or unfavourable.

A few things I had to handle:
- Beauty & Wellbeing and Personal Care were one segment until FY2024, so I combined them for all years.
- HUL restated FY2025 in its FY2026 report because of the Ice Cream demerger, so my forecast starts from the restated figure.
- All figures are standalone, in Rs crore, and I checked them against the totals printed in the reports.

Result: EBITDA came in about 3.8% (Rs 567 crore) below my forecast. Most of that was lower revenue, mainly in Home Care. HUL says price reductions earlier in the year held back Home Care sales growth.

## Part 2: FY2027 forecast and DCF

After that I forecast FY2027 the same way and built a DCF on top of it.

- Free cash flow for FY2027 to FY2031 is EBITDA less depreciation, tax and capex, adjusted for working capital. I worked out working capital from receivable, inventory and payable days on the FY2026 balance sheet.
- The discount rate comes from CAPM: risk-free rate, beta and the India equity risk premium. HUL's only debt is lease liabilities.
- For terminal value I used 5% growth, the same rate HUL uses in its own impairment testing.
- There is also a sensitivity table showing value per share for different discount rates and terminal growth rates.

I ran two cases:
- Base case: growth rises evenly from 2.6% in FY2027 to 5.0% in FY2031.
- Higher-growth case: 8% a year, which is the middle of the 7% to 9% growth HUL assumes for its main segments in its impairment note. This is just an illustration, not company guidance.

The base case gives about Rs 657 per share and the higher-growth case about Rs 793. The share price was Rs 1,977 on 4 November 2026, so both are well below it. The market is paying about 32 times EBITDA for HUL, while my terminal value works out to about 11 times. So my numbers are cautious, and I don't read this as the share being overpriced.

## Limitations
- Public data only. I had no internal budget or management guidance.
- The 3-year average growth includes an unusually strong FY2023.
- The DCF is simple. I kept capex and depreciation at their FY2026 share of revenue, and the result depends a lot on the discount rate and terminal growth.

## Files
HUL_FY26_Forecast_vs_Actual.xlsx` has everything: Summary, Data, Forecast, Variance, Forecast FY27, DCF, DCF High Growth and Valuation Summary.

## Sources
HUL annual reports FY2022-23 to FY2025-26 (financials, tax rate, growth and terminal growth assumptions), CCIL (10-year government bond yield, 3 Nov 2026), Aswath Damodaran (India equity risk premium and default spread), TopStockResearch (beta), Moneycontrol (share price, 4 Nov 2026).
