# 🫁 Lung Cancer Prediction Using Machine Learning

## 1. Overview
Lung cancer remains one of the most fatal diseases globally due to late diagnosis and limited early detection methods. This project applies machine learning techniques to predict the likelihood of lung cancer using patient demographic, lifestyle, and symptom-related data. The goal is to demonstrate how data-driven models can assist in early risk assessment and healthcare decision support.

This repository contains a complete end-to-end machine learning pipeline, from raw data processing to model evaluation and result interpretation, implemented in a Jupyter Notebook.

---

## 2. Problem Definition
Early-stage lung cancer often goes undetected due to mild or non-specific symptoms. Manual diagnosis based only on symptoms may be subjective and inconsistent.

**Objective:**  
Build a supervised classification model that predicts whether a patient is likely to have lung cancer based on structured health indicators.

**Type:** Binary Classification  
**Target Variable:** `LUNG_CANCER (YES / NO)`

---

## 3. Project Structure

---

## 4. Dataset Description
The dataset contains patient-level medical and behavioral attributes that influence lung cancer risk. Each row represents one patient record.

### Feature Explanation
- **AGE:** Patient age (numeric)
- **GENDER:** Gender of the patient
- **SMOKING:** Indicates smoking habits
- **YELLOW_FINGERS:** Effect of prolonged nicotine exposure
- **ANXIETY:** Anxiety or stress-related condition
- **PEER_PRESSURE:** Social influence affecting habits
- **CHRONIC DISEASE:** Existing long-term illnesses
- **FATIGUE:** Persistent tiredness
- **ALLERGY:** Presence of allergic conditions
- **WHEEZING:** Breathing difficulty or wheezing sounds
- **ALCOHOL CONSUMING:** Alcohol intake behavior
- **COUGHING:** Chronic or persistent cough
- **SHORTNESS OF BREATH:** Difficulty in breathing
- **CHEST PAIN:** Chest discomfort or pain
- **LUNG_CANCER:** Target label indicating diagnosis

---

## 5. Data Preprocessing
To ensure data quality and model reliability, the following preprocessing steps were performed:

- Converted categorical variables into numerical format using label encoding
- Checked and handled missing or inconsistent values
- Removed redundant features where applicable
- Applied feature scaling for distance-based models (SVM, KNN)
- Ensured balanced class representation during train-test split

---

## 6. Exploratory Data Analysis (EDA)
EDA was conducted to understand patterns, distributions, and relationships within the data.

Key EDA steps:
- Class distribution analysis to check imbalance
- Correlation heatmap to identify influential features
- Visualization of smoking, respiratory symptoms, and cancer correlation
- Gender- and age-wise lung cancer trend analysis

**Observations:**
- Smoking and respiratory symptoms show strong correlation with lung cancer
- Ensemble models benefit from feature interactions
- Some features have low predictive power individually but improve performance collectively

---

## 7. Machine Learning Models Implemented
Multiple supervised learning algorithms were trained and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

Using multiple models allowed performance benchmarking and robustness analysis.

---

## 8. Model Training Strategy
- Data split: **80% Training / 20% Testing**
- Stratified sampling to preserve class distribution
- Hyperparameter tuning applied where relevant
- Cross-validation used to reduce overfitting risk

---

## 9. Evaluation Metrics
Models were evaluated using standard classification metrics:

- **Accuracy:** Overall correctness
- **Precision:** Correct positive predictions
- **Recall:** Ability to identify cancer cases
- **F1-Score:** Balance between precision and recall
- **Confusion Matrix:** Error distribution analysis

### Best Model Performance
- **Model:** Random Forest Classifier
- **Accuracy:** ~95%
- Strong generalization due to ensemble learning
- Handles feature interactions and non-linearity effectively

---

## 10. Results & Insights
- Smoking-related and respiratory features are the strongest predictors
- Random Forest consistently outperformed linear models
- Feature engineering significantly improved model performance
- ML-based screening can support early risk identification but not diagnosis

---

## 11. Limitations
- Dataset size is limited
- No real-time clinical validation
- Predictions depend on self-reported symptoms
- Not suitable for direct medical diagnosis

---

## 12. Future Enhancements
- Use real hospital datasets
- Add model explainability using SHAP or LIME
- Deploy as a web application using Flask or FastAPI
- Integrate deep learning models for improved generalization
- Add automated data validation and monitoring

---

## 13. How to Run the Project
Clone the repository:
```bash
git clone https://github.com/manohar686/Lung-Cancer.git
