# Static Monte Carlo Profitability Analysis
This model utilizes a Static (Snapshot) Monte Carlo Simulation to quantify the financial viability of a proposed business venture. By moving beyond "best-case/worst-case" estimates, this analysis provides a probabilistic distribution of Year 1 outcomes, allowing for a more nuanced understanding of risk exposure and capital requirements.

## Methodology & Logic
The simulation performs **10,000 iterations** of the venture's income statement. Unlike traditional deterministic models, this approach treats key performance indicators (KPIs) as **stochastic variables** rather than fixed inputs:

* **Market Demand & Leads**: Modeled via **Uniform Distribution** to represent a bounded range of possible traffic.
* **Conversion Efficiency**: Modeled via Beta Distribution to reflect realistic "fat-tailed" sales cycles.
* **Operating Costs**: Modeled via **Normal Distribution** to account for standard budgetary variance.
* **Market Volatility**: Integrated as a **Correlation Coefficient** to simulate how external economic shocks simultaneously impact demand and customer acquisition costs (CAC).

## Key Deliverables
1. **Probability of Profitability**: Defined the statistical likelihood of achieving a positive Net Income (EBITDA).

2. **Value at Risk (VaR)**: Identified the **5th percentile downside risk**, establishing the minimum liquidity reserve ($35k) required to ensure venture solvency.

3. **One-Way Sensitivity Analysis**: Utilized **Tornado Charting** to rank variables by their impact on profit volatility, identifying **Conversion Rate** as the primary strategic lever.

## Strategic Conclusion
By shifting from "Single-Point Estimates" to a "Distribution-Based View," this model provides stakeholders with a defensible framework for decision-making under uncertainty. It serves as a foundation for Risk-Adjusted Capital Allocation and strategic prioritizing of operational improvements.
