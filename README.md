## Credit Scoring Model

## Introduction
Credit scoring is crucial for financial institutions to assess the creditworthiness of individuals. This project utilizes machine learning techniques to predict credit scores based on financial and demographic data.

The primary goal is to build, evaluate, and compare models for accurate predictions using:

-Random Forest Classifier

-----

## Dataset
The dataset consists of financial and demographic attributes, including:

-Age

-Occupation

-Annual Income

-Monthly In-hand Salary

-Number of Bank Accounts

-Credit Utilization Ratio

-Outstanding Debt

-Payment Behavior

-Credit Score (Target Variable)

The dataset is split into train.csv and test.csv for model training and evaluation.

-----

## Models Used
**RandomForestClassifier**:
-An ensemble method combining multiple decision trees.

-Provides better generalization and reduces overfitting.

-----

## Project Workflow
**Data Preprocessing**:

Dropped unnecessary columns (ID, Customer_ID, Name, SSN, Month).

Converted numerical columns stored as objects.

Handled missing values using mode (for categorical) and median (for numerical features).

**Feature Encoding and Scaling**:

Label encoding for categorical variables.

Standard scaling for numerical features.

**Model Training and Evaluation**:

Split the data into training and testing sets.

Trained the Random Forest Classifier.

Evaluated performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.

-----

## Dependencies
Install the required libraries using the following command:

pip install -r requirements.txt

-----

## Requirements
Python 3.7+

pandas

numpy

scikit-learn

matplotlib

seaborn

-----


## Results
The models were evaluated using the following metrics:

**Accuracy**

**Precision**

**Recall**

**F1-score**

**ROC-AUC**
