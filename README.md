# House Price Prediction Using Machine Learning and Explainable AI

## Project Overview

This project develops a machine learning-based framework for predicting residential property prices using housing characteristics such as area, bedrooms, bathrooms, stories, parking availability, furnishing status, air conditioning, basement facilities, and location-related features.

The objective is to estimate house prices accurately while identifying the factors that contribute most significantly to property valuation. In addition to predictive modeling, explainable AI techniques were applied to improve model transparency and interpretability.

---

## Dataset

**Dataset:** Housing Prices Dataset

**Source:** Kaggle

The dataset contains information about residential properties, including structural characteristics, amenities, and pricing information.

Target Variable:

* Price

Features Include:

* Area
* Bedrooms
* Bathrooms
* Stories
* Parking
* Main Road Access
* Guest Room
* Basement
* Air Conditioning
* Preferred Area
* Furnishing Status
* Additional engineered features

---

## Data Preprocessing

The following preprocessing steps were performed:

* Missing value analysis and handling
* Duplicate record removal
* One-hot encoding of categorical variables
* Feature engineering
* Data quality assessment

Engineered Features:

* Total Rooms
* Area Per Room

---

## Machine Learning Models Evaluated

The following regression models were trained and compared:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor
4. Decision Tree Regressor
5. K-Nearest Neighbors Regressor
6. Support Vector Regressor
7. XGBoost Regressor

---

## Model Performance

| Model                       | R² Score |
| --------------------------- | -------- |
| Linear Regression           | 0.659    |
| XGBoost Regressor           | 0.646    |
| Gradient Boosting Regressor | 0.618    |
| KNN Regressor               | 0.603    |
| Random Forest Regressor     | 0.571    |
| Decision Tree Regressor     | 0.430    |
| Support Vector Regressor    | 0.414    |

### Best Performing Model

**Linear Regression**

R² Score: **0.659**

The results indicate that housing prices within this dataset exhibit a largely linear relationship with the available features.

---

## Explainable AI

SHAP (SHapley Additive Explanations) was used to interpret model predictions and identify the features that most strongly influence house prices.

Key Influential Features:

* Area
* Total Rooms
* Area Per Room
* Air Conditioning
* Bathrooms
* Preferred Area
* Furnishing Status
* Basement
* Parking

---

## Visualizations

The project includes multiple visualizations:

* Price Distribution
* Correlation Heatmap
* Actual vs Predicted Prices
* Area vs Price
* Feature Importance
* SHAP Summary Plot
* SHAP Feature Importance
* Residual Analysis
* PCA Visualization
* Model Comparison
* Error Distribution
* Outlier Detection

All generated visualizations are available in the `charts` directory.

---

## Business Insights

The analysis revealed that larger properties with more rooms, better amenities, parking availability, and favorable locations tend to command higher prices.

These findings can help:

* Real estate agencies improve pricing strategies
* Buyers assess fair market value
* Sellers understand high-value property features
* Investors identify influential property characteristics

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* SHAP
* XGBoost
* SciPy

---

## Repository Structure

```text
house-price-prediction-ml
│
├── analysis.ipynb
├── Housing.csv
├── summary.pdf
├── README.md
└── charts/
```

---

## Author

Saanvi Mishra

Machine Learning and Data Science Enthusiast
