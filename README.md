# 📈 Stock Market Predictor App

This project is a **Stock Market Price Prediction Web App** built using **Streamlit**, which visualizes historical stock prices and predicts future trends using a trained LSTM model.

## 🚀 Features

- 📊 Real-time stock data fetching using `yfinance`
- 📈 Visualization of:
  - Historical stock prices
  - Moving Averages (MA50, MA100, MA200)
- 🤖 Deep Learning-based price prediction using a pre-trained Keras model
- 📉 Comparison between predicted and actual closing prices

## 🧠 Machine Learning Model

- Trained using LSTM (Long Short-Term Memory) neural network
- Model expects sequences of the past 100 days' closing prices for prediction
- Data normalized using `MinMaxScaler`

## 🛠️ Technologies Used

- Python
- Streamlit
- yFinance
- Keras
- NumPy / Pandas
- Matplotlib
- Scikit-learn

## 📂 Project Structure

```
📁 StockApp/
├── StockApp.py                # Streamlit application
├── Stock Predictions Model.keras  # Trained LSTM model (not provided here)
├── StockPricePrediction.ipynb # (Optional) Jupyter notebook used for training
```

## ▶️ How to Run

1. Install required packages:
   ```bash
   pip install streamlit yfinance keras scikit-learn matplotlib pandas
   ```

2. Place your trained model at the following path:
   ```
   C:\Python\Stock\Stock Predictions Model.keras
   ```

   > ⚠️ Update the path in `StockApp.py` if your model is saved elsewhere.

3. Run the Streamlit app:
   ```bash
   streamlit run StockApp.py
   ```

## 📝 Notes

- Default stock ticker is `GOOG`. You can input other valid tickers like `AAPL`, `TSLA`, etc.
- The app fetches stock data from **2012 to 2022**. You can modify the `start` and `end` dates as required.
- Model predictions are made based on the final 20% of the dataset with the last 100 days used for input preparation.


## 📧 Contact

For any queries or contributions, reach out to:
**Varuni Balodhi**  
📧 varunibalodhi@gmail.com
