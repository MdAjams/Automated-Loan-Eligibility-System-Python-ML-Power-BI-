# 🏦 Real-Time Loan Eligibility Prediction

Automating loan eligibility decisions for Dream Housing Finance using **Machine Learning** & **Exploratory Data Analysis**.

---

## 🎯 Objective

To build a classification model that predicts whether a customer is eligible for a home loan based on details submitted in the application form.  
This enables **faster**, **data-driven**, and more **consistent** loan approvals.

---

## 📁 Project Structure


---

## 📊 Dataset Description

Located in the `data/` folder:

| Feature            | Description                                |
|--------------------|--------------------------------------------|
| Loan_ID            | Unique Loan ID                             |
| Gender             | Male / Female                              |
| Married            | Applicant married (Y/N)                    |
| Dependents         | Number of dependents                       |
| Education          | Graduate / Under Graduate                  |
| Self_Employed      | Self-employed (Y/N)                        |
| ApplicantIncome    | Income of applicant                        |
| CoapplicantIncome  | Income of co-applicant                     |
| LoanAmount         | Loan amount (in thousands)                 |
| Loan_Amount_Term   | Loan repayment term (in months)            |
| Credit_History     | Meets credit guidelines (1 = Yes, 0 = No)  |
| Property_Area      | Urban / Semi Urban / Rural                 |
| Loan_Status        | Target: Loan approved (Y/N) *(train only)* |

- **Train dataset**: `train.csv`  
- **Test dataset**: `test.csv` *(for predictions)*

---

## 🔍 Exploratory Data Analysis (EDA)

Visual insights generated from `train.csv`

📷 **EDA Preview**  
![EDA](images/eda_plot.png)

📷 **Feature Importance**  
![Feature Importance](images/feature_importance.png)

📷 **Dashboard (Excel / Power BI)**  
![Dashboard](images/dashboard.png)

---

## 🧠 Model Building

Steps followed in `notebooks/model_building.ipynb`:

- Baseline model using **Logistic Regression** (with class weights)
- Tree-based models: **Random Forest** and **XGBoost**
- Hyperparameter tuning with **GridSearchCV**
- Final model selection based on **F1 Score**

🏆 **Final Model**: `RandomForestClassifier`  
💾 Saved as: `models/loan_eligibility.pkl`

---

## 🚀 Prediction

`loan_predict.py` is a script to load `test.csv` and generate predictions.

### Usage:

```bash
python loan_predict.py


---

## 📊 Dataset Description

Located in the `data/` folder:

| Feature            | Description                                |
|--------------------|--------------------------------------------|
| Loan_ID            | Unique Loan ID                             |
| Gender             | Male / Female                              |
| Married            | Applicant married (Y/N)                    |
| Dependents         | Number of dependents                       |
| Education          | Graduate / Under Graduate                  |
| Self_Employed      | Self-employed (Y/N)                        |
| ApplicantIncome    | Income of applicant                        |
| CoapplicantIncome  | Income of co-applicant                     |
| LoanAmount         | Loan amount (in thousands)                 |
| Loan_Amount_Term   | Loan repayment term (in months)            |
| Credit_History     | Meets credit guidelines (1 = Yes, 0 = No)  |
| Property_Area      | Urban / Semi Urban / Rural                 |
| Loan_Status        | Target: Loan approved (Y/N) *(train only)* |

- **Train dataset**: `train.csv`  
- **Test dataset**: `test.csv` *(for predictions)*

---

## 🔍 Exploratory Data Analysis (EDA)

Visual insights generated from `train.csv`

📷 **EDA Preview**  
![EDA](images/eda_plot.png)

📷 **Feature Importance**  
![Feature Importance](images/feature_importance.png)

📷 **Dashboard (Excel / Power BI)**  
![Dashboard](images/dashboard.png)

---

## 🧠 Model Building

Steps followed in `notebooks/model_building.ipynb`:

- Baseline model using **Logistic Regression** (with class weights)
- Tree-based models: **Random Forest** and **XGBoost**
- Hyperparameter tuning with **GridSearchCV**
- Final model selection based on **F1 Score**

🏆 **Final Model**: `RandomForestClassifier`  
💾 Saved as: `models/loan_eligibility.pkl`

---

## 🚀 Prediction

`loan_predict.py` is a script to load `test.csv` and generate predictions.

### Usage:

```bash
python loan_predict.py

