# Trader Performance vs Market Sentiment

## Objective

Analyze how Bitcoin market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid.  
Identify behavioral patterns and propose actionable strategy recommendations.

---

## Datasets

- Bitcoin Market Sentiment (Fear/Greed Index)
- Historical Trader Data (Hyperliquid)

---

## Methodology

- Cleaned and aligned datasets at daily level  
- Aggregated trade-level data into daily trader metrics  
- Merged sentiment classification with trader activity  
- Conducted statistical testing (t-tests)  
- Segmented traders by:
  - Activity level  
  - Exposure level  
  - PnL consistency  

---

## Key Insights

- Profitability does not significantly differ between Fear and Greed regimes.
- Trading behavior changes significantly across sentiment regimes.
- High activity traders consistently outperform.
- Exposure amplifies performance primarily during Greed regimes.
- Higher volatility traders achieve higher returns but with lower win rates.

---

## Strategy Recommendations

### 1. Sentiment-Based Exposure Adjustment

Allow higher exposure during Greed regimes while tightening exposure controls during Fear regimes.

### 2. Segment-Based Risk Profiling

Apply differentiated risk management rules based on trader activity, exposure, and volatility profile rather than uniform controls.

---

## Bonus – Predictive Model

A logistic regression model was trained to predict next-day profitability using sentiment and behavioral features.

- Accuracy: ~63%
- ROC AUC: ~0.63%

---

## How to Run

Install dependencies:

pip install -r requirements.txt

Run the notebook from top to bottom.
