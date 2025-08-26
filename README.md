# Project Background  
This project simulates a fintech setting where I analyzed a universe of 7,990 tickers, narrowing it down to 2,017 highly liquid tickers after applying filters like price range ($1–$1,000), non-zero trading volume, and at least 150 trading days per year. The analysis covers data from the early 1990s through today, with a focused look at the period from January 2019 to January 2024 to calculate growth (CAGR) and volatility metrics.  

The goal was to build tools that could be used by retail investors, internal product teams, and the analytics team to:  
- Explore historical price performance and volatility trends  
- Spot steady compounders and fast-growing stocks  
- Model growth projections under different CAGR scenarios to support investment planning  

This analysis focuses on three key areas:  
- Market Snapshot  
- Growth and Stability Leaders  
- Historical Trends and Volatility Patterns  

The interactive Tableau dashboard for this project can be found here: [Tableau Dashboard](https://public.tableau.com/app/profile/hunter.baliatico/viz/EquityVaIuationForecasting/EquityValuationForecasting)  

---

# Data Structure and Initial Checks  

The dataset includes roughly 728,000 monthly records, capturing key details like pricing, returns, volatility, volume, and dividend information for each ticker. The main tables include:  
- Price and Returns: Monthly open, close, high, and low prices, along with monthly return calculations  
- Volatility: Monthly volatility to help measure risk and consistency  
- Volume: Daily and monthly volume data to confirm liquidity filters  
- Dividends: Flags to identify dividend-paying stocks  

---

# Executive Summary  

### Overview of Findings  
Between 2019 and 2024, the market delivered an average CAGR of 4.02% with monthly volatility averaging 2.46%. Roughly 78% of the tickers in the dataset are dividend-paying, highlighting the importance of income-focused strategies in this universe. Many of the highest-growth names came from the tech and semiconductor industries, while companies with high risk-adjusted returns included well-established, stable names like Microsoft (MSFT) and Eli Lilly (LLY).  

---

# Insights Deep Dive  

### Market Snapshot  
- From 2019 to 2024, the market grew at an average CAGR of 4.02%, showing steady performance despite periods of macroeconomic pressure like pandemic recovery phases and interest rate hikes.  
- Average volatility sat at 2.46%, suggesting that the overall market environment was relatively stable. This stability was especially beneficial for more conservative investors.  
- Dividend-paying stocks made up about 78% of all tickers, showing just how common income-generating stocks are in the market. This insight supports the idea that dividend-focused strategies can be applied widely.  
- The scenario simulator provides simple but valuable growth projections. For example, a stock like Microsoft, priced at $408, would grow to around $473 at a 3% CAGR, $521 at 5% CAGR, and $658 at 10% CAGR over five years. These examples make it easier to understand the power of compounding over time.  
- Sector analysis shows that technology and healthcare sectors generally outperformed, while utilities and consumer staples stayed more stable but grew at a slower pace, making them better suited for income-focused portfolios.  
<img width="1352" height="824" alt="D1" src="https://github.com/user-attachments/assets/92b134de-0e3c-4496-be87-4306b0855647" />

---

### Growth and Stability Leaders  
- High-growth names dominated the top CAGR rankings. Between 2019 and 2024, stocks like SAVA, AEHR, CAMT, HDSN, and HOV posted some of the strongest gains, with growth rates exceeding 80% CAGR for the period. These trends were driven by demand in fast-growing industries such as semiconductors, biotech, and advanced manufacturing.  
- Strong sector themes emerged. Many top performers came from semiconductors and EDA (Electronic Design Automation) companies, including LSCC, RMBS, AMD, ACLS, and NVMI, boosted by the rapid expansion of AI and cloud computing.  
- When adjusting for risk using the Sharpe Proxy (CAGR ÷ annualized volatility), the leaderboard changes. Companies like LLY, ETN, SNPS, and MSFT rise to the top thanks to their combination of strong growth and relatively low volatility, appealing to investors looking for steady, risk-adjusted returns.  
- This risk-adjusted view highlights an important trade-off: while some stocks grew explosively, their high volatility may not fit a conservative approach. Conversely, stable compounders like MSFT and LLY stand out for consistent performance with less risk.  
- The dashboard makes it easy to compare growth and stability, helping different types of investors—from aggressive traders to cautious portfolio managers—find opportunities that match their strategies.  
<img width="1649" height="817" alt="D3" src="https://github.com/user-attachments/assets/175a75f5-0dd9-4da3-8636-2e68db0ff809" />

---

### Historical Market Insights  
- Looking back from 1990 through 2024, markets have shown a steady upward climb, proving the strength of long-term investing even through short-term downturns.  
- Significant market events are clearly reflected in price and volatility trends:  
  - The 2008 financial crisis, where markets dropped sharply and volatility spiked before a strong multi-year recovery  
  - The 2020 COVID-19 pandemic, which caused a rapid drop followed by one of the fastest recoveries in history due to global stimulus efforts  
  - The 2022 correction, driven by inflation and rate hikes, which slowed growth but didn’t disrupt the broader upward trend  
- Volatility trends highlight periods of market stress but also show how quickly risk levels normalize, reinforcing the importance of staying invested during uncertainty.  
- Monthly return patterns highlight recurring seasonal and momentum effects, with six-month moving averages helping to smooth out noise and show longer-term trends.  
- These insights make it clear that maintaining exposure to high-quality, liquid equities is one of the most reliable ways to build wealth over the long term.  
<img width="1651" height="823" alt="D2" src="https://github.com/user-attachments/assets/92ce7a65-674a-4f4d-9858-c2549837d17b" />

---

# Recommendations  

- Use the Market Snapshot dashboard to quickly evaluate overall portfolio performance, growth potential, and risk levels across sectors.  
- Take advantage of the Scenario Simulator to model different growth rates and see how compounding could impact returns, helping both cautious and aggressive investors plan ahead.  
- From the Growth and Stability Leaders dashboard, prioritize companies with strong risk-adjusted returns for stable portfolios, while keeping an eye on high-growth stocks in tech and semiconductor spaces for higher-risk, higher-reward plays.  
- Use the Historical Insights dashboard to understand market cycles, prepare for periods of volatility, and build confidence in holding long-term positions.  
- Regularly refresh and review the data, especially for rapidly evolving sectors like AI, biotech, and clean energy, where valuations can shift quickly.  

---

# Assumptions and Caveats  
- Some pricing data was missing or inaccurate and had to be cleaned or removed to keep the analysis accurate.  
- The Sharpe Proxy used in this project is a simplified version (CAGR ÷ Average Monthly Volatility) and does not factor in risk-free rates.  
- Volatility spikes in thinly traded stocks may slightly skew stability rankings.  
- Dividend data only flags whether a stock pays dividends but does not account for the actual size of those payouts.  
