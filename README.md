# Loan Prediction Dataset - Machine Learning Project

## 📋 Project Overview

This project focuses on building a machine learning model to predict whether a loan applicant is likely to default on a loan. Using the Loan Prediction Dataset from Kaggle, this implementation demonstrates a complete data science workflow from data exploration to model deployment.

## 🎯 Objective

Predict loan default risk using classification algorithms to help financial institutions make better lending decisions.

## 📊 Dataset Information

**Source:** [Loan Prediction Problem Dataset on Kaggle](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)

**Size:** 614 records with 13 features

### Dataset Features

| Feature | Description | Type |
|---------|-------------|------|
| Loan_ID | Unique Loan ID | Categorical |
| Gender | Applicant's gender (Male/Female) | Categorical |
| Married | Applicant's marital status (Yes/No) | Categorical |
| Dependents | Number of dependents (0,1,2,3+) | Categorical |
| Education | Education level (Graduate/Not Graduate) | Categorical |
| Self_Employed | Self employment status (Yes/No) | Categorical |
| ApplicantIncome | Applicant's income | Numerical |
| CoapplicantIncome | Co-applicant's income | Numerical |
| LoanAmount | Loan amount in thousands | Numerical |
| Loan_Amount_Term | Term of loan in days | Numerical |
| Credit_History | Credit history meets guidelines (1.0/0.0) | Numerical |
| Property_Area | Area of property (Urban/Rural/Semiurban) | Categorical |
| Loan_Status | Loan approved (Y/N) | Target Variable |

## 🛠️ Technical Implementation

### Libraries Used
- **Data Handling:** pandas, numpy
- **Visualization:** matplotlib, seaborn
- **Machine Learning:** scikit-learn
- **Data Download:** kaggle API

### Models Implemented
1. **Logistic Regression**
2. **Decision Tree Classifier**

### Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report

## 📈 Project Workflow

### 1. Data Acquisition & Setup
- Download dataset from Kaggle using API
- Extract and load data into pandas DataFrame
- Initial data inspection and structure analysis

### 2. Data Cleaning & Preprocessing
- Handle missing values:
  - Categorical features: Mode imputation
  - Numerical features: Median imputation
- Convert '3+' to 3 in Dependents column
- Remove irrelevant features (Loan_ID)

### 3. Exploratory Data Analysis (EDA)
- Loan status distribution visualization
- Loan amount distribution analysis
- Feature correlation analysis
- Categorical feature analysis

### 4. Feature Engineering
- Label encoding for categorical variables
- Data splitting into training and testing sets
- Feature scaling for numerical variables

### 5. Model Training & Evaluation
- Train multiple classification models
- Evaluate performance using accuracy and confusion matrix
- Compare model results
- Generate classification reports

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas matplotlib seaborn scikit-learn kaggle
```
## 🔧 Kaggle API Setup
1. Create Kaggle account and get API credentials

2. Place ``` kaggle.json ``` in appropriate directory

3. Set environment variable for Kaggle config
## 📁 Directory Structure
```
└── 📁 .kaggle/
    └── 🗄️ kaggle.json
```
## 🚀 Execution
Run the Jupyter notebook ``` loan_prediction_dataset.ipynb ``` sequentially:

1. 📚 Import libraries and setup environment

2. 📥 Download and extract dataset

3. 🧹 Execute data cleaning steps

4. 📊 Run EDA visualizations

5. 🤖 Train and evaluate models

## 📊 Key Findings
### Data Quality
- Dataset contains 614 samples with 13 features
- Missing values present in several columns:
  - Gender: 13 missing
  - Married: 3 missing
  - Dependents: 15 missing
  - Self_Employed: 32 missing
  - LoanAmount: 22 missing
  - Loan_Amount_Term: 14 missing
  - Credit_History: 50 missing
### Data Distribution
- Loan approval rate analysis

- Income distribution patterns

- Loan amount characteristics

- Regional distribution of applicants
  
## 💡 Business Implications

This model can help financial institutions:
- Automate loan approval processes

- Reduce default rates through better risk assessment

- Standardize lending decisions

- Improve portfolio quality
## 🔮 Future Improvements

- Implement additional algorithms (Random Forest, XGBoost)

- Feature engineering for better predictive power

- Hyperparameter tuning for model optimization

- Cross-validation for robust performance evaluation

- Deployment as a web application

## 📝 License
The dataset is available on Kaggle with unknown license. Please check Kaggle for specific usage terms.

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
  
