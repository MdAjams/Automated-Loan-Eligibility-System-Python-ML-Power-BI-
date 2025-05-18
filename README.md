# 🏦 Real-Time Loan Eligibility Prediction

Automating loan eligibility decisions for Dream Housing Finance using **Machine Learning** & **Exploratory Data Analysis**.

---

## 🎯 Objective

To build a classification model that predicts whether a customer is eligible for a home loan based on details submitted in the application form.  
This enables **faster**, **data-driven**, and more **consistent** loan approvals.

---

## 📁 Project Structure
loan-eligibility-prediction/
│
├── data/ # Dataset files
│ ├── train.csv
│ ├── test.csv
│
├── images/ # Visualizations & plots
│ ├── eda_plot.png
│ ├── feature_importance.png
│ ├── dashboard.png
│
├── notebooks/ # Jupyter Notebooks
│ ├── eda.ipynb
│ ├── model_building.ipynb
│
├── models/ # Saved models
│ └── loan_eligibility.pkl
│
├── submission/ # Output predictions
│ └── submission.csv
│
├── loan_predict.py # Prediction script
├── requirements.txt # Python dependencies
└── README.md # Project documentation

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

📦 Requirements
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Libraries used:
pandas

numpy

matplotlib

seaborn

scikit-learn

xgboost

joblib

shap

✅ Key Findings
Credit_History is the most important feature.

High ApplicantIncome to LoanAmount ratio improves chances.

Married graduates from semi-urban areas had higher approval rates.

Final model achieved 80%+ accuracy on validation set.

💡 Recommendations
Auto-approve applicants with strong credit history and good income-to-loan ratios.

Use model confidence scores for risk-based decision making.

Retrain model periodically with new data to improve performance.

🙋‍♂️ Author
Made with ❤️ by Md Ajam

🔗 GitHub: MdAjams

🌐 Portfolio: mdajams.github.io

📧 Email: [your-email@example.com] (optional)



