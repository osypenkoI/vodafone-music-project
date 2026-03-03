# 🎵 Vodafone Music Subscription Prediction

## 📌 Project Overview
Binary classification task: predict whether a Vodafone subscriber will purchase the Music service.

**Business goal:** Optimize marketing campaigns by identifying high-potential customers — enabling more efficient allocation of marketing resources and improving campaign ROI.

---

## 📊 Key Results

| Sprint | Model | Val ROC-AUC |
|--------|-------|-------------|
| 2 | Logistic Regression | 0.8013 |
| 2 | Random Forest | 0.8158 |
| 2 | LightGBM | 0.8261 |
| 3 | **XGBoost (tuned)** | **0.8371** |

**Final model:** XGBoost with RandomizedSearchCV tuning  
**Improvement vs baseline:** +0.011 AUC  
**Optimal threshold:** 0.69

---

## 📂 Project Structure
```
├── data/
│   ├── raw/                        # Raw data (unchanged)
│   └── processed/                  # Cleaned & engineered data
├── models/
│   ├── final_results.json          # Final model metrics
│   ├── sprint3_results.csv         # Sprint 3 comparison
│   └── selected_features.csv       # 514 selected features
├── notebooks/
│   ├── 01_data_understanding.ipynb # EDA & data overview
│   ├── 02_cleaning.ipynb           # Missing values & cleaning
│   ├── 03_eda.ipynb                # Deep EDA & correlations
│   ├── 04_feature_engineering.ipynb# Feature creation (430 → 576)
│   ├── 05_baseline_models.ipynb    # LR, RF, LightGBM
│   ├── 06_model_improvement.ipynb  # XGBoost, CatBoost, tuning
│   └── 07_final_report.ipynb       # Final summary & recommendations
├── src/
├── README.md
└── requirements.txt
```

---

## 🎯 Metrics
- **Primary:** ROC-AUC (imbalance-resistant)
- **Additional:** F1-score, Precision, Recall, Average Precision

---

## 🛠 Tech Stack
- **Python 3.11**
- **Pandas, NumPy** — data processing
- **Matplotlib, Seaborn** — visualization
- **Scikit-learn** — modeling & validation
- **LightGBM, XGBoost, CatBoost** — gradient boosting
- **Jupyter Notebook** — development environment

---

## 🚀 Getting Started
```bash
git clone https://github.com/osypenkoI/vodafone-music-project.git
pip install -r requirements.txt
```
Run notebooks in order: 01 → 02 → 03 → 04 → 05 → 06 → 07

---

## 👤 Author
**Ilona Osypenko** — Data Science Internship