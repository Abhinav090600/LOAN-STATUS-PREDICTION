# 🏦 Loan Status Prediction | Machine Learning

## 📌 Overview

Can machine learning help predict whether a loan application will be approved or rejected?

This project uses applicant details such as income, credit history, education and employment status to predict loan approval using a **Support Vector Machine (SVM)** classification model.

It covers data preprocessing, exploratory data analysis, model training and performance evaluation using Python.

## 🎯 Project Objective

- Identify patterns in applicant information related to loan approval.
- Prepare and analyse the loan application dataset.
- Build a machine learning classification model.
- Predict loan status and evaluate model performance.

## 🛠️ Tech Stack

- **Python** – Programming
- **Pandas & NumPy** – Data manipulation
- **Seaborn** – Data visualization
- **Scikit-learn** – Machine learning
- **Google Colab** – Development environment

## 📂 Dataset

- **Total Records:** 614
- **Total Columns:** 13
- **Records after cleaning:** 480
- **Target Variable:** `Loan_Status`

The dataset contains applicant details such as gender, marital status, dependents, education, income, loan amount, credit history and property area.

`Loan_Status` is converted into binary values:
- `Y` → 1 (Approved)
- `N` → 0 (Rejected)

## ⚙️ Project Workflow

1. **Data Exploration:** Examined dataset structure, statistics and missing values.
2. **Data Preprocessing:** Removed missing records and converted categorical variables into numerical values.
3. **EDA:** Used Seaborn visualizations to explore patterns in loan approvals.
4. **Data Splitting:** Applied a stratified 90:10 train-test split.
5. **Model Building:** Trained a Support Vector Classifier (SVM) with a linear kernel.
6. **Evaluation:** Measured model performance using accuracy score.

## 🤖 Model & Performance

**Algorithm:** Support Vector Machine (Linear Kernel)

| Metric | Accuracy |
|---|---:|
| Training Accuracy | **79.86%** |
| Testing Accuracy | **83.33%** |

The model achieved **83.33% test accuracy**, correctly classifying 40 out of 48 test records.

## 🚀 How to Run

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/Loan-Status-Prediction.git
```

**2. Install dependencies**

```bash
pip install numpy pandas seaborn scikit-learn jupyter
```

**3. Open the notebook**

```bash
jupyter notebook
```

Open `Loan_Status_Prediction.ipynb`, ensure `dataset.csv` is available at the specified path, and run the cells sequentially.

Alternatively, open the notebook directly in Google Colab.

## 📁 Repository Structure

```text
Loan-Status-Prediction/
│
├── Loan_Status_Prediction.ipynb
├── dataset.csv
└── README.md
```

## 🔮 Future Improvements

- Compare SVM with Logistic Regression and Random Forest.
- Improve missing-value handling and feature preprocessing.
- Evaluate using precision, recall, F1-score and confusion matrix.
- Perform hyperparameter tuning.
- Build an interactive system for predicting new loan applications.

## 👨‍💻 Author

**Abhinav Anand**  
B.Tech, Petroleum Engineering  
IIT (ISM) Dhanbad

---

 *Feel free to explore the project and share your feedback!*
