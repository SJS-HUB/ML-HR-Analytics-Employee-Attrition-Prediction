# HR Analytics – Employee Attrition Prediction

This project aims to predict whether an employee is likely to leave the company using supervised machine learning algorithms. It was built as part of a learning journey to explore classification models, feature engineering, and performance evaluation techniques.

---

##  Problem Statement

High employee attrition increases operational costs and affects team productivity. The goal of this project is to build a predictive model that identifies at-risk employees based on HR data.

---

## Dataset

- Source: IBM HR Analytics Employee Attrition dataset  
- Records: 1,470 employees  
- Features: 35 (demographics, job role, satisfaction, income, etc.)  
- Target: `Attrition` (Yes/No)

---

##  Workflow Overview

- **EDA & Visualization**: Explored distributions, correlations, and attrition patterns  
- **Data Cleaning**: Dropped constant and redundant features  
- **Encoding**: Label, One-Hot, and Binary Encoding for categorical variables  
- **Feature Scaling**: Normalized continuous variables using MinMaxScaler  
- **Imbalance Handling**: Used SMOTE to oversample the minority class  
- **Modeling**: Trained and tuned 7 classification models  

---

##  Models Trained

| Model               | Train Accuracy | Test Accuracy | Notes                     |
|--------------------|----------------|---------------|---------------------------|
| Logistic Regression| 71.6%          | 74.4%         | Underfit but stable       |
| KNN Classifier     | 100%           | 61.5%         | Overfit                   |
| Decision Tree      | 99.8%          | 72.1%         | Overfit                   |
| Random Forest      | 100%           | 87.1%         | Strong generalization     |
| AdaBoost           | 86%            | 84%           | Good balance              |
| Gradient Boost     | 93.5%          | 86.3%         | Best trade-off            |
| XGBoost            | 100%           | 87.4%         | High performer            |

✅ **Best performing models**: Random Forest, Gradient Boost, XGBoost  
❌ **Avoid in production**: KNN, Decision Tree

---

## 📌 Key Insights

- OverTime and JobSatisfaction significantly correlate with attrition.
- Most employees who left were younger and in early career stages.
- Gradient Boosting delivered the best balance between accuracy and generalization.

---

##  Technologies Used

- **Languages**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost, imbalanced-learn
- **Techniques**: EDA, SMOTE, Feature Engineering, Model Tuning, Classification Report

---

##  Next Steps

- Deploy model using Flask (WIP)
- Add model versioning and logging (MLflow)
- Experiment with SHAP for interpretability

---

⭐️ *This project is part of my data science learning portfolio. Contributions and feedback are welcome!*  

