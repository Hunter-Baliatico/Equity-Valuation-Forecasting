# Project Background  
This project simulates a fintech environment where I analyzed a universe of 7,990 tickers, narrowed down to 2,017 liquid tickers after applying validity filters (price range $1–$1,000, non-zero volume) and liquidity screens (≥150 trading days per year). The analysis spans the post-1990 period, with a focused window from January 2019 to January 2024 for CAGR and volatility metrics.  

The goal was to build tools for **retail investors**, **internal product teams**, and the **head of analytics** to:  
- Explore historical price performance and volatility trends.  
- Identify stable compounders and high-growth opportunities.  
- Model growth projections under multiple CAGR scenarios for valuation planning.  

Insights and recommendations are provided on the following key areas:  
- **Market Snapshot**  
- **Growth & Stability Leaders**  
- **Historical Trends & Volatility Patterns**  
An interactive Tableau dashboard used to explore these metrics can be found here [link].  

---

# Data Structure & Initial Checks  

The dataset includes over **770,000 monthly observations** covering ticker-level pricing, returns, volatility, volume, and dividends. The structured tables:  
- **Price & Returns:** Monthly open, close, high, and low prices along with calculated returns.  
- **Volatility:** Derived monthly volatility to evaluate stability and risk-adjusted returns.  
- **Volume:** Daily and monthly volume trends to validate liquidity screens.  
- **Dividends:** Flags to identify dividend-paying vs. non-dividend stocks.
- 
---

# Executive Summary  

### Overview of Findings  
Between 2019 and 2024, the market delivered an average **CAGR of 4.02%** with average monthly volatility of **2.46%** across the liquid universe of 2,017 tickers. Dividend-paying companies represented **78% of the dataset**, reflecting strong market coverage of income-generating assets. High-growth tickers primarily came from technology and semiconductor industries, while risk-adjusted leaders included stable large-cap names with consistent performance.  

---

# Insights Deep Dive  

### Market Snapshot  
The overall market CAGR averaged 4.02% between 2019 and 2024, reflecting a modest but stable growth period. The distribution between dividend and non-dividend stocks highlights that income-oriented companies form the majority of liquid names analyzed, while the scenario simulation provides clear growth projections under multiple CAGR assumptions.  
<img width="1350" height="835" alt="D1" src="https://github.com/user-attachments/assets/7c1b3969-e634-4e61-97f4-964cbb169b43" />

---

### Growth & Stability Leaders  
High-CAGR tickers like **SAVA, AEHR, CAMT, HDSN, and HOV** showed exceptional growth, largely driven by technology and semiconductor sectors. However, when adjusted for volatility, companies like **LLY, ETN, SNPS, and MSFT** surfaced as stable compounders offering consistent growth with lower risk.  
<img width="1649" height="817" alt="D3" src="https://github.com/user-attachments/assets/ba39b823-14aa-4764-8cda-2d63e89ef72d" />

---

### Historical Market Insights  
A deep look at post-1990 data shows long-term upward market momentum, interrupted by notable volatility spikes during events such as the 2008 financial crisis, the 2020 COVID crash, and 2022 market corrections. Despite these fluctuations, overall returns have demonstrated resilience, with smoothed moving averages confirming consistent recovery patterns across decades.  
<img width="1651" height="823" alt="D2" src="https://github.com/user-attachments/assets/e028291b-fad6-429a-9eeb-19a9ffae8e12" />

---

# Recommendations  
- Use **CAGR and volatility filters** to isolate companies that match desired risk/return profiles.  
- Highlight **stable compounders** with high Sharpe-like metrics for conservative strategies.  
- Leverage historical volatility patterns to build context when projecting future scenarios.  
- Incorporate these dashboards into broader portfolio analytics tools to enhance investor decision-making.  

---

# Assumptions and Caveats  
- Missing or anomalous pricing data was dropped from the analysis to maintain metric integrity.  
- Sharpe proxy calculations are simplified (CAGR ÷ Avg. Monthly Volatility) and do not account for risk-free rates.  
- Volatility spikes may slightly distort stability rankings for certain low-liquidity tickers.  
