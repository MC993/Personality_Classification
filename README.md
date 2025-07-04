# Personality Classification: Introverts vs Extroverts

This project aims to classify individuals as **Introverts** or **Extroverts** based on behavioral and social interaction features. The classification is performed using multiple machine learning models, with the best performance achieved using **XGBoost**, enhanced by **hyperparameter optimization with Optuna**.

## 📊 Problem Overview

The dataset includes features related to:

- Time spent alone
- Stage fear
- Social event attendance
- Going outside frequency
- Post frequency
- Drained energy after socializing
- Size of friend circle

The target variable is `Personality`, a binary class indicating **Introvert (1)** or **Extrovert (0)**.

---

## 🧠 Approach

### 1. **Data Preprocessing**
- Missing values handled using a combination of:
  - Mean/mode imputation
  - Predictive modeling (RandomForest-based feature imputation)
- Categorical encoding using `LabelEncoder`
- Train/test split with stratification

### 2. **Model Training**
Several classification models were tested:
- Logistic Regression
- Random Forest
- XGBoost

### 3. **Hyperparameter Tuning**
High-performing results were achieved through **Optuna**, a powerful hyperparameter optimization library. Key parameters tuned included:

- Learning rate
- Tree depth
- Number of estimators
- Regularization terms

### 4. **Evaluation Metrics**
Models were evaluated using:
- Accuracy
- Precision
- F1 Score

> 🔥 **XGBoost with Optuna-tuned parameters achieved the best performance on the validation set.**

