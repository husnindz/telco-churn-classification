# Telco Churn Classification (Multi-Model Comparison)

This project focuses on predicting customer churn using a comparative multi-model classification approach based on telecom customer behavior.

Multiple machine learning algorithms are implemented and evaluated to identify the best-performing model for churn prediction. The evaluation includes classification metrics, confusion matrix analysis, and ROC-AUC comparison.

The goal is to support **customer retention strategies** and provide insights into factors influencing customer churn.

---

## 📊 Dataset

- Source: Telecom Customer Churn Dataset (UCI / Kaggle variant)
- Type: Tabular dataset (numerical features)
- Target: `class` (0 = No Churn, 1 = Churn)

### Characteristics:
- Fully numeric dataset
- Represents customer usage behavior and service interaction
- Includes telecom activity across day, evening, night, and international usage

### Key Feature Groups:

- **Customer Information**
  - `state`, `account_length`, `area_code`

- **Service Plans**
  - `international_plan`, `voice_mail_plan`, `number_vmail_messages`

- **Usage Metrics**
  - Call duration, frequency, and charges (day, evening, night, international)

- **Customer Interaction**
  - `number_customer_service_calls` → strong churn indicator

---

## ⚙️ Project Workflow

### 1. Data Understanding
- Explore dataset structure, data types, and distributions
- Analyze class imbalance

### 2. Exploratory Data Analysis (EDA)
- Distribution analysis (histogram & KDE)
- Correlation analysis using heatmap
- Churn behavior visualization based on usage patterns

### 3. Data Preprocessing
- Remove irrelevant features (`area_code`, `phone_number`)
- Feature-target separation
- Train-test split

### 4. Feature Importance
- Apply Random Forest to identify influential features
- Visualize feature importance

### 5. Modeling (Multi-Model)
Implemented multiple classification models:
- Logistic Regression
- Support Vector Machine (SVM with calibration)
- Random Forest
- K-Nearest Neighbors (KNN)
- Naive Bayes

### 6. Evaluation
- Classification report (Precision, Recall, F1-score)
- Confusion matrix analysis
- ROC Curve & AUC comparison across models

### 7. Model Comparison & Selection
- Compare all models based on AUC score
- Identify best-performing model

---

## 🧠 Key Concept

This project uses:
- **Multi-model classification**
- **Model comparison using ROC-AUC**
- **Feature importance analysis**
- **Behavior-based churn prediction**

---

## 📈 Results

- Random Forest achieved the highest performance based on AUC score
- Customers with high service calls and high usage charges show higher churn probability
- Multi-model comparison helps identify the most reliable predictive approach

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib & Seaborn

---

## 📌 Future Improvements

- Apply hyperparameter tuning (Grid Search)
- Improve recall for churn class
- Add feature engineering
- Deploy model for real-world use

---

## 👤 Author

- GitHub: [husnindz](https://github.com/husnindz)
