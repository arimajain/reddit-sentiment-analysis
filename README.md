# 📊 Reddit Sentiment Analysis

This program scrapes Reddit posts and comments to find the most mentioned stock tickers and uses the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analyzer to calculate sentiment scores for each ticker.

It helps identify which stocks retail investors are talking about most and what the general sentiment (bullish, bearish, neutral) is around those tickers.

---

## 🚀 Features

- Scans specified subreddits for stock ticker mentions.
- Filters posts/comments based on:
  - Upvote ratio
  - Flair
  - Author credibility
  - Upvotes
- Performs sentiment analysis on each mentioned ticker.
- Outputs top-mentioned tickers and their sentiment breakdown.
- Avoids spam by allowing per-author comment limits and exclusion filters.

---

## 🔧 Program Parameters

| Parameter         | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `subs`           | List of subreddits to search                                                |
| `post_flairs`    | Dictionary of post flairs to include (set to `None` to include all flairs)  |
| `goodAuth`       | Dictionary of authors whose multiple comments are allowed                   |
| `uniqueCmt`      | Boolean - If `True`, only one comment per author per symbol is allowed      |
| `ignoreAuthP`    | Dictionary of authors to ignore for posts                                   |
| `ignoreAuthC`    | Dictionary of authors to ignore for comments                                |
| `upvoteRatio`    | Minimum upvote ratio for a post to be considered (e.g., `0.70` = 70%)       |
| `ups`            | Minimum upvotes required for a post to be considered                         |
| `limit`          | Comment fetch limit (for 'replace more' method)                             |
| `upvotes`        | Minimum upvotes for a comment to be considered                              |
| `picks`          | Number of top tickers to display                                             |
| `picks_ayz`      | Number of tickers to include in sentiment analysis                           |

---
## Conclusion
- 🎯 This stock price prediction project demonstrates how deep learning techniques, specifically LSTM networks, can be effectively applied to time-series data for forecasting financial trends. By leveraging historical stock data and TensorFlow, we were able to model and predict Apple’s future closing prices with reasonable accuracy. 
