# Trader Behavior & Market Sentiment Analysis

## 📌 Project Overview
This project analyzes cryptocurrency trader behavior under different market sentiment regimes using the Fear & Greed Index.  
The goal is to understand how sentiment influences trading performance, risk-taking behavior, and strategy outcomes.

The project includes:
- Data preparation & feature engineering
- Behavioral analytics
- Trader segmentation
- Predictive modeling
- Interactive dashboard (optional)

---

## 📂 Dataset
Two datasets were used:

1. **Historical Trading Data**
   - Trade-level execution records
   - Account activity and PnL

2. **Fear & Greed Index**
   - Daily crypto market sentiment indicator

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/trader-sentiment-analysis.git
cd trader-sentiment-analysis
2. Install Dependencies
pip install pandas numpy matplotlib seaborn scikit-learn streamlit
3. Run Notebook

Open:

analysis.ipynb

and run all cells sequentially.

▶️ Run Dashboard (Optional)
streamlit run app.py
📊 Outputs

The project generates:

Performance comparison charts (Fear vs Greed)

Behavioral analysis plots

Trader segmentation visualization

Predictive model evaluation

Strategy recommendation tables

🧠 Methodology Summary

Clean and align trading + sentiment datasets.

Engineer behavioral metrics:

Daily PnL

Win rate

Trade frequency

Long/Short ratio

Compare performance across sentiment regimes.

Segment traders into behavioral archetypes.

Train a model to predict next-day profitability.

📈 Key Findings

Trader performance varies significantly across sentiment regimes.

Trading frequency increases during Greed markets.

High leverage traders show higher volatility.

💡 Strategy Recommendations

Reduce leverage during Fear markets.

Increase activity selectively during Greed periods.

Favor consistent traders over high-frequency risk-takers.

🛠 Tech Stack

Python

Pandas

Scikit-learn

Seaborn / Matplotlib

Streamlit

👤 Author

KEERTHAN VIMAL


---

📊 Results & Analysis (Based on Output Graphs)
1️⃣ Trade Size vs Market Sentiment
Observation

Trade sizes vary across sentiment regimes.

Fear markets show wider spread and larger upper outliers.

Extreme Greed shows more compact distributions.

Median trade size is relatively moderate across regimes but variability increases during Fear.

Interpretation

During Fear periods, traders appear to take larger and more inconsistent positions, possibly attempting recovery trades or reacting emotionally to market downturns.

In contrast, Extreme Greed markets exhibit more controlled trade sizing, suggesting confidence-driven but structured participation.

Insight

Market fear increases position-size volatility rather than uniformly reducing risk exposure.

2️⃣ Trading Frequency vs Sentiment
Observation

Trading frequency is significantly higher during Fear periods.

Fear regime shows large upper outliers (very active traders).

Greed markets have lower median activity.

Neutral sentiment shows relatively stable behavior.

Interpretation

Traders become more active during uncertain markets, likely due to:

rapid price movements

attempts to time reversals

reactive trading behavior

This suggests stress-driven overtrading during Fear conditions.

Insight

Traders respond to negative sentiment by increasing activity rather than reducing exposure.

3️⃣ Drawdown by Sentiment
Observation

Largest negative drawdowns appear in Greed and Fear regimes.

Neutral markets show smaller downside risk.

Extreme losses occur primarily when sentiment is polarized.

Interpretation

Both optimistic and pessimistic extremes increase risk exposure:

Greed → overconfidence

Fear → panic or recovery trading

Neutral sentiment corresponds to more stable trading outcomes.

Insight

Emotional market regimes amplify downside risk compared to neutral conditions.

4️⃣ Long/Short Ratio vs Sentiment
Observation

Long/Short ratios exhibit extreme outliers in Greed and Fear regimes.

Neutral markets maintain balanced positioning.

Extreme Greed shows relatively tighter distributions.

Interpretation

Traders strongly bias positions when sentiment is strong:

Greed → aggressive directional bets

Fear → asymmetric hedging or panic positioning

Balanced positioning disappears during emotional regimes.

Insight

Sentiment drives directional conviction, increasing market imbalance.

🧠 Combined Behavioral Understanding

Across all plots, a consistent pattern emerges:

Sentiment	Trader Behavior
Fear	High activity, large variance, unstable risk
Greed	Directional conviction, occasional overconfidence
Neutral	Stable and controlled trading
Extreme Greed	Structured but optimistic participation
💡 Strategy Recommendations (Part C)
Strategy 1 — Fear Market Risk Control

Reduce leverage and trade frequency during Fear periods since traders historically exhibit higher volatility and drawdowns.

Strategy 2 — Momentum Participation in Greed

Selective participation during Greed markets may be beneficial, but risk limits should be enforced due to directional crowding.

Strategy 3 — Neutral Market Stability

Neutral sentiment periods provide more predictable outcomes and may favor systematic or algorithmic strategies.

🤖 Predictive Modeling Implication

The observed behavioral shifts confirm that:

Market sentiment contains predictive signal for trader performance and risk-taking behavior.

This validates the use of sentiment features in the next-day profitability prediction model.
