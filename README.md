# Optimization Portfolio Allocation for Young Investors

This project explores how a young investor can use **predictive and prescriptive analytics** to optimize a $10,000 stock portfolio across 40 NYSE-listed stocks. We aim to **maximize the Sharpe Ratio** (risk-adjusted return) while enforcing real-world constraints like diversification and individual stock exposure.

Built in Excel and supported with Monte Carlo simulation and a full financial modeling pipeline, this project balances risk and return for long-term retirement growth.



## Project Goals

- Maximize risk-adjusted returns over a 20-year investment horizon
- Compare optimized strategy to S&P 500 and passive saving
- Simulate realistic scenarios with inflation, salary growth, and market volatility
- Evaluate trade-offs between diversification, return, and risk



## Key Results

| Scenario | Sector Constraints | Sharpe Ratio | Expected Return | Companies Invested |
|----------|--------------------|--------------|-----------------|--------------------|
| S0       | Max 10% per sector | 2.16         | 24.2%           | 13                 |
| S1       | 5–15% per sector   | 2.58         | 21.1%           | 20                 |
| S2       | 0–20% per sector   | 2.85         | 16.6%           | 18                 |
| S3       | No constraints     | 3.13         | 19.7%           | 16                 |

- The **optimized portfolio (S0)** nearly **doubles** the value of passive S&P 500 investing over 20 years.
- Relaxing constraints **increases Sharpe Ratio** but **reduces return and sector diversification**.



## Files Included

- `20 Year Retirement Plan Project.xlsx` – Full model built in Excel (Solver, Monte Carlo Sim, return analysis)
- `Term Paper.pdf` – 13-page technical report with sensitivity analysis, forecasting, and methodology
- `Presentation.pdf` – Executive summary slides for stakeholders and recruiters

---

## Methodology

### Predictive Analytics
- Historical stock data sourced from **NASDAQ**
- Daily returns → Annualized means and volatility
- **Monte Carlo simulation** with 1000 iterations over 20 years
- Inflation adjustment: 2.5% | Risk-free rate: 4.9% | Salary base: $85,000 with 3.6% annual growth

### Prescriptive Analytics
- Objective: **Maximize Sharpe Ratio**
- Constraints:
  - Full capital allocation: ∑xᵢ = 1
  - No short selling: xᵢ ≥ 0
  - Max 10% per stock ($1,000 cap)
  - Max 10% per sector (S0 baseline)
- Solver: Excel’s **GRG Nonlinear Solver**



## 💡 Business Impact

This model helps young professionals make **data-driven retirement decisions** by optimizing return without blindly investing in index funds. It lays the foundation for building Python-based tools used by analysts and hedge funds.

It proves that **consistent contributions, early investing, and risk-aware allocation** are the pillars of long-term wealth.



## Future Enhancements

- Rebalancing logic to reflect real-world portfolio updates
- Python-based version with more flexibility and scalability
- Machine learning for improved forecasting
- Customizable profiles for different investors (income, risk, ESG preferences)



## Team

- **Bradley Bryant**  
- Joaquin Moreano  
- Justin Phumathon  
- Jack Smiley



## References

- NASDAQ stock data (5-year history)
- Monte Carlo market modeling
- Sharpe Ratio optimization (Modern Portfolio Theory)



> “Build wealth through data. Invest smarter, not harder.”
