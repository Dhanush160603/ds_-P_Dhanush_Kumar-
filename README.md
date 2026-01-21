# Data Science Assignment – Web3 Trading (Sentiment x Trader Behavior)

This project analyzes how trader performance and behavior vary across different market sentiment regimes (Fear, Greed, Neutral) using Hyperliquid historical trade data and Bitcoin Fear & Greed sentiment data.

The objective is to understand whether sentiment influences trader profitability, participation, risk, accuracy, and positioning.

---

## 📂 Repository Structure

ds_P_Dhanush_Kumar/

│

├── notebook_1.ipynb

│

├── csv_files/

│   ├── fear_greed_index.csv

│   ├── historical_data.csv

│   └── merged_sentiment_trades.csv

│

├── outputs/

│   ├── pnl_vs_sentiment_box.png

│   ├── risk_vs_sentiment.png

│   ├── volume_vs_sentiment_box.png

│   ├── winrate_vs_sentiment.png

│   └── directional_bias_vs_sentiment.png

│

├── ds_report.pdf

│

└── README.md

---

## 🧠 Key Behavioral Dimensions Analyzed

- **Profitability vs Sentiment**
- **Risk Exposure vs Sentiment** (USD notional as proxy)
- **Participation vs Sentiment** (Volume & trade count)
- **Win-rate vs Sentiment**
- **Directional Bias vs Sentiment**

These dimensions reflect expected deliverables for the assignment prompt.

---

## 🔍 Summary of Insights

- Fear regimes produced the strongest PnL and highest win-rates.
- Greed regimes increased participation but reduced accuracy and profitability.
- Risk exposure peaked during Fear, suggesting accumulation behavior.
- Neutral regimes showed strongest bullish positioning but low activity.
- Behavioral patterns align with known crypto sentiment cycles.

---

## 🛠 Technical Approach

- Data cleaning + timestamp normalization
- Daily aggregation for alignment with sentiment
- Merge sentiment ↔ trades
- Behavioral feature engineering:
  - pnl_sum, win_rate, usd_volume, directional_bias, hedge_rate
- Visualization via seaborn & matplotlib
- Manual insight extraction for trading context

---

## ▶️ How to Run

1. Open `notebook_1.ipynb` in Google Colab
2. Upload CSV files to `/csv_files/`
3. Run all cells sequentially

Dependencies:
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

---

## 📄 Report

See `ds_report.pdf` for insights, visual outputs, conclusion, and interpretation.

---

## 🚀 Future Work (Optional)

- Regime-based trading strategies (Long Fear / Fade Greed)
- Integration of funding rates & open interest
- Sentiment signal decay modeling
- Predictive ML for profitability classification
- Backtesting framework for alpha extraction

---

## ✔ Status

Assignment complete according to expected deliverables.
