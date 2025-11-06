# 🛒 Walmart Weekly Sales Forecasting Project

This project focuses on **forecasting weekly sales across Walmart stores and departments** using historical data that includes promotions, holidays, weather, and economic indicators.  
The goal is to identify the key factors influencing weekly sales and to build a model that can **accurately predict future sales** for better inventory, staffing, and promotion planning.

## 🎯 Project Objectives
- **Data Integration:** Combine multiple data sources — features, stores, and sales — into a single analytical dataset.
- **Feature Engineering:** Create meaningful features such as seasonal indicators, lag variables (`Weekly_Sales_Lag`), and dummy variables for departments, store types, and weeks.
- **Modeling:** Use regression-based approaches (OLS and reduced OLS) to understand how promotions, holidays, and seasonal patterns affect sales.
- **Evaluation:** Compare models using metrics like AIC/BIC, RMSE, and MAE to find the simplest model that still explains most of the variation in weekly sales.
- **Insights:** Identify top-performing departments (e.g., Dept 38, 92, 95) and understand their sales behavior relative to promotions and holidays.

## 🧠 What This Notebook Does
1. **Data Preprocessing:** Load, merge, and clean the Walmart sales, features, and stores datasets.  
2. **Feature Engineering:** Generate dummy variables for categorical columns (store type, department, season, etc.) and lag-based sales features.  
3. **Exploratory Analysis & Visualizations:** Study trends, correlations, and outliers across departments and weeks.  
4. **Model Building:** Fit baseline and extended OLS regression models (`result_withoutpromotion`, `result_with_dpt`, etc.) to predict weekly sales.  
5. **Reduced Models & Comparison:** Drop non-significant predictors (e.g., redundant dummies) to simplify the model while monitoring performance loss.  
6. **Performance Evaluation:** Compute metrics like RMSE, MAE, AIC/BIC, and accuracy for both training and testing sets.  
7. **Scalability & Profiling:** Evaluate computational performance and memory usage for potential deployment.

## ⚙️ Tools & Libraries Used
- **Python** (for all computations and visualizations)  
- **pandas / NumPy:** Data manipulation and feature generation  
- **statsmodels:** Regression modeling and statistical inference  
- **scikit-learn:** Model evaluation and error metrics  
- **matplotlib / seaborn:** Visualizations and insights  
- **AWS (optional future integration):** For deployment or model hosting once finalized

> **Purpose:**  
> This notebook serves as both an **analytical exploration** and a **predictive modeling pipeline** to support Walmart’s decision-making around sales forecasting, promotion planning, and inventory management.
