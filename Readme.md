# 📊 Customer Churn Prediction

## 📝 Project Overview
Customer churn is when a customer stops doing business with a company.  
For telecom companies, predicting churn is critical for retaining customers.  

In this project, we analyze the **Telco Customer Churn Dataset** to:  
- Understand customer behavior  
- Identify key factors leading to churn  
- Build machine learning models to predict churn  

---

## 📂 Dataset
**Source:** [Telco Customer Churn Dataset (Kaggle)](https://www.kaggle.com/blastchar/telco-customer-churn)  

- Rows: ~7,000 customers  
- Target variable: `Churn` (Yes/No)  
- Features:  
  - Customer demographics (gender, senior citizen, etc.)  
  - Services subscribed (internet, phone, streaming, etc.)  
  - Account info (contract type, payment method, tenure, monthly charges, etc.)  

---

## 🔍 Exploratory Data Analysis (EDA)
- Distribution of churn (Yes vs No)  
- Churn vs Contract type, Payment method, Internet service, etc.  
- Correlation between numerical features (tenure, monthly charges, total charges)  

---

## 🛠️ Data Preprocessing
- Handled missing values  
- Converted categorical variables using One-Hot Encoding  
- Converted target variable `Churn` into binary (1 = Yes, 0 = No)  
- Train-test split (80:20)  

---

## 🤖 Models Used
1. Logistic Regression  
2. Decision Tree Classifier  
3. Random Forest Classifier  

---

## 📈 Model Evaluation
Metrics used: Accuracy, Precision, Recall, F1 Score, ROC-AUC  

| Model                  | Accuracy | Precision | Recall  | F1 Score | 
|------------------------|----------|-----------|-------- |----------|
| Logistic Regression    | 0.738822 | 0.505172  | 0.783422| 0.614256 |         
| Decision Tree          | 0.736693 | 0.504155  | 0.486631| 0.495238 |         
| Random Forest          | 0.789922 | 0.630872  | 0.502674| 0.559524 |         

*(Fill in with your actual results)*  

---

## 🔑 Key Insights
- Customers with **month-to-month contracts** churn more often than those with longer contracts.  
- **Electronic check payment method** is associated with higher churn.  
- **Fiber optic internet** customers show higher churn rates.  
- Customers with **longer tenure** are less likely to churn.  

---

## 💾 Model Deployment
- Best model (Random Forest) saved using `joblib`.  
- File: `churn_model.pkl`  
- Can be used in production APIs for real-time churn prediction.  

---

## 🚀 How to Run the Project
1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/Customer-Churn-Prediction.git
