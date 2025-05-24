# 🤖 Customer Churn Prediction

This repository focuses on predicting customer churn for a subscription service using historical customer data. A complementary PowerPoint presentation summarizing the data description, methodology, model highlights, and business recommendations is included in the repo. It contains exploratory notebooks, model training, and a serialized Support Vector Classifier model ready for deployment.

## 📂 Repository Contents

* 📝 **CustomerChurnPrediction.ipynb**
  A comprehensive Jupyter notebook that:

  * Describes the dataset (columns and data dictionary).
  * Performs Exploratory Data Analysis (EDA): missing value treatment, variable types standardization, univariate and bivariate analysis.
  * Implements feature engineering (e.g., encoding categorical variables, handling outliers).
  * Trains and compares multiple classification models (e.g., Logistic Regression, Random Forest, SVC).
  * Evaluates models using accuracy, precision, recall, F1-score, and ROC AUC, with visualizations of confusion matrices and ROC curves.

* 💾 **CustomerChurn\_SerializedModel.ipynb**
  A notebook demonstrating how to:

  * Load the best-performing model.
  * Serialize and save the trained model using `joblib` or `pickle`.
  * Load the serialized model for inference on new data.

* 📦 **finalized\_model\_svc.sav**
  The serialized Support Vector Classifier (`.sav`) file exported from the modeling notebook, ready for loading in production scripts.

## 📦 Dependencies

The notebooks require the following Python packages:

```
pandas
numpy
scikit-learn
matplotlib
seaborn
joblib
```

## 🚀 Usage

1. **Explore & Train**: Run `CustomerChurnPrediction.ipynb` to reproduce data analysis and model training.
2. **Serialize Model**: Execute `CustomerChurn_SerializedModel.ipynb` to generate `finalized_model_svc.sav`.
3. **Inference**: In a Python script or notebook, load the model with:

   ```python
   import joblib
   model = joblib.load('finalized_model_svc.sav')
   preds = model.predict(new_data)
   ```

---

## 🎓 Presentation Deck

* 📊 **Customer Churn Prediction Presentation**: A PowerPoint overview that:

  * Defines churn rate and business context with industry benchmarks.
  * Lays out project goals: measuring churn magnitude, profiling churned vs. retained customers, factor analysis, predictive modeling, and retention strategies.
  * Describes the dataset source from Kaggle, feature definitions, and target class balance challenges.
  * Highlights the chosen model (SVC with RBF kernel), hyperparameter tuning approach, and performance metrics (high recall, F1-score).
  * Recommends actionable business interventions: tailored loyalty programs, cross-/up-sell tactics, UX audit of the customer journey, and SLA improvements for customer support.
