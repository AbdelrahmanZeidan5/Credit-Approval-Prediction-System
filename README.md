# Credit Approval Prediction System

## Overview
This project implements a **Credit Approval Prediction System** using Kaggle's Credit Approval Loan Data. It evaluates five machine learning models to classify loan approvals:
- Logistic Regression
- Support Vector Machine (SVM)
- Artificial Neural Network (ANN)
- Decision Tree
- Random Forest

## Dataset
- **Source**: [Credit Approval Loan Data](https://www.kaggle.com/datasets/samanemami/credit-approval-loan/data)
- **Features**:
  - Gender, Age, Income, Loan Amount, Loan Purpose, Credit History
- **Target Variable**: Approval Status (1 for approved, 0 for denied)

## Techniques
1. **Data Preprocessing**:
   - Handled missing values (mean/mode imputation).
   - Standardized numerical features using `StandardScaler`.
   - Categorical variables encoded with one-hot encoding.
2. **SMOTE**: Used to balance the dataset for better model performance.
3. **Evaluation**:
   - 5-fold cross-validation
   - Metrics: Accuracy, Precision, Recall, F1-Score

## Results
### Model Performance (Best F1-Scores):
- **Random Forest**: 85.64%
- **ANN**: 82.70%
- **Decision Tree**: 72% (Weighted Average)
- **SVM**: 64.87%
- **Logistic Regression**: 67.54%

## Installation and Setup
1. Clone the repository:
   `git clone https://github.com/AbdelrahmanZeidan5/Credit-Approval-Prediction-System.git`

2. Navigate to the directory:
   `cd Credit-Approval-Prediction-System`

3. Install the dependencies:
   `pip install -r requirements.txt`

4. Launch the Jupyter Notebook:
   `jupyter notebook`

5. Open `Credit_Approval_Prediction.ipynb` and run all cells sequentially.

## Results Visualization
The Random Forest model performed the best, achieving an accuracy of 85.93% and an F1-score of 85.64%. The ANN model followed with an F1-score of 82.70%. Below are some model comparison graphs:

- **Accuracy**: Random Forest > ANN > Decision Tree
- **Precision**: Random Forest > ANN > SVM
- **Recall**: ANN > Random Forest > Decision Tree

## License
This project is licensed under the MIT License.
