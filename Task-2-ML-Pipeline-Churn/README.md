# 🏢 Customer Churn Prediction - End-to-End ML Pipeline

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## 📋 Project Overview

This project implements a **production-ready machine learning pipeline** for predicting customer churn in the telecommunications industry. The pipeline demonstrates best practices in ML engineering, including robust preprocessing, model comparison, hyperparameter optimization, and model persistence.

### 🎯 Objective
Build a reusable, scalable ML pipeline that can predict which customers are likely to churn, enabling proactive retention strategies and reducing customer attrition.

### 📊 Dataset
- **Source:** Telco Customer Churn Dataset (IBM)
- **Size:** 7,043 customer records
- **Features:** 21 features including demographics, account details, and service subscriptions
- **Target:** Binary classification (Churn: Yes/No)
- **Churn Rate:** 26.5%

---

## 🏗️ Project Structure
customer-churn-prediction/
│
├── 📓 task2_churn_pipeline.ipynb # Main Jupyter notebook
├── 📊 WA_Fn-UseC_-Telco-Customer-Churn.csv # Dataset
├── 📁 models/ # Saved models directory
│ ├── churn_prediction_pipeline.pkl # Production-ready pipeline
│ └── churn_prediction_pipeline_*.pkl # Versioned models
├── 📄 model_performance_summary.txt # Performance metrics summary
├── 📋 requirements.txt # Python dependencies
└── 📖 README.md # Project documentation
---

## 🚀 Key Features

### ✨ Advanced ML Pipeline
- **Automated Preprocessing**: StandardScaler for numerical features, OneHotEncoder for categorical features
- **ColumnTransformer**: Handles mixed data types seamlessly
- **Multiple Models**: Logistic Regression, Random Forest, Gradient Boosting
- **Hyperparameter Tuning**: GridSearchCV with 5-fold cross-validation
- **Model Persistence**: Joblib serialization for production deployment

### 📈 Performance Metrics
| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Logistic Regression | 73.81% | 0.5043 | 0.7834 | 0.6136 | 0.8415 |
| Gradient Boosting | 80.62% | 0.6735 | 0.5241 | 0.5895 | 0.8432 |
| Random Forest | 78.42% | 0.6232 | 0.4733 | 0.5380 | 0.8193 |

### 🔍 Feature Importance Analysis
Top predictors of customer churn:
1. **Contract Type** - Month-to-month contracts show highest risk
2. **Tenure** - Newer customers more likely to churn
3. **Monthly Charges** - Higher charges correlate with increased churn
4. **Payment Method** - Electronic check users at higher risk
5. **Service Adoption** - Fewer services = higher churn probability

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **Python 3.8+** | Core programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computing |
| **Scikit-learn** | ML algorithms, pipelines, preprocessing |
| **Matplotlib/Seaborn** | Data visualization |
| **Joblib** | Model serialization |
| **Jupyter Notebook** | Interactive development environment |

---

## 📦 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Git (optional, for cloning)

