# 🎵 Vodafone Music Subscription Prediction

## 📌 Project Overview
This project is dedicated to developing a machine learning model for predicting the likelihood of Vodafone subscribers signing up for a music service.

This is a **binary classification** task, where the target variable indicates whether the user has subscribed (1) or not (0).

**Business goal:** Optimize marketing campaigns by identifying customers who are highly likely to be interested in the service. This will reduce the cost of communicating with uninterested subscribers.

---

## 🎯 Goals & Metrics
* **Primary metric:** ROC-AUC. This metric was selected because it allows the quality of the model to be evaluated independently of the selected classification threshold and is resistant to class imbalance.
* **Additional metrics:** F1-score, Precision, Recall.

---

## 📂 Project Structure
The project is organized this way:

```
├── data/
│   ├── raw/             # Raw data (unchanged)
│   └── processed/       # Cleaned data for modeling
├── notebooks/           # Jupyter Notebooks with analysis and code
│   ├── 01_eda.ipynb     # Exploratory data analysis (EDA)
│   └── 02_cleaning.ipynb # Data cleaning and missing 
├── src/                 # Python scripts
├── README.md            # Project description
└── requirements.txt     # List of required libraries
```
---

## 🛠 Tech Stack
* **Python 3.11.9**
* **Pandas, NumPy:** Data processing
* **Matplotlib, Seaborn:** Visualization and EDA
* **Scikit-learn:** Machine learning
* **Jupyter Notebook:** Development environment

---

## 🚀 Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/osypenkoI/vodafone-music-project.git
2. Install the necessary libraries:
   ```bash
   pip install -r requirements.txt
3. Open the notebooks/ folder and run the first file to view the analysis.

---

## 👤 Author
**Ilona Osypenko, student of Odesa National Polytechnic University**