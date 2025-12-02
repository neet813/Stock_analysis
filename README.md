📈 Financial stock analysis tool using Python - Technical indicators, trends, volatility analysis

# 📈 Stock Analysis Tool

## Overview
A Python-based financial analysis tool that analyzes stock performance using technical indicators, moving averages, and volatility metrics. Perfect for learning data analysis and financial concepts.

## Features
✅ Download real stock data from Yahoo Finance
✅ Calculate technical indicators (RSI, Moving Averages)
✅ Analyze volatility and price trends
✅ Generate professional visualizations
✅ Support for multiple stocks

## Quick Start

### Installation
```bash
pip install -r requirements.txt
```

### Run Analysis
```bash
python stock_analyzer.py
# Enter ticker: AAPL
# Enter ticker: MSFT
```

### Output
- Detailed metrics (price change, volatility, trends)
- 4 professional charts (price, RSI, volume, returns)
- Buy/sell signals based on technical analysis

## Example Results

### Apple (AAPL) Analysis
- Current Price: $180.50
- 1-Year Change: +28.5%
- Volatility: 2.1% (Low - Stable)
- Trend: Strong Uptrend (Price > MA20 > MA50)
- RSI: 65 (Neutral)

**Interpretation:** Stock is in uptrend with low risk. Good buying opportunity during dips.

## How It Works

### 1. Data Collection
Downloads 2 years of historical data from Yahoo Finance including:
- Opening, closing, high, low prices
- Trading volume
- Adjusted close prices

### 2. Technical Indicators
Calculates:
- **Moving Averages (20/50)** - Show trend direction
- **RSI (14)** - Identifies overbought/oversold conditions
- **Volatility** - Standard deviation of daily returns
- **Support/Resistance** - Price bounce levels

### 3. Analysis
Determines:
- Price trends (Uptrend/Downtrend/Neutral)
- Risk level (Low/Medium/High)
- Buy/Sell signals based on RSI and Moving Averages

### 4. Visualization
Creates 4-chart dashboard:
1. Price with moving averages and support/resistance
2. RSI indicator with overbought/oversold zones
3. Daily returns distribution
4. Cumulative returns over time

## File Descriptions

- **stock_analyzer.py** - Main analysis script
- **requirements.txt** - Required Python packages
- **TUTORIAL.md** - Step-by-step learning guide for beginners
- **docs/methodology.md** - Detailed explanation of technical indicators

## Key Learnings

After going through this project, you'll understand:
- How to download financial data via API
- Technical analysis concepts (RSI, moving averages)
- Data visualization with matplotlib
- Python pandas for data manipulation
- How to interpret financial charts

## Technologies Used
- **Python 3.x**
- **yfinance** - Yahoo Finance data
- **pandas** - Data manipulation
- **numpy** - Mathematical calculations
- **matplotlib** - Data visualization

## Limitations
- Historical data only (no predictions)
- Uses simple technical indicators
- Should not be sole basis for investment decisions
- Requires internet connection for data download

## Future Enhancements
- [ ] Add MACD indicator
- [ ] Add Bollinger Bands
- [ ] Export reports to PDF
- [ ] Web dashboard with Streamlit
- [ ] Email alerts for price milestones
- [ ] Portfolio tracking (multiple stocks)

## How to Use This for Learning

1. **Beginner:** Read TUTORIAL.md and understand each concept
2. **Intermediate:** Modify the script to analyze different stocks
3. **Advanced:** Add new technical indicators
4. **Expert:** Build a web app with real-time updates

## Example Commands
```python
# Single stock analysis
python stock_analyzer.py
# Enter: AAPL

# Compare multiple stocks
python stock_analyzer.py
# Enter: AAPL,MSFT,GOOGL

# Analyze specific period
# (Modify the script to change period parameter)
```

## Results Interpretation

### Trend Status
- **Strong Uptrend**: Price > MA20 > MA50 (Best for buying)
- **Mild Uptrend**: Price > MA20 only
- **Strong Downtrend**: Price < MA20 < MA50 (Risk)
- **Neutral**: No clear pattern

### RSI Levels
- **RSI > 70**: Overbought (might fall soon)
- **RSI < 30**: Oversold (might rise soon)
- **RSI 30-70**: Fair price (normal range)

### Volatility
- **< 2%**: Low (Safe, boring)
- **2-4%**: Medium (Normal)
- **> 4%**: High (Risky, exciting)

## Real-World Application

This tool is used by:
- Retail investors for stock research
- Day traders for entry/exit points
- Financial analysts for trend confirmation
- Students learning technical analysis

## Disclaimer
This tool is for educational purposes. Always do your own research before investing. Past performance doesn't guarantee future results.

## Contact & Questions
If you have questions or improvements, feel free to open an issue or submit a pull request!

---

**Built to learn. Built to analyze. Built for growth.**
