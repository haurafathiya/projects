# 🚢 Titanic Survival Prediction — Kaggle Competition

Submission notebook for the [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic) — predicting passenger survival using machine learning.

🔗 **[View on Kaggle](https://www.kaggle.com/code/hauraalya/submission-titanic-final)**

---

## 🔍 Overview

This project builds a classification model to predict which passengers survived the Titanic disaster, based on features like age, sex, ticket class, and family size.

**Kaggle Public Score: 0.78229**

---

## ⚙️ Workflow

1. **Data Loading** — Load `train.csv` and `test.csv` from Kaggle dataset
2. **Preprocessing**
   - Encode categorical features: `Sex` (male/female → 0/1), `Embarked` (S/C/Q → 0/1/2)
   - Fill missing values: `Age` and `Fare` with median
   - Feature engineering: `FamilySize` (SibSp + Parch + 1), `IsAlone` flag
3. **Modeling** — Train `RandomForestClassifier` (500 estimators, max depth 7)
4. **Prediction** — Generate `submission.csv` for Kaggle submission

---

## 📊 Features Used

| Feature | Description |
|---------|-------------|
| `Pclass` | Ticket class (1st, 2nd, 3rd) |
| `Sex` | Gender (encoded) |
| `Age` | Age (missing values filled with median) |
| `Fare` | Ticket fare |
| `FamilySize` | SibSp + Parch + 1 |
| `IsAlone` | 1 if travelling alone, 0 otherwise |
| `Embarked` | Port of embarkation (encoded) |

---

## 📈 Results

| Metric | Value |
|--------|-------|
| Kaggle Public Score | **0.78229** |
| Model | Random Forest (n=500, max_depth=7) |

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical computation |
| Scikit-learn | RandomForestClassifier |
| Kaggle Notebooks | Development environment |

---

## 📁 Files

| File | Description |
|------|-------------|
| [`submission-titanic-final.ipynb`](submission-titanic-final.ipynb) | Full notebook: preprocessing, modeling, and prediction |

---

## 👤 Author

**Haura Fathiya Alya Kusuma**  
Data Science Student · Insan Cita Indonesia University  
[LinkedIn](https://www.linkedin.com/in/haurafathiya1004) · [Kaggle](https://www.kaggle.com/hauraalya) · [GitHub](https://github.com/haurafathiya)
