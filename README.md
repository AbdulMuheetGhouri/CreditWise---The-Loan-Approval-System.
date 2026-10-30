# CreditWise – Loan Approval Prediction Using Machine Learning

CreditWise is a Machine Learning project that analyzes applicant financial and demographic information to predict loan approval outcomes. It applies data preprocessing, exploratory data analysis (EDA), feature engineering, and multiple classification algorithms to identify patterns associated with loan approval decisions.

The project explores and compares different machine learning models to understand their predictive performance.

## Features

- **Data Preprocessing:** Handles missing numerical and categorical values using mean and most-frequent imputation strategies.
- **Exploratory Data Analysis (EDA):** Analyzes loan approval distribution and explores relationships between applicant attributes and loan approval outcomes.
- **Data Visualization:** Uses pie charts, bar charts, box plots, and correlation heatmaps to understand the dataset.
- **Categorical Encoding:** Applies Label Encoding and One-Hot Encoding to convert categorical variables into numerical representations.
- **Feature Engineering:** Applies logarithmic transformations to income-related features and power transformations to selected numerical features.
- **Feature Scaling:** Uses StandardScaler to standardize numerical features.
- **Model Training:** Implements multiple classification algorithms.
- **Hyperparameter Tuning:** Uses GridSearchCV with 10-fold cross-validation to optimize KNN's number of neighbors.
- **Model Evaluation:** Evaluates model performance using accuracy, precision, recall, and F1-score.

## Machine Learning Algorithms

CreditWise implements three classification algorithms:

| Algorithm | Implementation |
|---|---|
| Logistic Regression | `LogisticRegression` |
| K-Nearest Neighbors (KNN) | `KNeighborsClassifier` with GridSearchCV |
| Gaussian Naive Bayes | `GaussianNB` |

The models are evaluated before and after feature engineering to examine the impact of feature transformations on predictive performance.

## Dataset Features

The project uses an applicant loan approval dataset (`approval_dataset.csv`) containing the following attributes:

| Feature | Description |
|---|---|
| Applicant_ID | Unique applicant identifier |
| Applicant_Income | Applicant's income |
| Coapplicant_Income | Co-applicant's income |
| Age | Applicant's age |
| Dependents | Number of dependents |
| Credit_Score | Applicant's credit score |
| Existing_Loans | Number of existing loans |
| DTI_Ratio | Debt-to-income ratio |
| Savings | Applicant's savings |
| Collateral_Value | Value of collateral |
| Loan_Amount | Requested loan amount |
| Loan_Term | Loan repayment term |
| Employment_Status | Applicant's employment status |
| Marital_Status | Applicant's marital status |
| Loan_Purpose | Purpose of the loan |
| Property_Area | Applicant's property area |
| Education_Level | Applicant's education level |
| Gender | Applicant's gender |
| Employer_Category | Category of employer |
| Loan_Approved | Target variable (Yes/No) |

## Project Workflow

The project follows these major steps:

1. **Data Loading:** Imports the dataset using Pandas.
2. **Data Inspection:** Examines dataset structure, statistical summaries, and missing values.
3. **Missing Value Treatment:** Imputes missing numerical values using the mean and categorical values using the most frequent value.
4. **Exploratory Data Analysis:** Investigates target distribution and relationships between applicant characteristics and loan approval.
5. **Categorical Encoding:** Converts categorical features into numerical representations.
6. **Correlation Analysis:** Examines relationships between features using correlation analysis and heatmaps.
7. **Feature Scaling:** Applies StandardScaler to prepare features for model training.
8. **Model Training and Evaluation:** Trains Logistic Regression, KNN, and Gaussian Naive Bayes classifiers.
9. **Hyperparameter Tuning:** Uses GridSearchCV to identify an optimal KNN neighbor parameter.
10. **Feature Engineering:** Applies transformations to selected features, followed by model retraining and evaluation.

## Technologies & Libraries

- **Python** – Core programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization
- **Scikit-learn** – Data preprocessing, machine learning models, hyperparameter tuning, and evaluation
- **Jupyter Notebook** – Development and experimentation environment

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/CreditWise.git
```

### 2. Navigate to the Project Directory

```bash
cd CreditWise
```

### 3. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Add the Dataset

Place `approval_dataset.csv` in the project directory alongside the notebook.

### 5. Run Jupyter Notebook

```bash
jupyter notebook
```

Open `credit_wise.ipynb` and execute the cells to explore the complete machine learning workflow.

## Model Evaluation Metrics

The project evaluates its classification models using:

- **Accuracy:** Measures the proportion of correctly classified predictions.
- **Precision:** Measures how many predicted loan approvals were actually approved.
- **Recall:** Measures how many actual loan approvals were correctly identified.
- **F1-Score:** Provides a balance between precision and recall.
```
```
## Project Objective

The primary objective of CreditWise is to explore how machine learning classification algorithms can analyze applicant information and identify patterns associated with loan approval decisions.

It also provides practical experience with the end-to-end machine learning workflow, from raw data preprocessing to model evaluation and feature engineering.

## Disclaimer

CreditWise is an educational machine learning project developed for experimentation and learning purposes. Its predictions should not be treated as actual financial advice or used as the sole basis for real-world lending decisions.
