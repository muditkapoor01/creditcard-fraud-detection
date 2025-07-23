# 🛡️ Credit Card Fraud Detection

A complete machine learning project to detect fraudulent credit card transactions using real-world data. This project focuses on handling imbalanced datasets, building classification models, and evaluating performance to support financial fraud mitigation.

---

## 📌 Project Overview

This project uses supervised machine learning to detect fraudulent credit card transactions. It involves data preprocessing, exploratory data analysis, model training, and evaluation to distinguish between legitimate and fraudulent activity.

---

## 📂 Dataset

- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records**: 284,807 transactions
- **Features**: 30 numerical variables (V1-V28 are PCA components, plus `Time`, `Amount`, and `Class`)
- **Fraud Ratio**: Only 0.17% of transactions are fraudulent

---

## 🛠️ Technologies Used

- **Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Models**: Logistic Regression, Random Forest Classifier

---

## 📊 Exploratory Data Analysis (EDA)

- Identified severe class imbalance
- Visualized distribution of `Amount`, `Time`, and anonymized features
- Used correlation matrix and boxplots to detect potential fraud patterns
- Found distinct transaction behavior in fraud vs. non-fraud cases

---

## 🔧 Data Preprocessing

- Scaled `Amount` and `Time` using StandardScaler
- Performed train-test split (70:30 ratio)
- Used undersampling to balance classes
- Removed outliers and normalized features

---

## 🤖 Models & Results

### ✅ Logistic Regression
- **Precision (fraud class)**: 83%
- **Recall (fraud class)**: 63%
- **F1 Score**: 0.72
- **ROC AUC**: 0.958

### ✅ Random Forest Classifier
- Outperformed logistic regression in recall and AUC
- Handled class imbalance better and provided stronger generalization

---

## 📈 Evaluation Metrics

- **Confusion Matrix**  
  - TP: 62, FN: 36, TN: 56851, FP: 13 (Logistic Regression)
- **Classification Report**  
  - Balanced accuracy and precision-recall tradeoff
- **ROC Curve**  
  - AUC of ~0.96 indicates strong separability

---

## 📌 Key Insights

- Fraudulent transactions have distinct patterns in feature distribution
- Imbalanced data requires careful handling for effective fraud detection
- Random Forest offers better recall and robustness than Logistic Regression

---

## 💼 Business Impact

- Detecting fraud early helps financial institutions save millions
- Improves customer trust and reduces operational risk
- Supports regulatory compliance and customer satisfaction

---

## 🔮 Future Enhancements

- Apply SMOTE for oversampling minority class
- Explore XGBoost or LightGBM for better accuracy
- Use SHAP for model explainability
- Deploy as an API or web service for real-time fraud detection

---

## 🧠 Author

**Mudit Kapoor**  
Project completed as part of portfolio development for data and business analytics roles.

