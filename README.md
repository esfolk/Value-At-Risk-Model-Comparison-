# Value-At-Risk-Model-Comparison

Scientific Paper written by Dany Cajas designed in simple OOP format. 

# Value at Risk (VaR) Models Analysis

In this repository, I delve into various Value at Risk (VaR) models to assess the potential losses an investment portfolio might face over a specified period for a given confidence interval. VaR models are essential tools in risk management and quantitative finance.

Original work covered by Dany Cajas. 

## Models Covered:

1. **VaR (Value at Risk)**: Represents the maximum loss over a specified time horizon at a given confidence level.
2. **CVaR (Conditional Value at Risk)**: Also known as Expected Shortfall (ES), it represents the expected loss given that the loss is beyond the VaR level.
3. **EVaR (Entropic Value at Risk)**: A risk measure based on the concept of entropy, providing a balance between VaR and CVaR.
4. **RLVaR (Relativistic Value at Risk)**: A coherent risk measure and a special case of φ-divergence risk measure based on κ-entropy. It's bounded between the EVaR and ess sup.

## Features:

- **OOP Approach**: The codebase follows an Object-Oriented Programming (OOP) approach, making it modular and easy to extend.
- **Histogram Risk Parity**: We've implemented a histogram-based risk parity approach for RLVaR on portfolio returns, allowing for a visual representation of risk distribution.
- **Visualization**: The results from all VaR models are visualized using a histogram, providing a clear comparison of the risk measures.

## Usage:

1. Define your portfolio returns.
2. Instantiate the `RiskMeasures` class.
3. Call the desired risk measure method on your portfolio returns.
4. Visualize the results using the provided histogram plotting function.

## Example:

```python
risk_measures = RiskMeasures()
var = risk_measures.VaR(portfolio_losses)
cvar = risk_measures.CVaR(portfolio_losses)
evar = risk_measures.EVaR(portfolio_losses)
rlvar = risk_measures.RLVaR(portfolio_losses)
```

## Conclusion:

This repository provides a comprehensive analysis of various VaR models, aiding in the assessment of potential portfolio losses. By understanding these risk measures, investors and financial analysts can make more informed decisions regarding portfolio management and risk mitigation.
