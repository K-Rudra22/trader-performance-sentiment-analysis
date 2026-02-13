# Trader Performance vs Market Sentiment

## Objective

Analyze how Bitcoin market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid.  
Identify behavioral patterns and propose actionable strategy recommendations.

---

## Datasets

- Bitcoin Market Sentiment (Fear/Greed Index)  
- Historical Trader Data (Hyperliquid)  

---

## Data Access

Due to file size limitations, raw datasets are not included in this repository.

To reproduce the analysis:

1. Download the datasets from the assignment source.
2. Create a folder named `data` in the project root.
3. Place the files inside the folder as shown below:

data/
  sentiment.csv
  trader_data.csv

The notebook expects the files to be located in this directory.

---

## Methodology

- Cleaned and standardized column names  
- Converted timestamps and aligned datasets at daily level  
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
- High activity traders consistently outperform low activity traders.
- Exposure amplifies performance primarily during Greed regimes.
- Higher volatility traders generate higher returns but with lower win rates.

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

The model shows modest predictive power, indicating that sentiment and behavior contain signal but are not fully explanatory.

---

## How to Run

Install dependencies:

pip install -r requirements.txt

Then open and run the notebook from top to bottom.
