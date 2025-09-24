# 📈 Sentiment-Enhanced Stock Price Forecast

This project integrates **financial news sentiment** with historical stock price data to improve short-term price movement prediction. By combining **FinBERT sentiment embeddings** with **LSTM time-series modeling**, the model achieves significantly lower prediction error compared to using price data alone.

---

## 🚀 Features
- **Sentiment Extraction**: Uses [FinBERT](https://arxiv.org/abs/1908.10063) to analyze daily financial news headlines.  
- **Relevance Filtering**: Applies **cosine similarity** to keep only stock-relevant headlines.  
- **Hybrid Forecasting Model**: Combines sentiment time series with historical OHLCV data in an **LSTM model**.  
- **Performance Gains**:  
  - **Google (GOOG)**: 12.6% reduction in RMSE  
  - **NVIDIA (NVDA)**: 8.4% reduction in RMSE  

---

## 🧠 Tech Stack
- **Python**  
- **PyTorch** – LSTM model training  
- **Pandas, NumPy, scikit-learn** – data preprocessing & evaluation  
- **FinBERT** – sentiment analysis model for finance  
- **Matplotlib/Seaborn** – visualization  

---

## 📊 Results
The model demonstrates how **market sentiment directly impacts short-term price movements**:  

| Stock  | Price-only RMSE | Sentiment + Price RMSE | Improvement |
|--------|----------------|------------------------|-------------|
| GOOG   | 5.23           | 4.57                   | **12.6%**   |
| NVDA   | 6.44           | 5.89                   | **8.4%**    |

---

