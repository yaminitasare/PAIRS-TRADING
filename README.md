# Pairs Trading Strategy: COP and KO

## Project Overview
This project implements a pairs trading strategy using ConocoPhillips (COP) and Coca-Cola (KO) stocks. The strategy leverages statistical arbitrage opportunities by identifying and exploiting temporary mispricings between these two historically correlated securities.

## Features
- Data retrieval using yfinance for COP and KO stocks
- Z-score calculation for pair correlation analysis
- Trade signal generation based on z-score thresholds
- Visualization of z-scores, individual stock trades, and overall portfolio performance
- Profit and Loss (PnL) calculation
- Performance comparison against S&P 500 benchmark

## Technologies Used
- Python
- pandas for data manipulation
- numpy for numerical computations
- matplotlib for data visualization
- statsmodels for statistical modeling
- yfinance for retrieving stock data

## Methodology
1. **Data Collection**: Historical price data for COP and KO is fetched using yfinance.
2. **Z-Score Calculation**: A rolling z-score is computed to measure the divergence between the two stocks.
3. **Signal Generation**: Trading signals are generated when the z-score crosses predefined thresholds.
4. **Portfolio Management**: The strategy simulates buying and selling stocks based on the generated signals.
5. **Performance Analysis**: The strategy's performance is evaluated using various metrics and compared against the S&P 500.

## Key Components
- `zscore()`: Calculates the rolling z-score for the stock pair
- `generate_trade_signals()`: Creates buy/sell signals based on z-score
- `pnl_calculation()`: Computes the profit and loss of the trading strategy
- `calculate_cagr()`: Calculates the Compound Annual Growth Rate

## Results
- The strategy's performance is visualized through various plots including z-score, individual stock trades, and overall portfolio value.
- CAGR (Compound Annual Growth Rate) of the strategy is calculated and compared to the S&P 500 benchmark.

## Future Improvements
- Implement more sophisticated entry/exit strategies
- Extend the analysis to multiple stock pairs
- Incorporate risk management techniques
- Optimize parameters using machine learning algorithms
