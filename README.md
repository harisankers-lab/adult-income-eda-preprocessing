# Adult Income – EDA & Data Preprocessing

## 📌 Project Overview

This project explores the Adult Income dataset through Exploratory Data Analysis (EDA) and data preprocessing.

The objective is to understand the factors associated with income levels and prepare the dataset for a future machine learning classification task.

The target variable is `income`, which represents whether an individual earns more than $50K annually.

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

## 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Dataset structure and statistical summaries
- Missing value identification
- Duplicate record detection
- Target class distribution
- Age distribution based on income
- Working hours vs income
- Education level vs income
- Marital status vs income

## 🧹 Data Cleaning

- Standardized inconsistent target labels (`<=50K.` and `>50K.`).
- Replaced unwanted `?` values with NaN.
- Identified and handled impossible values in age and working hours.
- Removed duplicate records.
- Dropped `fnlwgt` (census sampling weight).

## ⚙️ Data Preprocessing

The following preprocessing steps were implemented:

1. **Train-Test Split:** 80% training and 20% testing using stratified sampling.
2. **Missing Value Imputation:**
   - Numerical columns: Median imputation.
   - Categorical columns: Most frequent value imputation.
3. **Feature Scaling:** StandardScaler applied to numerical features.
4. **Categorical Encoding:** OneHotEncoder applied to categorical features.
5. **Target Encoding:** Income labels converted into binary values:
   - `<=50K` → 0
   - `>50K` → 1
6. **Class Imbalance Handling:** SMOTE applied to the training data.
7. **Feature Selection:** Selected features based on correlation with the target variable.

## 📈 Key Observations

- The dataset exhibits an imbalance between the two income classes.
- Age shows a relationship with income levels.
- Education level is associated with income distribution.
- Marital status shows differences in income distribution.
- Working hours alone are insufficient to distinguish income classes.

## 📂 Project Structure

```text
adult-income-eda-preprocessing/
│
├── Harisanker_AdultIncome_EDA_Preprocessing.ipynb
└── README.md
```

## 🎯 Project Outcome

Completed the exploratory data analysis and preprocessing workflow, producing training and testing datasets ready for further classification experiments.

**Note:** This project focuses on EDA and preprocessing. Model training and evaluation are not included in the current notebook.
