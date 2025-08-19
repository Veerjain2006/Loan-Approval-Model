# Loan-Approval-Model
Loan Approval model based on data through an online survey found on (path = kagglehub.dataset_download("burak3ergun/loan-data-set")
It takes in applicant information such as income, co-applicant income, loan amount, credit history, and other factors, and predicts whether a loan application is likely to be approved or rejected.

🔹 Features
* Preprocessing with handling of missing values and feature scaling (MinMaxScaler). <br>
* Machine learning models implemented: Decision Tree and Logistic Regression. <br>
* Evaluation using metrics such as accuracy score, confusion matrix, and classification report. <br>
* Visualization of applicant distributions with Seaborn and Matplotlib.

A concise machine-learning pipeline that predicts **loan approval** using applicant data. The project covers **data cleaning, one‑hot encoding, imputation**, and model training with **Decision Tree** and **Logistic Regression**.

## What this repo shows
- **Data prep**
  - Dropped non-informative IDs (e.g., `Loan_ID`).
  - **Imputed** missing values (median for numeric, most-frequent for categorical).
  - **One‑hot encoded** categorical features.
  - (Optional) Scaled numeric features with `MinMaxScaler`.
- **Models**
  - **Decision Tree Classifier** (regularized with `max_depth`, `min_samples_leaf`).
  - **Logistic Regression** (`solver='saga'`, `max_iter` increased for convergence).
- **Evaluation**
  - Train/test split.
  - **Accuracy**, **confusion matrix**, and **classification report** (precision/recall/F1).
- **Usage**
  - Predict on **new applicants** with the same feature order as training data.
