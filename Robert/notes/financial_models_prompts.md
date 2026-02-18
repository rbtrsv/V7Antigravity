# Financial Models Prompts — Reference Guide

> Source: `Robert/Financial Models Prompts/` (images 1.png–6.png)
> Author of original prompts: ABI Bouhmaida (@forgoodcode)
> Note: Prompt #5 is missing from the source images. The collection jumps from #4 to #6.

---

## Table of Contents

1. [DCF Valuation Model](#1-dcf-valuation-model)
2. [Three-Statement Financial Model](#2-three-statement-financial-model)
3. [LBO (Leveraged Buyout) Model](#3-lbo-leveraged-buyout-model)
4. [Comparable Company Analysis (Comps)](#4-comparable-company-analysis-comps)
5. [Credit Analysis & Debt Capacity Model](#5-credit-analysis--debt-capacity-model)
6. [Investment Committee Memo](#6-investment-committee-memo)

---

## 1. DCF Valuation Model

**Role:** Senior Analyst at Goldman Sachs
**Objective:** Build a complete Discounted Cash Flow valuation model for a target company.
**Output Format:** Investment banking pitch book valuation page with clear formulas.

### What to Provide

- **Free cash flow projections:** Next 5 years with growth assumptions
- **WACC calculation:** Cost of equity + cost of debt breakdown
- **Terminal value:** Both perpetuity growth and exit multiple methods
- **Sensitivity analysis:** How value changes with different assumptions
- **Discount rate justification:** Why this specific WACC was chosen
- **Key drivers:** What makes cash flow go up or down
- **Comparable companies:** How assumptions compare to peers
- **Valuation range:** Bull case, base case, bear case scenarios

### Input Required

> Company: [DESCRIBE COMPANY, INDUSTRY, FINANCIALS]

### What This Model Does

The DCF model estimates the intrinsic value of a company by projecting its future free cash flows and discounting them back to present value using the Weighted Average Cost of Capital (WACC). It is the foundational valuation methodology in investment banking and equity research. The sensitivity analysis and scenario ranges (bull/base/bear) provide a valuation corridor rather than a single point estimate, which is how real pitch books present valuations.

---

## 2. Three-Statement Financial Model

**Role:** VP at Morgan Stanley
**Objective:** Build a complete three-statement model for a target company.
**Output Format:** Excel-style model with formulas explained in plain English.

### What to Provide

- **Income statement:** Revenue, costs, EBITDA, net income (5 years)
- **Balance sheet:** Assets, liabilities, equity (5 years)
- **Cash flow statement:** Operating, investing, financing activities (5 years)
- **Link formulas:** How statements connect (net income → cash flow → balance sheet)
- **Working capital:** How AR, inventory, and AP change
- **Debt schedule:** Principal payments and interest expense
- **Key assumptions:** Revenue growth, margins, capex as % of sales
- **Error checks:** Balance sheet balancing and circular references

### Input Required

> Company: [DESCRIBE BUSINESS, CURRENT FINANCIALS, GROWTH STAGE]

### What This Model Does

The three-statement model is the backbone of all financial modeling. It links the income statement, balance sheet, and cash flow statement into a single integrated model where changes in one statement flow through to the others. The circular references (e.g., interest expense depends on debt balance, which depends on cash flow, which depends on interest expense) are a core challenge. This model serves as the foundation on top of which DCFs, LBOs, and M&A models are built.

---

## 3. LBO (Leveraged Buyout) Model

**Role:** Private Equity Associate at KKR
**Objective:** Build a complete LBO model for a target company.
**Output Format:** Private equity investment committee memo with returns analysis.

### What to Provide

- **Sources and uses:** How deal is funded (debt, equity, fees)
- **Debt structure:** Senior debt, mezzanine, interest rates, covenants
- **Cash flow sweep:** How excess cash pays down debt
- **Exit scenarios:** Strategic sale vs. IPO in year 5
- **IRR calculation:** Internal rate of return for equity investors
- **Cash-on-cash multiple:** Total proceeds divided by equity invested
- **Debt paydown schedule:** Year-by-year principal reduction
- **Management assumptions:** EBITDA growth and margin improvement

### Input Required

> Company: [DESCRIBE COMPANY, EBITDA, ASKING PRICE, INDUSTRY]

### What This Model Does

The LBO model is the primary tool used by private equity firms to evaluate acquisition targets. It models how a company is acquired using a combination of debt and equity, how the debt is paid down over the holding period using the company's own cash flows, and what returns the equity investors achieve upon exit. The two key return metrics are IRR (time-weighted return) and cash-on-cash multiple (money multiple). The debt structure (senior, mezzanine, etc.) determines the risk/return profile and the cash flow sweep mechanics determine how quickly leverage is reduced.

---

## 4. Comparable Company Analysis (Comps)

**Role:** Equity Research Analyst at Citi
**Objective:** Build a trading comps analysis for a target company.
**Output Format:** Comparable company valuation table with multiples highlighted.

### What to Provide

- **Peer group:** 10–15 public companies in the same industry
- **Trading multiples:** EV/EBITDA, EV/Revenue, P/E for each peer
- **Financial metrics:** Revenue, EBITDA, margins for comparison
- **Valuation range:** 25th percentile, median, 75th percentile multiples
- **Implied valuation:** What the target company is worth at each multiple
- **Adjustments:** Why the company deserves a premium or discount
- **Growth comparison:** How the target's growth compares to peers
- **Quality screen:** Which peers are most comparable and why

### Input Required

> Company: [DESCRIBE COMPANY, FINANCIALS, CLOSEST COMPETITORS]

### What This Model Does

Comparable company analysis (comps) is a relative valuation method. Instead of estimating intrinsic value from cash flows (like DCF), it values a company by looking at what the market is paying for similar companies. The key multiples (EV/EBITDA, EV/Revenue, P/E) provide different lenses — EV-based multiples are capital-structure neutral, while P/E reflects equity value directly. The percentile ranges and quality screening ensure the valuation isn't distorted by outliers or non-comparable peers. Premium/discount adjustments account for differences in growth, margins, market position, or risk.

---

## 5. Credit Analysis & Debt Capacity Model

**Role:** Leveraged Finance Banker at Credit Suisse
**Objective:** Build a debt capacity analysis for a target company.
**Output Format:** Credit memo with debt capacity recommendation.

### What to Provide

- **EBITDA analysis:** Last 3 years and next 3 years projected
- **Leverage ratios:** Total Debt/EBITDA industry standards
- **Interest coverage:** EBITDA/Interest expense minimum thresholds
- **Debt structure:** Senior secured, unsecured, subordinated layers
- **Covenants:** Financial maintenance tests (leverage, coverage)
- **Maximum debt:** How much company can borrow responsibly
- **Pricing grid:** Interest rates at different leverage levels
- **Refinancing analysis:** When existing debt matures and needs rollover

### Input Required

> Company: [DESCRIBE COMPANY, CURRENT DEBT, EBITDA, INDUSTRY]

### What This Model Does

The credit analysis model evaluates a company from the lender's perspective — not "what is this company worth?" but "how much can this company safely borrow?" It analyzes the company's cash flow stability, existing leverage, and industry benchmarks to determine maximum debt capacity. The debt structure (senior secured vs. subordinated) reflects the priority of claims — senior secured lenders get paid first, so they accept lower rates. Covenants are contractual safeguards that trigger action if the company's financial health deteriorates (e.g., if leverage exceeds 4.0x, the borrower must take corrective action). The pricing grid shows how interest rates increase as leverage rises, reflecting higher risk.

---

## 6. Investment Committee Memo

**Role:** Partner at Blackstone
**Objective:** Write an investment committee memo for a deal/company.
**Output Format:** Investment committee presentation deck outline.

### What to Provide

- **Executive summary:** 3-paragraph overview of opportunity (investment thesis, returns, risks)
- **Deal overview:** Structure, size, use of proceeds, timeline
- **Company analysis:** Business model, competitive position, financial performance
- **Industry analysis:** Market size, growth, trends, competitive dynamics
- **Investment thesis:** Why this deal makes money (3–5 key points)
- **Valuation summary:** Multiple methodologies with football field chart description
- **Returns analysis:** IRR, cash-on-cash multiple, exit scenarios

### Input Required

> Deal: [DESCRIBE OPPORTUNITY, DEAL TERMS, EXPECTED RETURNS]

### What This Model Does

The investment committee (IC) memo is the decision document — it synthesizes all the quantitative models (DCF, LBO, comps, credit analysis) into a narrative that recommends whether to proceed with an investment. It is structured to answer the three questions every IC asks: (1) Why is this a good business? (2) Why is this a good deal? (3) What can go wrong? The football field chart visually presents the valuation range from each methodology side by side. The returns analysis ties back to the fund's target returns (typically 20%+ IRR for PE) and shows how realistic the path to those returns is under different exit scenarios.

---

## Category Summary

| # | Model | Perspective | Core Question |
|---|-------|-------------|---------------|
| 1 | DCF Valuation | Investment Banker | What is this company intrinsically worth? |
| 2 | Three-Statement Model | Investment Banker | How do this company's financials flow together? |
| 3 | LBO Model | Private Equity | What returns can we get buying this with leverage? |
| 4 | Comps Analysis | Equity Research | What is the market paying for similar companies? |
| 5 | Credit Analysis | Leveraged Finance | How much debt can this company support? |
| 6 | IC Memo | PE Partner | Should we invest in this deal? |

---

## How These Models Connect

```
Three-Statement Model (foundation)
    │
    ├──► DCF Valuation (intrinsic value from projected cash flows)
    │
    ├──► LBO Model (returns analysis using leveraged capital structure)
    │       │
    │       └──► Credit Analysis (determines how much debt the LBO can use)
    │
    ├──► Comps Analysis (relative value from market multiples)
    │
    └──► Investment Committee Memo (synthesizes all of the above into a decision)
```

The three-statement model provides the financial projections that feed into every other model. The DCF and comps provide valuation from different angles. The credit analysis determines the debt capacity that constrains the LBO structure. The IC memo brings it all together into a single investment recommendation.
