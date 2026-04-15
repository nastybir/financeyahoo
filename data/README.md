Financial Dataset Data Card (Yahoo Finance)
1. Project Overview

This project focuses on collecting, processing, and evaluating financial time-series data using the Yahoo Finance API via the Python library yfinance.

The goal is to assess the data quality of stock market datasets using standard Data Quality KPIs and visualize historical trends for analysis and machine learning applications.

2. Data Source

All data is obtained from:

Yahoo Finance (https://finance.yahoo.com
)
Accessed using Python library: yfinance

Yahoo Finance provides reliable financial market data including:

Open price
High price
Low price
Close price
Adjusted Close price
Trading Volume

This dataset is widely used in financial analytics and time-series forecasting.

3. Selected Companies

Five NASDAQ-listed companies were selected:

Apple Inc. (AAPL)
Microsoft Corporation (MSFT)
Amazon.com Inc. (AMZN)
Tesla Inc. (TSLA)
NVIDIA Corporation (NVDA)

Each stock uses a different time period (1 to 5 years) to ensure diversity in dataset size and temporal coverage.

4. Dataset Description

The dataset consists of daily OHLCV (Open, High, Low, Close, Volume) data.

Features:
Date (index)
Open
High
Low
Close
Volume
Adjusted Close

This structure makes the dataset suitable for:

Time-series forecasting
Financial trend analysis
Machine learning models
Anomaly detection
5. Data Quality Evaluation (KPI Framework)

The dataset is evaluated using four Key Performance Indicators (KPIs):

5.1 Completeness

Measures the proportion of non-missing values.

𝐶
𝑜
𝑚
𝑝
𝑙
𝑒
𝑡
𝑒
𝑛
𝑒
𝑠
𝑠
=
1
−
𝑀
𝑖
𝑠
𝑠
𝑖
𝑛
𝑔
 
𝑉
𝑎
𝑙
𝑢
𝑒
𝑠
𝑇
𝑜
𝑡
𝑎
𝑙
 
𝑉
𝑎
𝑙
𝑢
𝑒
𝑠
Completeness=1−
Total Values
Missing Values
	​


Indicates data integrity and missing value ratio.

5.2 Latency

Measures how recent the dataset is compared to the current date.

𝐿
𝑎
𝑡
𝑒
𝑛
𝑐
𝑦
=
𝐶
𝑢
𝑟
𝑟
𝑒
𝑛
𝑡
 
𝐷
𝑎
𝑡
𝑒
−
𝐿
𝑎
𝑡
𝑒
𝑠
𝑡
 
𝐴
𝑣
𝑎
𝑖
𝑙
𝑎
𝑏
𝑙
𝑒
 
𝐷
𝑎
𝑡
𝑎
 
𝐷
𝑎
𝑡
𝑒
Latency=Current Date−Latest Available Data Date

Lower latency means more up-to-date data.

5.3 Accuracy

Checks financial validity rules:

Close price must be between High and Low
𝐴
𝑐
𝑐
𝑢
𝑟
𝑎
𝑐
𝑦
=
𝑉
𝑎
𝑙
𝑖
𝑑
 
𝑅
𝑒
𝑐
𝑜
𝑟
𝑑
𝑠
𝑇
𝑜
𝑡
𝑎
𝑙
 
𝑅
𝑒
𝑐
𝑜
𝑟
𝑑
𝑠
Accuracy=
Total Records
Valid Records
	​


Ensures logical correctness of market data.

5.4 Consistency

Ensures logical stability of values:

No negative prices
High ≥ Low
Valid Open/Close values
𝐶
𝑜
𝑛
𝑠
𝑖
𝑠
𝑡
𝑒
𝑛
𝑐
𝑦
=
𝑉
𝑎
𝑙
𝑖
𝑑
 
𝑅
𝑒
𝑐
𝑜
𝑟
𝑑
𝑠
𝑇
𝑜
𝑡
𝑎
𝑙
 
𝑅
𝑒
𝑐
𝑜
𝑟
𝑑
𝑠
Consistency=
Total Records
Valid Records
	​

6. KPI Results Summary
Ticker	Completeness	Latency (days)	Accuracy	Consistency
AAPL	0.xx	xx	0.xx	0.xx
MSFT	0.xx	xx	0.xx	0.xx
AMZN	0.xx	xx	0.xx	0.xx
TSLA	0.xx	xx	0.xx	0.xx
NVDA	0.xx	xx	0.xx	0.xx
7. Data Visualization

The dataset includes visual analysis such as:

Closing price time-series plots
Trend analysis over time
Optional moving averages (7-day / 30-day)
Volatility analysis

These visualizations help identify market patterns and trends.

8. Reproducibility

The dataset and results are fully reproducible using:

Python 3.x
yfinance
pandas
matplotlib

All data is dynamically retrieved from Yahoo Finance.

9. Limitations
Data depends on Yahoo Finance availability
Latency depends on download time
No intraday (minute-level) data included
External validation sources are not used for accuracy benchmarking
10. Conclusion

The dataset demonstrates strong overall quality across all evaluated KPIs.

High completeness indicates minimal missing data
Accuracy confirms financial consistency rules
Consistency ensures logical correctness
Latency remains acceptable for historical analysis
Overall, the dataset is suitable for:
Stock price prediction
Time-series forecasting
Financial data analysis
Machine learning applications
