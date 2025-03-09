# Predicting Educational Outcomes with Machine Learning

This project explores factors influencing standardized test scores across school districts in California. Using regression-based models, the analysis investigates how student demographics, teacher counts, and per-student spending correlate with test performance.

---

## 📊 Dataset
- [California School Data](https://vincentarelbundock.github.io/Rdatasets/doc/Ecdat/Caschool.html)
- Source: `Ecdat::Caschool` dataset from the R Datasets package

---

## 🧠 Problem Statement
> Can we predict average test scores in California schools based on variables like student-teacher ratio, district income, and number of computers?

---

## 🔍 Features Used
- Student enrollment, teacher count, income levels
- Percentage of students on CalWorks (proxy for economic disadvantage)
- English learner percentage, computers per student
- Expenditure per student, student-teacher ratio

---

## 🧪 Methods & Models
- Linear Regression
- Ridge Regression (L2)
- Lasso Regression (L1)
- K-Nearest Neighbors (KNN) Regression
- Cross-Validation and Feature Scaling (StandardScaler)
- Hyperparameter Tuning with `GridSearchCV`

---

## 📈 Key Findings
- **Lasso Regression** slightly outperformed others on test and CV scores.
- **Socioeconomic factors** (CalWorks %, average income) were strong predictors.
- **Feature scaling** was critical for KNN performance.
- All models explained ~77–79% of variance in test scores.

---

## 🧰 Tools Used
- Python (Jupyter Notebook)
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 🧠 What I Learned
- How to compare multiple regression models and interpret their coefficients
- The importance of feature scaling in distance-based models like KNN
- Regularization can improve model generalizability by shrinking unimportant coefficients
- How to evaluate models using training/test split and k-fold cross-validation

---

## 📎 Future Ideas
- Try ensemble methods (Random Forest, XGBoost)
- Explore fairness metrics (e.g., does model error correlate with economic disadvantage?)
- Extend to other education datasets (e.g., OECD PISA scores)

---

