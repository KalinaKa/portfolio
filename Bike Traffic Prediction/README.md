# 🚴 Bike Traffic Prediction

A Data Science Bootcamp capstone project to predict daily bike traffic volume across NYC East River crossings (Queensboro Bridge, Williamsburg Bridge, Manhattan Bridge, Brooklyn Bridge) using historical count data and weather factors.

## 📂 Repository Contents

* 📊 **NYC\_Bikes\_Predict\_Traffic.ipynb**
  Jupyter notebook covering:

  * Data ingestion from monthly Excel files (`April 2017–October 2017`).
  * Exploratory Data Analysis (EDA): daily counts, weekly patterns, bridge comparisons.
  * Feature engineering: weekday/weekend flag, weather variables (temperature, precipitation).
  * Modeling: Linear Regression (with and without bridge location), polynomial regression, Decision Tree.
  * Evaluation: R², MAE, MAPE, RMSE metrics and diagnostic plots.

* 🗄️ **Raw Data Excel Files**
  Monthly cyclist counts in `/mnt/data`:  `04 April 2017 Cyclist Numbers for Web.xlsx` through `10 October 2017 Cyclist Numbers.xlsx`.

* 📈 **NYC\_Bikes\_Predict\_Traffic\_presentation.pptx**
  PowerPoint deck summarizing insights, methodology, and results.

## 🗃️ Data Source

* **Timeframe**: April 2017 – October 2017
* **Crossings**: Queensboro Bridge, Williamsburg Bridge, Manhattan Bridge, Brooklyn Bridge
* **Features**: Daily bicycle counts, day type (weekday/weekend), temperature, precipitation

## 🔧 Methodology

1. **EDA & Visualization**

   * Identify average daily volume (\~16K bikes), busiest crossing (Williamsburg: 36%).
   * Uncover stable weekly patterns and higher weekday traffic.

2. **Feature Engineering**

   * Created binary **Is Weekday** flag.
   * Merged weather data for temperature & precipitation.

3. **Modeling**

   * **Linear Regression**: Best fit with R²=1.00, MAE=4.1, RMSE=5.08 (including bridge location).
   * **Without Bridge Location**: R²=0.51, MAE=2773, RMSE=3538.
   * Tested polynomial regression and decision tree (less effective due to linear relationships).

4. **Evaluation**

   * Metrics comparison and residual/ROC plots to validate predictive performance.

## 📈 Key Insights

* **Average Daily Volume**: \~16,000 crossings
* **Busiest Bridge**: Williamsburg Bridge (36% of total)
* **Predictors**: Bridge location, day type, precipitation highly influence counts
* **Model Performance**: Linear regression excels when including location; accuracy drops significantly without it

## 🚀 How to Run

1. **Open Notebook**:

   ```bash
   jupyter notebook NYC_Bikes_Predict_Traffic.ipynb
   ```

## 🔮 Future Improvements

* **Extend Timeframe**: Include full annual data to capture seasonal trends (watch for anomalies in 2020).
* **Temporal Granularity**: Add hourly counts to model commute patterns.
* **Additional Features**: Incorporate wind speed, humidity, and special events data.
* **Advanced Models**: Explore time-series models (ARIMA, LSTM) for sequential prediction.

---

*Powered by NYC Department of Transportation data and Weather API samples.*
