Trader Performance vs Market Sentiment
Objective

Analyze how Bitcoin market sentiment (Fear/Greed) relates to trader behavior and performance on Hyperliquid. Identify behavioral patterns and propose actionable strategy recommendations.

Dataset

Bitcoin Market Sentiment (Fear/Greed Index)

Historical Trader Data (Hyperliquid)

Methodology

Cleaned and aligned datasets at daily level

Aggregated trade-level data into daily trader metrics

Merged sentiment classification with trader activity

Conducted statistical testing (t-tests)

Segmented traders by:

Activity level

Exposure level

PnL consistency

Built a simple logistic regression model to predict next-day profitability

Key Insights

Profitability does not significantly differ between Fear and Greed regimes.

Trading behavior changes significantly across sentiment regimes.

High activity traders consistently outperform.

Exposure amplifies performance primarily during Greed regimes.

Higher volatility traders achieve higher returns but with lower win rates.

Strategy Recommendations

Implement sentiment-aware exposure adjustment.

Apply segment-based risk profiling rather than uniform risk controls.

Bonus Model

A logistic regression model achieved:

Accuracy ≈ 63%

ROC AUC ≈ 0.63

Indicating modest predictive signal from sentiment and behavioral features.
