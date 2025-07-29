# Markowitz-s-Framework-applied-to-the-SP500
Can you outperform the S&P 500 using Markowitz’s Optimal Portfolio Theory?

In this project, I attempted to construct a better version of the S&P 500 by applying Markowitz’s mean-variance optimization theory. Using historical price data from all S&P 500 stocks over a one year period, I computed the portfolio weights that minimize total variance, under to three key constraints: the portfolio must be fully invested,  it must deliver at least the same return as the S&P 500 (SPY) over that same period, and shorting or using leverage is not allowed.

I solved this as a convex optimization problem using the SLSQP algorithm, and applied the resulting weights to a completely out-of-sample test period (the following year). The goal was to evaluate how well the optimized portfolio performs in terms of both absolute returns and risk-adjusted returns (Sharpe).

Out-of-sample results showed that the optimized portfolio not only achieved lower volatility than the S&P 500, but also slightly outperformed it on a Sharpe ratio basis. Meaning, the portfolio is better compensated for the risk it is taking on.

To visualize this, I plotted cumulative returns over the test period. As shown in the image below, the most notable observation is the reduced drawdown of the optimized portfolio during the market instability caused by the tariffs.
