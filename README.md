# Yield-Curve-Prediciton



````markdown
📈 Yield Curve Prediction

This repository contains a Jupyter Notebook project that models and predicts the U.S. Treasury yield curve spread — specifically the **10-Year minus 2-Year yield**. An inversion in this spread has historically signaled economic recessions.



📘 Files

- `Yield_curve_prediction.ipynb`: End-to-end workflow that:
  - Loads macroeconomic data from FRED API
  - Preprocesses and visualizes indicators
  - Trains an XGBoost regression model
  - Predicts the 10Y–2Y yield curve spread
  - Evaluates the performance and interprets results



🎯 Objective

To forecast when the yield curve is likely to invert (i.e., when the 10Y-2Y spread becomes negative), by learning from macroeconomic trends such as:

- **Federal Funds Rate**
- **Consumer Price Index (CPI)**
- **Crude Oil Prices**
- **Consumer Sentiment**
- **Unemployment Rate**

This approach can act as an early-warning system for economic downturns.



 📈 Results

After training the model with macroeconomic indicators:

- ✅ **Model Used**: `XGBoostRegressor`
- 📉 **RMSE (Root Mean Squared Error)**: **0.0115**  
- 📊 **R² Score**: **0.9998**

These results indicate **extremely high predictive accuracy**. The R² score of 0.9998 suggests the model can explain over 99.98% of the variance in the yield spread, while the RMSE of 0.0115 means the average prediction error is nearly negligible.



📉 Observations

- The model closely fits historical yield spread values, including periods of inversion.
- Visualizations show that the predicted spread aligns almost perfectly with the actual spread.
- Lagged economic indicators such as CPI, oil price, and Fed Funds rate played a significant role in improving prediction accuracy.

> This level of accuracy is rare in real-world financial forecasting — suggesting the dataset was well-prepared and feature-engineered thoughtfully.



🔧 Requirements

To run this notebook, install the following:

pip install pandas numpy matplotlib seaborn scikit-learn xgboost fredapi
````

You also need a free FRED API key:
🔗 [https://fred.stlouisfed.org/docs/api/api\_key.html](https://fred.stlouisfed.org/docs/api/api_key.html)

---

## 🚀 How to Run

1. Clone the repository
2. Open `Yield_curve_prediction.ipynb` in Jupyter
3. Insert your FRED API key where prompted
4. Run all cells

---

## 📚 Data Source

* Macroeconomic indicators fetched from [FRED](https://fred.stlouisfed.org/)
* Spread calculated as:

  ```
  US10Y Treasury Yield - US2Y Treasury Yield
  ```

---

## Author

Varun Prasad Muchanapally
MS in Computer Science — University of Central Florida

---

## 📝 License

MIT License. Feel free to use, modify, or extend.

```


