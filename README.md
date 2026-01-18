# 🚲 Bike Rental Demand Prediction

## 📌 Project Overview
This project analyzes a bike-sharing system dataset to understand how environmental, seasonal, and calendar-related factors influence daily bike rental demand. The goal is to build a machine learning model that can accurately predict daily bike rental counts and support data-driven decision-making in urban mobility planning.

---

## 🎯 Objectives
- Perform Exploratory Data Analysis (EDA) to identify patterns and trends in bike rental usage
- Analyze the impact of weather, seasonality, and time-related features on demand
- Build and compare multiple regression models
- Select the best-performing model for predicting daily bike rentals

---

## 📂 Dataset
- Source: Bike Sharing Dataset
- File used: `day.csv`
- Records: 731 daily observations
- Target variable: `cnt` (total daily bike rentals)

The `day.csv` dataset was selected as it directly represents daily rental demand and aligns with the project objective without requiring aggregation from hourly data.

---

## 🔍 Exploratory Data Analysis
The analysis includes:
- Univariate analysis of numerical and categorical features
- Bivariate analysis to study feature impact on bike rental demand
- Correlation analysis to detect multicollinearity and feature relationships

Key insights:
- Strong seasonality in bike rental demand
- Clear dependence on weather and temperature conditions
- Non-linear relationships between environmental variables and rentals

---

## 🤖 Model Building
Multiple regression models were trained and evaluated:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

A pipeline-based approach was used to ensure consistent preprocessing and prevent data leakage.

---

## 📊 Model Evaluation
Models were evaluated using:
- R² Score
- RMSE
- MAE

**Gradient Boosting Regressor** achieved the best performance with:
- Highest R² score
- Lowest RMSE
- Strong generalization on unseen test data

---

## 🏆 Final Model
**Gradient Boosting Regressor** was selected as the final model due to its ability to capture non-linear relationships and deliver reliable demand predictions.

---

## ⚠️ Challenges Addressed
- Prevented data leakage by removing `casual` and `registered` variables
- Handled multicollinearity between temperature features
- Addressed non-linear patterns through ensemble models
- Used appropriate regression metrics for evaluation

---

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Machine Learning (Regression)

---

## 📌 Conclusion
The project demonstrates how machine learning can be applied to real-world transportation data to forecast demand and support urban mobility planning. The results highlight the importance of environmental and seasonal factors in predicting bike rental usage.

---

## 🔮 Future Scope
- Incorporating real-time weather forecast data
- Exploring hourly-level demand prediction
- Applying hyperparameter tuning and cross-validation
- Extending the dataset with more recent data
