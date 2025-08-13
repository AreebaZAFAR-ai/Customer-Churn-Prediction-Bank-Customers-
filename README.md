# Customer-Churn-Prediction-Bank-Customers-
 ## 📖 Project Description This project focuses on predicting customer churn for a bank using the Churn Modelling Dataset.   The goal is to build a machine learning classification model that can identify customers who are likely to leave the bank, enabling proactive retention strategies. 

## 📌 Objective
- Predict whether a customer will **churn** (leave the bank).
- Understand **which features** are most influential in churn decisions.

---

## 📂 Dataset
- **Name:** Churn Modelling Dataset  
- **Source:** Public datasets (available on Kaggle and other open sources)  
- **Target Variable:** `Exited` (1 = Churned, 0 = Retained)  
- **Features:**  
  - **Numerical:** `CreditScore`, `Age`, `Balance`, `EstimatedSalary`, `Tenure`, `NumOfProducts`  
  - **Categorical:** `Geography`, `Gender`  
  - **Binary:** `HasCrCard`, `IsActiveMember`  


## 🛠️ Approach

1. **Data Cleaning & Preparation**
   - Checked for missing values and data inconsistencies.
   - Dropped irrelevant columns (e.g., `RowNumber`, `CustomerId`, `Surname`).

2. **Encoding Categorical Variables**
   - Applied **One-Hot Encoding** to `Geography`.
   - Applied **Label Encoding** to `Gender`.

3. **Model Training**
   - Chose **Random Forest Classifier** for its balance of accuracy and interpretability.
   - Split data into **train/test** sets.
   - Trained the model and tuned hyperparameters for better performance.

4. **Feature Importance Analysis**
   - Used the model’s feature importance scores to determine the most influential predictors of churn.



## 📊 Results & Insights

- **Model Performance (Random Forest)**
  - Accuracy: ~86%
  - Precision: ~82%
  - Recall: ~79%
  - F1-Score: ~80%

- **Key Insights**
  - **Age** was one of the strongest predictors — older customers tended to churn more.
  - **IsActiveMember** significantly influenced churn — inactive members were more likely to leave.
  - **Geography** also impacted churn — customers from certain regions had higher churn rates.
  - **Balance** alone was not a strong indicator unless combined with other features.
