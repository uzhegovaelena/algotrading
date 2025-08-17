# Algotrading Research and References

### Open-source algorithmic trading toolkit for stocks & crypto.  
It combines:
- **Factor correlations:** blend macro (rates, inflation, PMI, yields) and micro (momentum, volatility, earnings) to score assets.
- **News sentiment:** analyze finance headlines to detect bullish/bearish tone per ticker.
- **Signals & backtests:** convert scores → BUY/SELL/HOLD and validate with a lightweight backtester.

> ⚠️ Educational use only. This is not financial advice.

## Core modules (planned)
- `data/` – loaders for prices (equities/crypto), macro series, and news.
- `features/` – factor engineering (returns, vol, spreads, earnings surprises, etc.).
- `sentiment/` – headline ingestion + model inference (e.g., FinBERT) → sentiment score.
- `signals/` – correlation & sentiment fusion into a composite alpha score.
- `backtest/` – vectorized backtester with costs, metrics (CAGR, Sharpe, MaxDD).
- `app/` – CLI + Streamlit dashboard for recommendations.

## Roadmap (MVP → v1)
1) MVP-A: Factor correlation scorer (macro+micro) → per-ticker signal  
2) MVP-B: News ingestion + sentiment model → per-ticker sentiment factor  
3) Blend scores (weights/learning) → recommendations; backtest & report  
4) Streamlit dashboard + CI tests; docs & examples

## References
### Architecture Reference: 
<img width="1560" height="926" alt="image" src="https://github.com/user-attachments/assets/83ce57ca-82c9-42d4-b96e-802df99c3f21" />
Russian article: https://habr.com/ru/companies/ods/articles/673376/

### Sentiment Analysis References: 
- [Crypto Fear & Greed Index](https://alternative.me/crypto/fear-and-greed-index/)
- [Crypto sentiment tf-idf by Yorko](https://github.com/crypto-sentiment/crypto_sentiment_tfidf_logreg_streamlit)

