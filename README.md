# Behavioral Market Sentiment Analysis on Hyperliquid Trader Data

## Quantitative Research & Behavioral Trading Analysis

---

# Overview

This project analyzes the relationship between cryptocurrency market sentiment and trader performance using historical trading activity from Hyperliquid alongside the Bitcoin Fear & Greed Index.

The primary objective is to uncover how emotional market conditions influence:
- trader profitability
- trading behavior
- position sizing
- transaction activity
- overall market risk exposure

The project combines:
- Exploratory Data Analysis (EDA)
- Behavioral Finance Interpretation
- Risk Analysis
- Market Sentiment Analysis
- Machine Learning

to simulate a real-world quantitative trading research workflow.

---

# Business Problem

Cryptocurrency markets are highly driven by emotion, volatility, and speculative behavior.

The Bitcoin Fear & Greed Index is commonly used to measure overall market psychology:
- Fear reflects uncertainty and defensive positioning.
- Greed reflects optimism and aggressive risk-taking.

This project investigates:
1. How trader profitability changes under different market sentiment regimes.
2. Whether traders take larger risks during Greed periods.
3. How transaction costs impact effective profitability.
4. Whether market sentiment contributes predictive information regarding trading outcomes.

Understanding these relationships can help design:
- sentiment-aware trading systems
- better risk management frameworks
- behavioral trading strategies
- adaptive position sizing systems

---

# Dataset Information

## 1. Hyperliquid Historical Trader Dataset

Contains detailed trade-level information including:
- Account
- Coin
- Execution Price
- Size Tokens
- Size USD
- Direction
- Fee
- Closed PnL
- Timestamp

## 2. Bitcoin Fear & Greed Index

Contains:
- Date
- Fear/Greed classification
- Sentiment score

The datasets were merged using daily timestamps to analyze trader activity under different emotional market conditions.

---

# Project Structure

```bash
hyperliquid-sentiment-analysis/
│
├── data/
│   ├── historical_data.csv
│   └── fear_greed_index.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── outputs/
│   ├── processed_data.csv
│   └── plots/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Methodology

The project workflow consists of:

## 1. Data Cleaning & Preprocessing
- datetime conversion
- missing value handling
- dataset merging
- feature engineering

## 2. Exploratory Data Analysis
- sentiment distribution
- profitability analysis
- trade size analysis
- transaction fee analysis
- directional positioning behavior

## 3. Behavioral Finance Analysis
- fear vs greed positioning
- emotional trading behavior
- risk appetite analysis
- overtrading patterns

## 4. Machine Learning
A Random Forest classifier was used to predict trade profitability using:
- market sentiment
- trade size
- transaction fees

---

# Feature Engineering

Additional features were created to improve analytical depth:

- Profitability flag (`is_profit`)
- Net PnL after transaction fees (`net_pnl`)
- Absolute PnL (`abs_pnl`)
- Trade size categorization
- Encoded sentiment classification

---

# Exploratory Data Analysis

The EDA section investigates:
- market sentiment frequency
- profitability distributions
- fee accumulation patterns
- trade sizing behavior
- trader positioning trends

Key visualizations include:
- sentiment distribution charts
- PnL distributions
- fee analysis
- correlation heatmaps
- directional trading analysis

---

# Machine Learning Model

## Model Used
- Random Forest Classifier

## Objective
Predict whether a trade is profitable based on:
- market sentiment
- transaction fees
- trade size

## Model Performance

- Accuracy: ~68%
- The model demonstrates moderate predictive capability in highly volatile crypto trading environments.

Given the stochastic nature of financial markets, this performance is considered realistic for an exploratory sentiment-aware predictive model.

---

# Key Insights

## 1. Sentiment Impacts Profitability
Trader profitability improved during Greed market conditions.

## 2. Emotional Markets Increase Risk
Extreme Fear periods showed larger downside volatility and unstable outcomes.

## 3. Traders Increase Exposure During Greed
Trade sizes increased significantly during optimistic market conditions.

## 4. Transaction Costs Matter
High trading activity resulted in elevated fee accumulation, reducing effective profitability.

## 5. Trader Positioning Follows Market Emotion
Long positions dominated during Greed phases, while defensive positioning increased during Fear periods.

---

# Behavioral Finance Interpretation

The analysis reveals strong evidence of sentiment-driven trading behavior.

### Observed Behavioral Patterns
- Increased risk-taking during Greed
- Defensive positioning during Fear
- Overtrading during euphoric phases
- Emotional market conditions amplifying volatility

These findings align closely with established behavioral finance theories.

---

# Strategic Recommendations

Based on the analysis, the following recommendations are proposed:

## 1. Sentiment-Aware Position Sizing
Reduce exposure during Extreme Fear conditions.

## 2. Fee Optimization
Limit excessive trading activity during emotionally volatile markets.

## 3. Dynamic Risk Controls
Implement adaptive stop-loss systems during high-volatility periods.

## 4. Behavioral Monitoring
Track aggressive risk-taking behavior during Greed phases.

## 5. Contrarian Opportunities
Extreme Fear conditions may provide attractive long-term entry opportunities.

---

# Limitations

This project has several limitations:

- Sentiment was analyzed using daily aggregated labels.
- Intraday sentiment fluctuations were not captured.
- External macroeconomic and news events were excluded.
- The ML model is exploratory and not production-optimized.

Future work may incorporate:
- real-time sentiment feeds
- time-series forecasting
- deep learning models
- reinforcement learning systems
- portfolio optimization frameworks

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- Jupyter Notebook

---

# How to Run

## 1. Clone Repository

```bash
git clone <repository-url>
```

## 2. Create Virtual Environment

```bash
python -m venv venv
```

## 3. Activate Environment

### Windows
```bash
venv\Scripts\activate
```

### Mac/Linux
```bash
source venv/bin/activate
```

## 4. Install Dependencies

```bash
pip install -r requirements.txt
```

## 5. Run Notebook

Open:

```bash
notebooks/analysis.ipynb
```

and execute all cells.

---

# Conclusion

This project demonstrates that cryptocurrency market sentiment significantly influences:
- trader profitability
- trade sizing behavior
- transaction activity
- directional positioning

The findings highlight the importance of integrating:
- behavioral finance
- sentiment analysis
- adaptive risk management

into modern quantitative trading systems.

---

# Author

Anushka Joshi

Behavioral Market Sentiment Analysis Project