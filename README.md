# 📈 Stock Price Prediction using NLP and Financial Sentiment

This project uses **Natural Language Processing (NLP)** and financial sentiment to predict Microsoft (MSFT) stock prices. It combines human-labeled sentiment data and FinBERT — a finance-specific transformer model — with historical stock price data to train a machine learning model.

---

## 🔧 Tools & Technologies
- 🧠 **FinBERT**: Transformer-based model for financial sentiment analysis
- 📘 **Takala Financial PhraseBank**: Human-labeled financial sentence dataset
- 💹 **yfinance**: For downloading historical MSFT stock data
- 🐍 **Python**, **pandas**, **scikit-learn**, **matplotlib**, **transformers**

---

## 🔍 What This Project Does
- Applies FinBERT to thousands of financial sentences to extract sentiment
- Simulates news dates to align sentiment with real stock prices
- Merges:
  - Previous day's stock price
  - Takala sentiment score (label-based)
  - FinBERT sentiment score (NLP)
- Trains a **Linear Regression model** to predict closing prices
- Evaluates model performance using RMSE, MAE, and R²

---

## 📊 Model Performance

| Metric | Score |
|--------|-------|
| MAE    | ~1.78 |
| RMSE   | ~2.12 |
| R²     | **0.9198** ✅ |

> The model explains ~92% of the variation in MSFT stock prices using sentiment + historical price.

---

## 📷 Sample Output

![download](https://github.com/user-attachments/assets/f2cbc3e1-c8d6-4912-a909-38b02a968af0)


---

## 🗂️ Files
- `notebook.ipynb` – Full Jupyter Notebook with all steps
- `requirements.txt` – Python dependencies
- `README.md` – This file
- Optionally: `finbert_predictions.csv` or `merged_dataset.csv`

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
