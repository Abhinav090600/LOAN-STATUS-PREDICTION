🏦 Loan Status Prediction | Machine Learning


📌 Overview

Getting a loan approved depends on several factors, including an applicant's income, credit history, employment status and other financial details. But can we use machine learning to identify patterns in these factors and predict the likelihood of loan approval?

This project explores that question by building a Loan Status Prediction model using Machine Learning. Using applicant information from a loan dataset, I developed a Support Vector Machine (SVM) classification model to predict whether a loan application is likely to be approved or rejected.

The project gave me practical experience with data preprocessing, exploratory data analysis, feature preparation, model training and performance evaluation using Python.

🎯 Project Objective

The main objective is to build a classification model that can:

Analyse applicant information and identify patterns related to loan approval.

Understand the relationship between financial and personal attributes and loan status.

Predict whether a loan application will be approved or rejected.

Evaluate the model's performance using training and testing accuracy.

🛠️ Tech Stack

Technology

Purpose

Python

Programming language

NumPy

Numerical operations

Pandas

Data manipulation and preprocessing

Seaborn

Data visualization

Scikit-learn

Model training and evaluation

Google Colab

Development environment

📂 Dataset Description

The project uses a loan application dataset containing 614 records and 13 columns.

The dataset includes information about applicants, such as:

Feature

Description

Gender

Applicant's gender

Married

Marital status

Dependents

Number of dependents

Education

Graduate or non-graduate

Self_Employed

Employment status

ApplicantIncome

Applicant's income

CoapplicantIncome

Co-applicant's income

LoanAmount

Requested loan amount

Loan_Amount_Term

Loan repayment period

Credit_History

Credit history information

Property_Area

Urban, semiurban or rural

Loan_Status

Final loan approval status

Loan_ID is an identifier and is excluded from model training.

Target Variable: Loan_Status

Y → 1 (Loan Approved)

N → 0 (Loan Rejected)

After removing records containing missing values, 480 records were retained for model development.

⚙️ Project Workflow

The project follows a step-by-step machine learning workflow:

1. Data Collection and Exploration

Imported the dataset using Pandas.

Examined the dataset's dimensions, first few records and statistical information.

Identified missing values and understood the available features.

2. Data Preprocessing

Removed rows containing missing values.

Converted the target variable from categorical labels (Y, N) into numerical values (1, 0).

Converted categorical features into numerical representations.

Represented the 3+ dependents category as 4.

Removed the unnecessary Loan_ID column.

3. Exploratory Data Analysis (EDA)

Used Seaborn to visualize the relationship between applicant characteristics and loan approval.

Created count plots to examine loan status across education and marital-status categories.

Explored patterns in the applicant data.

4. Feature Selection and Data Splitting

Separated the independent variables (X) and dependent variable (Y).

Divided the dataset into training and testing sets.

Used a stratified 90:10 train-test split with random_state=2.

5. Model Building

Selected the Support Vector Machine (SVM) algorithm.

Implemented a Support Vector Classifier with a linear kernel.

Trained the model using the training dataset.

6. Model Evaluation

Generated predictions for training and testing data.

Compared predicted values with actual loan statuses.

Evaluated model performance using the accuracy score.

🤖 Machine Learning Model

Support Vector Machine (SVM)

SVM is a supervised machine learning algorithm commonly used for classification problems. It identifies an optimal decision boundary (hyperplane) that separates different classes.

In this project, a linear kernel was used to classify loan applications into two categories:

Approved

Rejected

📊 Model Performance

The model was evaluated using accuracy score on both training and testing datasets.

Evaluation Metric

Accuracy

Training Accuracy

79.86%

Testing Accuracy

83.33%

<p align="center">
  <img src="https://img.shields.io/badge/Training_Accuracy-79.86%25-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Testing_Accuracy-83.33%25-success?style=for-the-badge" />
</p>

The model achieved 83.33% accuracy on the test dataset, correctly classifying 40 out of 48 test records.

The results provide a useful starting point for understanding how machine learning can be applied to loan classification problems.

🚀 How to Run the Project

Option 1: Google Colab (Recommended)

Download or clone this repository.

Open Loan_Status_Prediction.ipynb in Google Colab.

Upload dataset.csv to the Colab session.

Make sure the dataset path is correct.

Run all cells sequentially.

Option 2: Run Locally

Step 1: Clone the repository

git clone https://github.com/YOUR-USERNAME/Loan-Status-Prediction.git

Step 2: Navigate to the project directory

cd Loan-Status-Prediction

Step 3: Install the required libraries

pip install numpy pandas seaborn scikit-learn jupyter

Step 4: Open Jupyter Notebook

jupyter notebook

Step 5: Open Loan_Status_Prediction.ipynb, ensure the dataset path is correct, and execute the notebook cells.

📁 Repository Structure

Loan-Status-Prediction/
│
├── Loan_Status_Prediction.ipynb
├── dataset.csv
└── README.md

Note: Include the dataset only if you have permission to redistribute it.

🔮 Future Improvements

There is still scope to improve this project. Some areas I would like to explore further are:

Experimenting with other classification algorithms such as Logistic Regression, Decision Trees and Random Forest.

Handling missing values through suitable imputation techniques instead of removing entire records.

Applying feature scaling and a proper preprocessing pipeline.

Evaluating the model using precision, recall, F1-score and a confusion matrix.

Performing hyperparameter tuning using cross-validation.

Developing a predictive system that accepts new applicant details and returns a loan status prediction.

👨‍💻 About Me

Abhinav Anand

B.Tech | Petroleum Engineering
Indian Institute of Technology (ISM), Dhanbad

I'm interested in exploring the applications of data analytics, programming and machine learning to solve real-world problems.
