# Behavioral Market Sentiment Analysis on Hyperliquid Trader Data

## Quantitative Research & Behavioral Trading Analysis

---

# Overview

This project analyzes the relationship between cryptocurrency market sentiment and trader performance using historical Hyperliquid trading data combined with the Bitcoin Fear & Greed Index.

The objective is to investigate how emotional market conditions influence:
- trader profitability
- trading activity
- directional positioning
- transaction costs
- overall risk behavior

The project combines:
- Exploratory Data Analysis (EDA)
- Statistical Testing
- Behavioral Finance Interpretation
- Strategy Analysis
- Machine Learning

to simulate a real-world quantitative trading research workflow.

---

# Business Problem

Cryptocurrency markets are highly influenced by:
- emotion
- volatility
- speculative behavior
- market psychology

The Fear & Greed Index is commonly used to measure overall market sentiment:
- Fear reflects uncertainty and defensive behavior
- Greed reflects optimism and aggressive risk-taking

This project investigates:
1. How trader profitability changes across sentiment regimes
2. Whether traders increase exposure during Greed periods
3. How transaction costs impact effective profitability
4. Whether sentiment contributes predictive information regarding trading outcomes

---

# Dataset Information

## 1. Hyperliquid Historical Trader Dataset

Contains:
- Account
- Coin
- Execution Price
- Trade Size
- Direction
- Fee
- Closed PnL
- Timestamp

## 2. Bitcoin Fear & Greed Index

Contains:
- sentiment classification
- sentiment score
- daily timestamps

The datasets were merged using trading dates to analyze trader behavior under different emotional market conditions.

---

# Project Structure

```bash
bitcoin-trader-sentiment-analysis/
│
├── data/
│
├── notebooks/
│   └── analysis.ipynb
│
├── outputs/
│   ├── pnl_by_sentiment.csv
│   ├── strategy_performance.csv
│   ├── trader_performance.csv
│   ├── top_coins.csv
│   └── volume_by_sentiment.csv
│
├── plots/
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
- profitability analysis
- sentiment distribution
- transaction fee analysis
- directional trading analysis
- volume analysis

## 3. Behavioral Finance Analysis
- fear vs greed positioning
- emotional trading behavior
- risk appetite analysis
- overtrading patterns

## 4. Statistical Testing
- Kruskal-Wallis significance testing
- Pearson correlation
- Spearman correlation

## 5. Machine Learning
A Random Forest classifier was used to predict trade profitability using:
- market sentiment
- transaction fees
- trade size

---

# Key Insights

## 1. Sentiment Influences Profitability
Trader profitability improved during Greed market conditions.

## 2. Emotional Markets Increase Volatility
Fear periods showed larger downside volatility and unstable outcomes.

## 3. Risk Appetite Increases During Greed
Traders increased trade sizes during optimistic market phases.

## 4. Transaction Costs Reduce Net Returns
High trading activity resulted in elevated fee accumulation.

## 5. Trader Positioning Follows Market Sentiment
Long positioning dominated during Greed while defensive positioning increased during Fear.

---

# Machine Learning Results

## Model Used
- Random Forest Classifier

## Objective
Predict whether a trade is profitable based on:
- market sentiment
- trade size
- transaction fees

## Performance
- Accuracy: ~68%

Given the highly stochastic and volatile nature of cryptocurrency markets, this performance is considered realistic for an exploratory predictive trading model.

---

# Behavioral Finance Interpretation

The analysis reveals strong evidence of sentiment-driven trading behavior.

### Observed Patterns
- Increased risk-taking during Greed
- Defensive positioning during Fear
- Emotional volatility amplifying market instability
- Overtrading during euphoric market conditions

These findings align closely with established behavioral finance theories.

---

# Strategic Recommendations

## 1. Sentiment-Aware Position Sizing
Reduce exposure during Extreme Fear conditions.

## 2. Fee Optimization
Limit excessive trading activity during volatile periods.

## 3. Dynamic Risk Controls
Implement adaptive stop-loss systems during high-volatility conditions.

## 4. Behavioral Monitoring
Track aggressive positioning during euphoric markets.

## 5. Contrarian Trading Opportunities
Extreme Fear periods may offer attractive long-term entries.

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

## Clone Repository

```bash
git clone <repository-url>
```

## Create Virtual Environment

```bash
python -m venv venv
```

## Activate Environment

### Windows
```bash
venv\Scripts\activate
```

### Mac/Linux
```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Notebook

Open:

```bash
notebooks/analysis.ipynb
```

and execute all cells.

---

# Conclusion

This project demonstrates that cryptocurrency market sentiment significantly impacts:
- trader profitability
- transaction behavior
- risk exposure
- directional positioning

The findings emphasize the importance of integrating:
- behavioral finance
- sentiment analysis
- adaptive risk management

into modern quantitative trading systems.

---

# Author

Anushka Joshi