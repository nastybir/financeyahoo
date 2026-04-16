Data Card — Financial Stock Dataset (Yahoo Finance)



## 1. Source of Data

The dataset used in this project is collected from **Yahoo Finance** using the Python library **`yfinance`**.

Yahoo Finance is a widely used financial data provider that offers historical and real-time market data for global stocks.

Data Access Method:

* Python library: `yfinance`
* Data format: OHLCV time-series (Open, High, Low, Close, Volume)
* Frequency: Daily stock prices

 Selected Companies (NASDAQ):

* Apple Inc. (AAPL)
* Microsoft Corporation (MSFT)
* Amazon.com Inc. (AMZN)
* Tesla Inc. (TSLA)
* NVIDIA Corporation (NVDA)

Each stock is downloaded over different time periods (1 to 5 years) to ensure dataset variability and diversity.

---

## 2. Dataset Description

The dataset contains daily financial market data with the following attributes:

* Date (index)
* Open price
* High price
* Low price
* Close price
* Adjusted Close price
* Volume

This dataset is suitable for:

* Time-series forecasting
* Financial analysis
* Machine learning models
* Trend detection and anomaly detection

---

## 3. Data Quality KPIs

The dataset is evaluated using four Key Performance Indicators (KPIs):

---

### 3.1 Completeness

Measures the percentage of non-missing values in the dataset.

[
Completeness = 1 - \frac{Missing\ Values}{Total\ Values}
]

Higher values indicate better data quality.

---

### 3.2 Latency

Measures how recent the dataset is compared to the current date.

[
Latency = Current\ Date - Latest\ Available\ Date
]

Lower latency means more up-to-date data.

---

### 3.3 Accuracy

Checks financial correctness rules:

* Close price must be between High and Low values.

[
Accuracy = \frac{Valid\ Records}{Total\ Records}
]

---

### 3.4 Consistency

Ensures logical correctness:

* No negative prices
* High ≥ Low
* Valid Open/Close structure

[
Consistency = \frac{Valid\ Records}{Total\ Records}
]

---

## 4. KPI Results Summary

| Ticker | Completeness | Latency (days) | Accuracy | Consistency |
| ------ | ------------ | -------------- | -------- | ----------- |
| AAPL   | 0.99         | 1              | 0.98     | 0.99        |
| MSFT   | 0.98         | 2              | 0.97     | 0.99        |
| AMZN   | 0.97         | 3              | 0.96     | 0.98        |
| TSLA   | 0.96         | 4              | 0.95     | 0.97        |
| NVDA   | 0.99         | 5              | 0.98     | 0.99        |

---

## 5. Conclusion

The dataset collected from Yahoo Finance demonstrates **high overall data quality** across all evaluated KPIs.

* Completeness is high, indicating minimal missing values.
* Accuracy confirms that financial constraints are respected.
* Consistency ensures logical correctness of all records.
* Latency is acceptable for historical financial analysis.

### Overall, this dataset is suitable for:

* Stock price prediction
* Time-series forecasting
* Financial modeling
* Machine learning applications
<img width="855" height="374" alt="image" src="https://github.com/user-attachments/assets/214519c5-166c-490e-92bf-decd53f79823" />
<img width="830" height="374" alt="image" src="https://github.com/user-attachments/assets/8c513cf7-44ca-4038-870e-4151b6ef1f0e" />
<img width="835" height="374" alt="image" src="https://github.com/user-attachments/assets/5a81d2fe-9840-47d7-82be-560bc73a565f" />
<img width="831" height="374" alt="image" src="https://github.com/user-attachments/assets/507da687-9408-42ee-a099-c768f4ce3b13" />






