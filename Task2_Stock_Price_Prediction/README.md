# Task 2: Stock Price Prediction (Short-Term)

## Objective
The objective of this task is to predict the next day's stock closing price using historical stock market data. Machine learning regression techniques are used to model the relationship between stock features and closing price.

---

## Dataset
Stock market data is obtained using the `yfinance` Python library from Yahoo Finance.

Example stock used:
- Apple Inc. (AAPL)

Features used:
- Open price
- High price
- Low price
- Volume

Target variable:
- Close price (next day prediction)

---

## Steps Performed

### 1. Data Collection
- Historical stock data downloaded using `yfinance`

### 2. Data Preprocessing
- Removed missing values
- Created target variable by shifting closing price
- Selected relevant features (Open, High, Low, Volume)

### 3. Model Training
- Linear Regression model trained on historical data
- Train-test split performed (time-series aware)

### 4. Prediction
- Model predicts next day's closing price

### 5. Evaluation
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### 6. Visualization
- Actual vs Predicted stock prices plotted

---

## Model Used
- Linear Regression

---

## Evaluation Metrics

- MAE: Measures average prediction error
- RMSE: Penalizes large errors
- R² Score: Measures how well model explains variance

---

## Results
The model was able to capture general trends in stock price movement. However, slight deviations exist due to market volatility, which is expected in financial forecasting.

---

## Key Insights

- Stock prices are highly volatile and difficult to predict accurately
- Linear Regression can capture short-term trends but not sudden market changes
- Volume and price features have strong correlation with closing price

---

## Libraries Used

- pandas
- numpy
- matplotlib
- scikit-learn
- yfinance
