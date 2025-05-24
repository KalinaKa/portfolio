# 🏦 Insurance Cost Prediction

A machine learning project to predict insurance costs based on customer demographic and health-related features. This repository includes data exploration, feature engineering, model training, and evaluation notebooks, along with the raw dataset.

## 📂 Repository Contents

* 📊 **InsuranceCostPrediction.ipynb**
  A Jupyter notebook that:

  * Loads and inspects the `insurance.csv` dataset (including column descriptions).
  * Performs Exploratory Data Analysis (EDA): distribution plots, correlation heatmaps, and relationship analysis between features and charges.
  * Implements feature engineering: encoding categorical variables (`sex`, `smoker`, `region`), scaling numeric features, and creating interaction terms.
  * Trains regression models (Linear Regression, Random Forest Regressor) to predict insurance charges.
  * Evaluates performance using RMSE, MAE, and R², with visualizations of residuals and feature importances.

* 🗃️ **insurance.csv**
  The raw dataset containing:

  * `age`, `sex`, `bmi`, `children`, `smoker`, `region`, and target `charges`.

## 📦 Dependencies

The notebook requires the following Python packages:

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

## 🚀 How to Run

1. **Install dependencies**

2. **Open Notebook**:

   ```bash
   jupyter notebook InsuranceCostPrediction.ipynb
   ```
3. **Re-run Cells** to reproduce data analysis, model training, and evaluation.

## 📈 Results

* **Best Model**: Random Forest Regressor achieved an RMSE of \~4200 and R² of 0.80 on the test set.
* **Key Features**: `smoker`, `bmi`, and `age` are the most important predictors of insurance charges.
