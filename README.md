#Loan Classification Model

##Overview
This project builds a machine learning model to predict whether a loan
application will be approved or declined based on applicant and
loan-related features.

The analysis focuses on data preprocessing, handling class imbalance,
model comparison, and evaluation to determine the most effective
approach for classification.

------------------------------------------------------------------------

##Problem Statement
Financial institutions need to assess loan applications efficiently
while minimizing risk.
Loan approval decisions depend on multiple factors such as income,
credit score, loan purpose, and financial history.

The objective of this project is to:
- Predict whether a loan application will be approved or declined
- Identify patterns that influence loan approval decisions
- Compare different machine learning models to find the best-performing
approach

------------------------------------------------------------------------

##Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- XGBoost
- Matplotlib
- Seaborn
- Google Colab

------------------------------------------------------------------------

##Project Structure
LoanClassification.ipynb # main analysis notebook
loan_data.csv # dataset (upload manually)

The Jupyter notebook contains the full pipeline from data loading to
final predictions.

------------------------------------------------------------------------

##Installation
1. Open Google Colab
2. Upload the notebook and dataset
3. Install dependencies if needed:

pip install pandas numpy scikit-learn imbalanced-learn xgboost
matplotlib seaborn

------------------------------------------------------------------------

##Usage
Run all cells in the notebook from top to bottom. The notebook will: -
Load and explore the dataset
- Handle missing values
- Perform preprocessing (encoding and scaling)
- Apply SMOTE for class imbalance
- Train and evaluate multiple models
- Predict outcomes for new input

------------------------------------------------------------------------

##Results / Output
- Tree-based models outperform linear models
- SMOTE improves minority class prediction
- XGBoost achieved the best performance
- Model can predict loan approval for new users

------------------------------------------------------------------------

##Dataset Source
Loan dataset https://www.kaggle.com/datasets/taweilo/loan-approval-classification-data
