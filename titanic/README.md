# 🛳️ Titanic Survival Analysis — Exploratory Data Project

This project explores the famous Titanic dataset to understand what factors influenced passenger survival. The analysis includes cleaning, feature engineering, visualisation, and early insights to guide modeling.

---

## 📁 Dataset

- Source: [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic/data)
- File used: `train.csv`
- Features include:
  - Demographics (`Sex`, `Age`)
  - Socioeconomic status (`Pclass`, `Fare`)
  - Family info (`SibSp`, `Parch`)
  - Others (`Cabin`, `Embarked`, `Name`, `Ticket`)

---

## 🧹 Data Cleaning & Preparation

- Handled missing values (`Age`, `Embarked`, `Cabin`)
- Created new features:
  - `Title` extracted from names
  - `IsAlone` from `SibSp` + `Parch`
  - `FareCategory` from fare quartiles

---

## 📊 Key EDA Questions

📌 **1. Dataset Overview**
- How many passengers are there in total?
- How many features (columns) are there?
- What data types do we have (numeric, categorical, text)?

📌 **2. Missing Values**
- Which columns have missing values?
- What % of data is missing in each column?
- How should we handle missing Age, Cabin, and Embarked values?

📌 **3. Survival Rate**
- What is the overall survival rate?
- How many survived vs didn’t survive?

📌 **4. Demographics vs Survival**
- Did men or women have higher survival rates?
- How does age relate to survival?
- What was the survival rate for children vs adults vs elderly?

📌 **5. Socioeconomic Status**
- Did passenger class (Pclass) impact survival?
- Which class had the highest/lowest survival rates?

📌 **6. Family Relationships**
- Did people with family aboard survive more often?
- What’s the survival rate for people traveling alone?

📌 **7. Port of Embarkation**
- What are the counts for Embarked values (C, Q, S)?
- Which port had the highest survival rate?

📌 **8. Fare and Cabin**
- What is the distribution of ticket fares?
- Do higher-paying passengers survive more?
- Can Cabin info be used for anything meaningful?

📌 **9. Feature Engineering**
- Can you create a FamilySize column?
- Can you create an IsAlone column?
- Can you extract title from the Name column (Mr, Mrs, etc.)?

📌 **10. Correlation**
- What features are most correlated with survival?
- Any strong relationships between numeric features (e.g., Fare and Age)?



## 🧰 Tools Used

- Python 3.x
- pandas
- numpy
- seaborn
- matplotlib
- Jupyter Notebook

---

## 📈 Outcome

This notebook prepares a clean and well-understood dataset ready for modeling. It lays the foundation for building predictive models (e.g. logistic regression, decision trees) in follow-up work.

---

## 🗂️ Files

- `titanic.ipynb`: Main analysis notebook
- `data/train.csv`: Dataset used for exploration
---

Feel free to fork the repo, run the notebook, or build your own model on top of it.
