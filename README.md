Pairs Trading Strategies & Optimal Execution: Profit Evaluation

• Curated a dataset of the top 100 publicly traded companies based on market capitalization using Yahoo Finance, ensuring robust data quality by filtering out illiquid stocks, redundant tickers (e.g., GOOG vs. GOOGL), and unreliable data (e.g., GTOFF, which exhibited missing or unrealistic prices). Transformed adjusted closing prices using log-scaling for standardization and selected only highly capitalized stocks to minimize volatility and ensure comprehensive historical data.


• Implemented regression models to analyze spread behavior and optimize trade execution, establishing OLS as the baseline model. Required OLS models to meet an adjusted R² of at least 0.9 and a test MSE of no more than 0.1 for validity. Introduced polynomial regression to capture non-linear dependencies, replacing OLS only if the adjusted R² improved by at least 2.5% and test MSE decreased by 2.5%. Ensured complexity was justified by performance gains while avoiding overfitting.


• Backtested the strategy against a buy-and-hold benchmark across different holding periods (15D, 1M, 45D, 2M, etc.), identifying optimal execution timing. Found short-term trades (e.g., 15D) were most profitable for pairs like LLY & NVO, LLY & NONOF, and NVO & PCCYF, while SHEL & XOM performed well over longer horizons (2M+). Observed profitability decay beyond 45 days, reinforcing the importance of time-constrained mean reversion strategies.
