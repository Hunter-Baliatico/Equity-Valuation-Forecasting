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

An interactive Tableau dashboard used to explore these metrics can be found here (https://public.tableau.com/app/profile/hunter.baliatico/viz/EquityVaIuationForecasting/EquityValuationForecasting) 

---

# Data Structure & Initial Checks  

The dataset includes over **770,000 monthly observations** covering ticker-level pricing, returns, volatility, volume, and dividends. The structured tables:  
- **Price & Returns:** Monthly open, close, high, and low prices along with calculated returns.  
- **Volatility:** Derived monthly volatility to evaluate stability and risk-adjusted returns.  
- **Volume:** Daily and monthly volume trends to validate liquidity screens.  
- **Dividends:** Flags to identify dividend-paying vs. non-dividend stocks.  

---

# Executive Summary  

### Overview of Findings  
Between 2019 and 2024, the market delivered an average **CAGR of 4.02%** with average monthly volatility of **2.46%** across the liquid universe of 2,017 tickers. Dividend-paying companies represented **78% of the dataset**, reflecting strong market coverage of income-generating assets. High-growth tickers primarily came from technology and semiconductor industries, while risk-adjusted leaders included stable large-cap names with consistent performance.  

---

# Insights Deep Dive  

### **Market Snapshot**  
- The overall market delivered an average **CAGR of 4.02%** between January 2019 and January 2024, reflecting a period of steady but moderate growth across the universe of 2,017 liquid tickers. This growth trajectory shows stability even as the broader market faced challenges from macroeconomic events like the pandemic recovery phase and interest rate hikes.  
- **Volatility levels were moderate**, averaging **2.46%**, which indicates relatively stable performance across most sectors. This stability allowed for consistent portfolio growth, particularly for risk-averse investors seeking balanced exposure.  
- Dividend-paying stocks dominate the dataset, representing approximately **78% of analyzed tickers**. This highlights the prevalence of income-generating assets within the liquid equity universe and suggests that dividend-focused strategies could be broadly applicable.  
- The **scenario simulator** provides actionable insights into growth projections. For instance, a stock priced at $50 could grow to $58 under a **3% CAGR**, $64 under a **5% CAGR**, and over $80 at a **10% CAGR** over five years. These projections are crucial for modeling different portfolio growth strategies and assessing compounding effects over time.  
- Sector-level breakdowns in this dashboard also show that technology and healthcare equities generally outperform other sectors, while utilities and consumer staples remain stable but slower-growing, making them ideal candidates for income-focused investors.  
<img width="1350" height="835" alt="D1" src="https://github.com/user-attachments/assets/23d2838d-c888-4ff6-a4db-7eb8eb64dde6" />


---

### **Growth & Stability Leaders**  
- **High-growth leaders dominate the top CAGR rankings.** Between 2019 and 2024, tickers such as **SAVA, AEHR, CAMT, HDSN, and HOV** posted the highest compound annual growth rates, some exceeding **80% CAGR** during the five-year period. This explosive performance reflects strong demand in high-growth industries such as semiconductors, biotech, and specialty manufacturing.  
- **A clear sectoral trend emerges.** Many of the top-performing companies are within the **semiconductor and EDA (Electronic Design Automation)** industries, including LSCC, RMBS, AMD, ACLS, and NVMI. These names benefited from structural growth drivers such as the expansion of AI infrastructure and cloud computing markets.  
- When **adjusted for risk** using the **Sharpe Proxy (CAGR ÷ annualized volatility)**, a different profile emerges. Companies such as **LLY, ETN, SNPS, and MSFT** rank highest due to their ability to deliver strong growth while maintaining **relatively low volatility**, making them attractive to investors prioritizing stable, risk-adjusted returns.  
- This risk-adjusted perspective shows that while certain high-growth tickers experienced dramatic gains, their elevated volatility may not align with more conservative strategies. Conversely, stable compounders like **MSFT and LLY** present a compelling case for inclusion in diversified portfolios.  
- The ranking visualization makes it easy to identify **growth vs. stability leaders**, enabling different investor personas — from aggressive traders to risk-averse investors — to find opportunities aligned with their objectives.  
<img width="1649" height="817" alt="D3" src="https://github.com/user-attachments/assets/175a75f5-0dd9-4da3-8636-2e68db0ff809" />

---

### **Historical Market Insights**  
- The **long-term historical analysis** spanning from 1990 through 2024 reveals a clear upward trajectory in equity markets, underscoring the strength and resilience of long-term investing. Despite short-term corrections, equities have consistently delivered positive returns over time.  
- Key market events are **clearly reflected in price trends and volatility spikes**, such as:  
  - The **2008 financial crisis**, which caused a sharp drawdown and elevated volatility before the market rebounded strongly in subsequent years.  
  - The **2020 COVID-19 pandemic**, which triggered a rapid but short-lived market collapse, followed by one of the fastest recoveries in history due to fiscal and monetary stimulus.  
  - The **2022 macroeconomic correction**, driven by inflation concerns and rate hikes, which temporarily slowed growth but did not derail the longer-term upward momentum.  
- The **volatility trendline** highlights these stress periods, showing heightened risk during crises but also an eventual return to baseline volatility levels, reinforcing the importance of holding through market cycles.  
- **Monthly return patterns** show strong seasonality and momentum effects, with smoothed six-month moving averages helping to filter out noise and identify broader trends. This view supports more data-driven decisions for long-term portfolio management, particularly when balancing growth and risk factors.  
- Historical insights also confirm that while timing the market is challenging, maintaining consistent exposure to high-quality, liquid equities yields robust performance over multi-year horizons, reinforcing core principles of disciplined investing.  
<img width="1651" height="823" alt="D2" src="https://github.com/user-attachments/assets/92ce7a65-674a-4f4d-9858-c2549837d17b" />

---

# Recommendations  

- Leverage the **Market Snapshot dashboard** to quickly assess portfolio-wide growth and volatility levels. This helps investors balance risk exposure across sectors and identify income opportunities within dividend-paying stocks.  
- Use the **Scenario Simulator** to create tailored portfolio growth models under varying CAGR conditions, providing a clear framework for both conservative and aggressive growth strategies.  
- In the **Growth & Stability Leaders dashboard**, prioritize names with high Sharpe Proxy values for stable, risk-adjusted returns while monitoring high-growth leaders for more aggressive plays, particularly in technology and semiconductor sectors.  
- Integrate insights from the **Historical Market Insights dashboard** to understand cyclical risk, prepare for volatility spikes during market stress, and maintain a long-term perspective on equity growth trends.  
- Continuously refresh and monitor the data to ensure real-time relevance, particularly in rapidly evolving sectors like AI, biotech, and clean energy where valuation dynamics can shift quickly.  

---

# Assumptions and Caveats  
- Missing or anomalous pricing data was dropped from the analysis to maintain metric integrity.  
- Sharpe proxy calculations are simplified (CAGR ÷ Avg. Monthly Volatility) and do not account for risk-free rates.  
- Volatility spikes may slightly distort stability rankings for certain low-liquidity tickers.  
- Dividend data is limited to binary flags for payers vs. non-payers and does not reflect the magnitude of payouts.  
