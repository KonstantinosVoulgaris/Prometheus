# AIQTM-Quantitative-Trading-Model
Voulgaris I. Konstantinos – AIQTM Artificial Intelligence Quantitative Trading Model


A fully automated, data-driven quantitative trading framework.
This project aims to detect statistically significant patterns, generate trading signals, and eventually execute trades autonomously.

### Key Philosophies

Statistical signals are more important than market intuition

Thousands of small models work best compared to one big model

Continual adaptation of models to evolving conditions

Data from any source is usable (weather, social media, shipping traffic)

Risk is rigorously controlled and optimized

### Project Goals

This project ims to challenge the Efficient Market Hypothesis (EMH) 
by identifying statistically exploitable inefficiencies in price behavior — demonstrating that markets are not always perfectly efficient.

Identify repeating market patterns using a multi-factor approach.
Generate buy/sell signals through statistical and machine learning models.
Achieve automation from data ingestion to execution with zero human intervention.

### Data Pipeline Structure

### 1. Price & Market Data  (Foundation of all quant models)

Ticker, Sector, Industry
Date, Open, High, Low, Close, Adjusted Close
Volume, % Change
Pre-market / After-hours (optional)
Sources include: stocks, ETFs, commodities, macroeconomic indicators (interest rates, CPI), and alternative data (e.g., Google Trends, social sentiment).

### 2. Technical Indicators (Feature Engineering)

Trend: SMA, EMA, MACD
Momentum: RSI, Stochastic, Williams %R
Volatility: ATR, Bollinger Bands, Rolling Std
Volume: OBV, Accumulation/Distribution, VWAP
Mean Reversion: Z-Score, Bollinger %B, Donchian

### 3. Quantitative & ML Features

Rolling returns (1–20 days), lag features
Z-scores, log returns, percentage changes
Cross-sectional rankings
PCA, clustering, feature ratios (e.g., RSI/SMA)

### 4. Fundamental Data (Optional)

P/E, P/B, Debt/Equity, ROE
Insider trading, earnings reports, institutional ownership

### 5. Alternative Data (High-edge components)

News sentiment, Reddit/Twitter trends
Satellite or geospatial activity (e.g., traffic)
Google Trends, order book depth

### Target Variables

Binary: Will price go up tomorrow? (0/1)
Regression: Expected return in X days
Multiclass: Degree of movement (Low/Medium/High)

### Backtesting Engine

Logic for signal generation and execution
Capital allocation & position sizing rules
Slippage, transaction costs, and drawdown limits
Risk management overlays (e.g., stop-loss, dynamic exposure)


### Tech Stack

Python, Pandas, NumPy, Scikit-learn

yFinance, Google Trends API, Reddit API

Plotly, Matplotlib, Jupyter, GitHub Actions

### Notes

Continuous variables → indicators & regressors

Binary variables → flags or event dummies

Patterns must show repeatability, not just correlation

### Status

Currently under development. Daily data ingestion & technical indicator generation scripts completed. Work in progress: feature engineering, ML modeling & backtesting framework.

📂 Repo Structure

📦AIQTM
 ┣ 📁data_ingestion/
 ┣ 📁indicators/
 ┣ 📁features/
 ┣ 📁models/
 ┣ 📁backtesting/
 ┣ 📄README.md
 ┣ 📄requirements.txt
 ┗ 📄LICENSE

### Contact

Konstantinos VoulgarisLinkedIn • GitHub • kos.voulg@gmail.com

