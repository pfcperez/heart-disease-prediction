# Heart Disease Prediction - Logistic Regression Model

[![Python](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Latest-orange.svg)](https://scikit-learn.org/)

## 📝 Overview

Data engineering pipeline that processes cardiac patient data and applies Logistic Regression to predict heart disease risk based on clinical measurements.

- **Dataset:** 303 cardiac patients × 14 features
- **Target:** Heart Disease (Yes/No - Binary)
- **Model Performance:** Accuracy 85.71% | Precision 85% | Recall 86%
- **Clinical Use:** Early disease detection & risk assessment

---

## 🎯 Key Features

✅ Load heart disease dataset (CSV)  
✅ Exploratory analysis of cardiac measurements  
✅ Correlation matrix of health factors  
✅ Feature scaling with StandardScaler  
✅ Train/test split (stratified)  
✅ Logistic Regression classifier  
✅ Precision, Recall, F1-Score evaluation  
✅ Probability predictions for risk assessment  

---

## 🛠️ Tech Stack

- **Python 3.11+** | Pandas | NumPy
- **Visualization:** Matplotlib, Seaborn
- **ML:** Scikit-learn (LogisticRegression, StandardScaler)
- **Development:** Jupyter Notebook

---

## 📦 Installation

```bash
# Clone repo
git clone https://github.com/your-username/heart-disease-prediction.git
cd heart-disease-prediction

# Create virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Download data
# Kaggle: Heart Disease Cleveland Dataset
# Place Heart_disease_cleveland_new.csv in /data/raw/
```

---

## 🚀 Usage

```bash
jupyter notebook logistic_cancer.ipynb
```

**Pipeline Steps:**
1. Load cardiac patient data (303 records × 14 features)
2. Exploratory analysis (age, blood pressure, cholesterol)
3. Correlation analysis (identify key disease predictors)
4. Standardize all features with StandardScaler
5. Split data 80/20 (train/test)
6. Train Logistic Regression model
7. Get predictions + probability scores
8. Evaluate with Precision, Recall, F1-Score

---

## 📊 Results

| Metric | No Disease | Disease |
|--------|-----------|---------|
| **Precision** | 90% | 81% |
| **Recall** | 85% | 87% |
| **F1-Score** | 0.87 | 0.84 |

| Overall | Value |
|---------|-------|
| **Accuracy** | 85.71% |
| **Test Records** | 91 |

**Interpretation:** Model accurately identifies 85% of all patients. For patients WITH disease, catches 87% of cases (high sensitivity for disease detection).

---

## 🔑 Clinical Features

- **age** - Age in years
- **sex** - Male/Female
- **cp** - Chest pain type (4 types)
- **trestbps** - Resting blood pressure (mmHg)
- **chol** - Serum cholesterol (mg/dL)
- **fbs** - Fasting blood sugar > 120 mg/dL
- **restecg** - Resting electrocardiographic results
- **thalach** - Maximum heart rate achieved
- **exang** - Exercise induced angina
- **oldpeak** - ST depression induced by exercise
- **slope** - Slope of ST segment
- **ca** - Number of major vessels
- **thal** - Thalassemia type
- **target** - Heart disease present (0/1)

---

## 📁 Project Structure

```
heart-disease-prediction/
├── logistic_cancer.ipynb     # Main notebook
├── README.md
├── requirements.txt
└── data/
    ├── raw/
    │   └── Heart_disease_cleveland_new.csv
```

---

## 🔑 Data Transformations

- **Feature Scaling:** StandardScaler normalizes all measurements
- **No Missing Values:** Dataset is clean
- **Correlation Analysis:** Identifies strongest predictors
- **Train/Test Split:** 80/20 with stratification

---

## 💡 Key Insights

From correlation analysis:
- **thalach** (max heart rate) - Strong predictor
- **exang** (exercise angina) - Important indicator
- **oldpeak** (ST depression) - Key risk factor
- **cp** (chest pain type) - Diagnostic value

**Clinical Implication:** Combination of heart rate, exercise tolerance, and ECG measurements best predict disease.

---

## 📚 Kaggle Dataset

Source: [Heart Disease UCI Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

---

**Author:** Ramiro Pérez | [GitHub](https://github.com/pfcperez)  
**Status:** ✅ Complete
