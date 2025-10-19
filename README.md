# Customer Churn Prediction

Customer churn prediction is a critical problem in business analytics — retaining an existing customer is often more cost-effective than acquiring a new one.  
This project applies machine learning techniques to predict whether a customer is likely to leave a telecom service provider based on their usage behavior and account information.

---

## Objective
To build a predictive model that classifies customers as **“Churn”** or **“Not Churn”**, enabling the business to identify high-risk customers early and plan retention strategies.

---

## Project Overview
This end-to-end project covers:
- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature Encoding and Selection  
- Model Training using Random Forest and XGBoost  
- Model Evaluation using Accuracy, Precision, Recall, and F1-Score  
- Business Insights for Customer Retention  

---

## Dataset
The dataset (Telecom Customer Churn dataset) contains customer demographics, service subscriptions, account details, and churn status.

**Key Features:**
- `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- `tenure`, `Contract`, `PaymentMethod`
- `MonthlyCharges`, `TotalCharges`
- Target: `Churn` (Yes/No)

---

## Steps Followed

### 1 Data Preprocessing
- Handled missing and inconsistent values  
- Converted categorical variables using Label/OneHot Encoding  
- Normalized numerical features (where needed)

### 2 Exploratory Data Analysis (EDA)
- Visualized churn distribution using Seaborn  
- Correlation heatmaps for feature relationships  
- Analyzed effect of contract type, tenure, and monthly charges on churn

### 3 Model Building
Implemented multiple models to compare performance:
- **Random Forest Classifier** (baseline)  
- **XGBoost Classifier** (optimized)  

Used **train_test_split** for data partitioning and cross-validation for robustness.

### 4️ Model Evaluation
Evaluated models using:
- Accuracy Score  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)

Visualized feature importance for business interpretability.

### 5️ Insights & Interpretation
- Customers on **month-to-month contracts** have the highest churn rate.  
- **Higher monthly charges** and **lower tenure** correlate strongly with churn.  
- Business can reduce churn through loyalty programs and bundled offers.

---

## Tech Stack
| Category | Tools / Libraries |
|-----------|-------------------|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Environment | Jupyter Notebook |

---

## Results
- Random Forest Accuracy: ~82%  
- XGBoost Accuracy: ~85%  
- Improved recall for churned customers after hyperparameter tuning  
- Feature importance shows **Contract Type**, **Monthly Charges**, and **Tenure** as key predictors.

---

## Business Impact
The model enables proactive customer retention by:
- Identifying churn-prone customers  
- Helping marketing teams personalize offers  
- Reducing churn rate and improving customer lifetime value  
