# Loan Approval Prediction

## Project Overview

This project focuses on building a machine learning model to predict whether a loan application will be approved or rejected based on applicant financial and demographic information.

The project demonstrates a complete supervised machine learning workflow including:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Handling missing values
* Encoding categorical variables
* Feature scaling
* Handling class imbalance using SMOTE
* Model training and evaluation
* Business interpretation of model outputs

The objective is to help financial institutions make faster, more accurate, and risk-aware loan approval decisions.

---

## Dataset

Dataset Source:

Kaggle Loan Approval Prediction Dataset

The dataset contains applicant information such as:

* Applicant income
* Co-applicant income
* Loan amount
* Loan term
* Credit history
* Education
* Property area
* Marital status

### Target Variable

`Loan_Status`

* Approved
* Rejected

---

## Technologies Used

* Python 3.x
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Imbalanced-learn (SMOTE)
* Jupyter Notebook

---

## Project Workflow

### 1. Data Loading

* Loaded dataset using Pandas
* Verified dataset structure and column types

### 2. Exploratory Data Analysis (EDA)

Performed:

* Missing value analysis
* Data type inspection
* Summary statistics
* Distribution analysis

### 3. Data Visualization

Created visualizations including:

* Loan approval distribution
* Applicant income distribution
* Education vs loan approval
* Correlation heatmap
* Confusion matrix
* ROC curve
* Feature importance chart

### 4. Data Preprocessing

Implemented:

* Missing value imputation
* One-hot encoding for categorical variables
* Feature scaling using StandardScaler

### 5. Handling Class Imbalance

Used:

* SMOTE (Synthetic Minority Oversampling Technique)

### 6. Model Building

Trained and evaluated:

* Logistic Regression
* Random Forest Classifier

### 7. Model Evaluation

Evaluation metrics used:

* Precision
* Recall
* F1 Score
* ROC-AUC

---

## Model Performance

| Model               | Precision | Recall | F1 Score | ROC-AUC |
| ------------------- | --------- | ------ | -------- | ------- |
| Logistic Regression | 0.863     | 0.965  | 0.911    | 0.869   |
| Random Forest       | 0.838     | 0.976  | 0.902    | 0.785   |

### Best Performing Model

Logistic Regression achieved the best overall performance based on ROC-AUC and F1 Score.

---

## Feature Importance Insights

The most influential features affecting loan approval were:

* Credit History
* Applicant Income
* Loan Amount
* Coapplicant Income
* Property Area

### Key Business Insights

* Applicants with strong credit history had significantly higher approval probability.
* Higher and stable income levels improved approval chances.
* Smaller loan amounts were associated with lower lending risk.
* Logistic Regression provided a strong balance between approval accuracy and risk reduction.

---

## Business Interpretation

The machine learning model successfully predicts loan approval outcomes using borrower financial and demographic information.

The project demonstrates how machine learning can assist banks and financial institutions in:

* Reducing risky loan approvals
* Improving approval consistency
* Supporting faster decision-making
* Identifying reliable borrowers

A deployment threshold of 0.6 is recommended to reduce financial risk and improve approval quality.

---

## Project Structure

```text
loan-approval-prediction/
│
├── data/
│   └── loan_prediction.csv
│
├── notebooks/
│   └── Loan_Approval_Prediction.ipynb
│
├── images/
│
├── report/
│   └── Loan_Approval_Report.pdf
│
├── README.md
│
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/loan-approval-prediction.git
```

Move into the project folder:

```bash
cd loan-approval-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Loan_Approval_Prediction.ipynb
```

Run all cells sequentially.

---

## Future Improvements

Possible future enhancements:

* Hyperparameter tuning
* XGBoost implementation
* Deployment using Flask or Streamlit
* Real-time loan approval API
* Model explainability using SHAP

---

## Conclusion

This project successfully developed a machine learning pipeline for loan approval prediction using preprocessing, class imbalance handling, model training, and evaluation techniques.

Among the evaluated models, Logistic Regression achieved the best balance between predictive performance and reliability.

The project demonstrates the practical application of machine learning in financial risk assessment and decision support systems.

---

## Author

SPANDANA NOMULA

---

## License

This project is for educational and learning purposes.
