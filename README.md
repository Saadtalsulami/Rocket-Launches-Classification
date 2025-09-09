# 🚀**Rocket Launches Classification Project**

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Classification-orange)
![Status](https://img.shields.io/badge/Project-Success-brightgreen)

---

## 🔥 Executive Summary

This project applies **Machine Learning techniques** to predict the outcome of rocket launches (**Success / Failure / Prelaunch Failure**) using historical data.  
It demonstrates the full ML pipeline: **data cleaning → feature engineering → handling imbalance → model training → evaluation**.  

The final models achieved **~89% accuracy** with Random Forest and **~88% with XGBoost**, proving that machine learning can reliably support **aerospace analytics**.

---

## 📌 Project Workflow

### 1. Data Preparation
- Loaded dataset `rocket_launches_cleand.csv`.  
- Removed irrelevant columns (`Unnamed: 0:1`, `Unnamed: 0`, `Detail`).  
- Selected features: `Company Name`, `Location`, `Datum`, `Status Rocket`.  
- Target variable: `Status Mission`.

### 2. Exploratory Data Analysis
- Generated dataset summary (rows, columns, unique target classes).  
- Plotted target distribution to check **class imbalance**.  

### 3. Feature Engineering
- Extracted **year, month, day** from launch date.  
- Encoded categorical variables (One-Hot & Label Encoding).  
- Applied **StandardScaler** for numerical features.  

### 4. Handling Class Imbalance
- Applied **SMOTE** to oversample minority classes and ensure balanced learning.  

### 5. Model Training
Implemented two classifiers:
- 🌲 **Random Forest Classifier** (n_estimators=200, class_weight="balanced")  
- ⚡ **XGBoost Classifier** (Gradient Boosting)  

### 6. Evaluation Metrics
- Accuracy Score  
- Precision, Recall, F1-score  
- Confusion Matrix + Heatmap  
- Feature Importance analysis  

---

## 📊 Results & Visuals

- **Random Forest** → ~89% Accuracy  
- **XGBoost** → ~88% Accuracy  

🔎 **Key Observations:**  
- Most classes predicted correctly.  
- Minority classes improved significantly after applying SMOTE.  
- Feature engineering boosted performance.  

📌 *Example outputs (add images in repo):*  
- Confusion Matrix ✅  
- Feature Importance Plot ✅  

---

## 💡 Why This Project Matters?

- Demonstrates **real-world ML application** in aerospace and mission analytics.  
- Provides **transferable pipeline** (cleaning, preprocessing, training) applicable to other datasets.  
- Bridges gap between **academic learning** and **industry-grade projects**.  

---

## 🛠️ Tools & Libraries

- **Python 3.9+**  
- **pandas, numpy** → Data manipulation  
- **matplotlib, seaborn** → Visualization  
- **scikit-learn** → Preprocessing, Random Forest, metrics  
- **imblearn (SMOTE)** → Handling class imbalance  
- **XGBoost** → Gradient Boosting classifier  
