# CAC 40 Portfolio Backtest

Anna Docheva and Julien Kanaan

This notebook constructs and evaluates a portfolio of ten CAC 40 stocks. It aligns one-minute prices, computes daily returns, uses lag-one return autocorrelation to forecast next-day returns, and builds daily portfolios with Markowitz optimization. It evaluates realized returns, Sharpe ratios, the upside potential ratio, maximum drawdown, and each stock’s contribution to portfolio volatility.

The notebook includes the original charts and discusses the look-ahead bias introduced by estimating the covariance matrix and autocorrelations over the full sample. The backtest is an in-sample analysis of September 2022 through March 2023.

## Run the notebook

1. Install the dependencies with `python -m pip install -r requirements.txt`.
2. Place the ten original course workbooks in a folder called `dataset TP1` beside the notebook. The loader expects `<ticker>_Prices.xlsx` for MC, OR, TTE, SAN, RMS, AIR, CS, DG, ENGI, and BNP. Row 2 contains the headers, with timestamps in the first column and a column named `Close`.
3. Open `cac40_portfolio_backtest.ipynb` from the repository root in Jupyter and run the cells in order.

The original one-minute market data was distributed through the course and is required to reproduce the saved results.
