# 🥑 Avocado Price Prediction Using Machine Learning

## 1. Project Overview
Avocado prices fluctuate significantly due to factors such as region, seasonality, supply-demand imbalance, and product type. Predicting avocado prices accurately can help farmers, distributors, retailers, and policymakers make informed decisions.

This project focuses on building a **machine learning regression model** to predict average avocado prices using historical sales data. It demonstrates a complete data science workflow including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and result interpretation.

---

## 2. Problem Statement
To develop a machine learning model that can **predict the average price of avocados** based on historical sales, volume, region, and avocado type.

- **Problem Type:** Regression  
- **Target Variable:** `AveragePrice`  
- **Goal:** Minimize prediction error and understand key drivers affecting price

---

## 3. Project Structure

---

## 4. Dataset Description
The dataset contains weekly avocado sales data collected from different regions in the United States.

### Key Features
- **Date:** Week of observation  
- **AveragePrice:** Average price of avocados (Target variable)  
- **Total Volume:** Total avocados sold  
- **4046, 4225, 4770:** Sales volume by PLU codes  
- **Total Bags:** Total bags sold  
- **Small Bags, Large Bags, XLarge Bags:** Bag size distribution  
- **Type:** Conventional or Organic avocado  
- **Year:** Year of observation  
- **Region:** Sales region  

---

## 5. Data Preprocessing
The following preprocessing steps were applied to prepare the data for modeling:

- Converted date column into datetime format
- Extracted time-based features such as year
- Encoded categorical variables (`Type`, `Region`)
- Checked and handled missing values
- Removed unnecessary or redundant columns
- Applied feature scaling where required
- Ensured clean numerical inputs for regression models

---

## 6. Exploratory Data Analysis (EDA)
EDA was conducted to understand patterns, trends, and relationships within the data.

### Key Analyses Performed
- Distribution of avocado prices over time
- Price comparison between organic and conventional avocados
- Regional price variation analysis
- Correlation analysis between volume and price
- Trend analysis across different years

### Insights
- Organic avocados are consistently priced higher than conventional ones
- Prices show seasonal and regional variation
- Higher supply volume generally correlates with lower prices

---

## 7. Feature Engineering
To improve model performance:
- Categorical features were label-encoded
- Time-based features were extracted from dates
- Irrelevant columns were dropped
- Numerical features were scaled where necessary

Feature engineering helped improve model generalization and stability.

---

## 8. Machine Learning Models Used
Multiple regression models were trained and compared:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Support Vector Regressor (SVR)  
- K-Nearest Neighbors Regressor  

---

## 9. Model Training Strategy
- Dataset split into **80% training and 20% testing**
- Models trained on the same feature set for fair comparison
- Hyperparameter tuning applied to tree-based models
- Cross-validation used to reduce overfitting risk

---

## 10. Evaluation Metrics
Regression models were evaluated using:

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

### Best Performing Model
- **Random Forest Regressor**
- Achieved lowest RMSE and highest R² score
- Effectively captured non-linear relationships between features and price

---

## 11. Results & Key Insights
- Avocado prices are influenced strongly by type, region, and total volume
- Ensemble models outperform linear regression
- Feature engineering and proper preprocessing significantly improve accuracy
- Machine learning models can effectively forecast commodity prices

---

## 12. Limitations
- Dataset limited to U.S. regions only
- External factors like weather and fuel costs are not included
- Model performance depends on historical patterns

---

## 13. Future Improvements
- Include external economic and climate data
- Deploy model using Flask or FastAPI
- Implement time-series forecasting models
- Add real-time price prediction dashboard
- Use deep learning for long-term trend prediction

---

## 14. How to Run the Project
Clone the repository:
```bash
git clone https://github.com/manohar686/avocado-price-prediction.git
