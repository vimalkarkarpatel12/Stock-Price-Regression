# 📈 Stock Price Prediction using Multiple Linear Regression

This project implements a **Multiple Linear Regression** model to predict the **closing price of a stock** using historical intraday data.  
The model uses **open, high, low, and volume** as input features and evaluates performance on both training and testing datasets.

---
## 📌 Project Objective

To build a regression-based machine learning model that:
- Predicts the **closing price** of a stock
- Evaluates model performance using standard regression metrics
- Visualizes results using training and testing graphs
- Makes predictions for new unseen data

## 📂 Dataset Description

The dataset contains intraday stock price information with the following columns:

| Column | Description |
|------|------------|
| timestamp | Date and time of the trade |
| open | Opening price |
| high | Highest price |
| low | Lowest price |
| close | Closing price (Target Variable) |
| volume | Trading volume |

---

## 🧠 Machine Learning Model

- **Model Used:** Multiple Linear Regression  
- **Target Variable:** `close`  
- **Input Features:** `open`, `high`, `low`, `volume`

---

## ⚙️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## 🔍 Model Workflow

1. Load and preprocess dataset
2. Select features and target variable
3. Split data into training and testing sets
4. Train the regression model
5. Evaluate performance using metrics
6. Visualize training and testing results
7. Predict closing price for new data

---

## 📊 Evaluation Metrics

The model is evaluated using the following regression metrics:

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score (Coefficient of Determination)**

### ✅ Sample Testing Results
- **MAE:** 0.12  
- **RMSE:** 0.16  
- **R² Score:** 0.9999  

> An R² score close to 1 indicates that the model explains almost all the variance in the closing price.

---

## 📈 Visualizations

- **Training Data Graph:** Actual vs Predicted Close Price  
- **Testing Data Graph:** Actual vs Predicted Close Price  

These graphs help analyze model fit and generalization performance.

---

## 🔮 Prediction Example

```python
new_data = [[472, 473, 471.5, 20000]]
predicted_close = model.predict(new_data)
