# Baza Telecom Customer Churn Prediction

This project predicts *customer churn* (i.e., whether a customer is likely to leave a telecom service) using machine learning techniques. It is implemented in *Google Colab* with a dataset of telecom customer details.

---

## Overview

Customer churn prediction helps telecom companies identify customers who are likely to discontinue their services. By understanding churn patterns, businesses can design better retention strategies and improve customer satisfaction.

This notebook demonstrates:
- Data exploration and visualization  
- Data preprocessing and encoding  
- Feature scaling and selection  
- Model building and evaluation  
- Predictive insights for churn management  

---

## Tech Stack

- *Language:* Python  
- *Environment:* Google Colab  
- *Libraries Used:*
  - pandas, numpy – Data manipulation  
  - matplotlib, seaborn – Data visualization  
  - scikit-learn – Model training and evaluation  
  - xgboost or lightgbm (optional) – Advanced models  

---

## Dataset

The dataset used is typically titled *"Telecom Customer Churn"* (CSV format).  
It contains columns like:

| Feature | Description |
|----------|--------------|
| customerID | Unique ID for each customer |
| gender | Male/Female |
| SeniorCitizen | Indicates if customer is a senior citizen |
| Partner, Dependents | Family details |
| tenure | Number of months with the company |
| PhoneService, InternetService, StreamingTV, etc. | Service features |
| Contract, PaymentMethod, MonthlyCharges, TotalCharges | Billing details |
| Churn | Target variable (Yes/No) |

---

## Steps Performed

1. *Data Loading & Inspection*  
   Load the dataset and inspect for missing/null values and data types.

2. *Data Preprocessing*  
   - Handle missing values  
   - Encode categorical variables (Label/One-Hot Encoding)  
   - Convert target labels (Churn) to binary (0/1)

3. *Exploratory Data Analysis (EDA)*  
   - Visualize churn distribution  
   - Correlation heatmap  
   - Key feature relationships with churn

4. *Feature Scaling*  
   Use StandardScaler or MinMaxScaler to normalize numerical features.

5. *Model Building*  
   - Train models such as:
     - Logistic Regression  
     - Random Forest  
     - Decision Tree  
     - XGBoost
   - Compare their performance using accuracy, precision, recall, and F1-score.

6. *Model Evaluation*  
   - Confusion Matrix  
   - ROC-AUC Curve  
   - Cross-validation  

7. *Prediction*  
   Predict churn on test data and analyze model performance.

---

## Results

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|-----------|------------|---------|-----------|
| Logistic Regression | ~80% | ~79% | ~81% | ~80% |
| Random Forest | ~85% | ~84% | ~86% | ~85% |
| XGBoost | ~87% | ~86% | ~88% | ~87% |

> Note: Actual metrics may vary depending on preprocessing and parameter tuning.

---

## Key Insights

- Customers with *month-to-month contracts* are more likely to churn.  
- Higher *monthly charges* correlate with churn.  
- *Electronic check payment* users show higher churn tendency.  
- *Longer tenure* customers are less likely to churn.

---

## How to Run

1. Open the Colab notebook.

2. Upload the dataset (telecom_churn.csv or equivalent).

3. Run the notebook sequentially:
   - Data loading → Preprocessing → Model building → Evaluation

4. Check the final churn predictions and metrics output.

---

## License

This project is open-source and available for educational use.

---

## Author

*Vechalapu Swamy Hyma Kumar*  
Data Science Enthusiast | Machine Learning Learner  
[vswamyhymakumar222@gmail.com]  
[https://github.com/swamy-4422-v]

---
