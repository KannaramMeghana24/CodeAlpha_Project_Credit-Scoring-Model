Credit Scoring Model

Overview

This repository contains a Credit Scoring Model that classifies individuals based on their creditworthiness. The model utilizes machine learning techniques, specifically a Random Forest Classifier, to predict credit scores and assess financial risk. It is designed for banks, financial institutions, and lending platforms to automate credit risk assessment.

Features

Data preprocessing and feature engineering

Handling missing values and data cleaning

Model training using Random Forest Classifier

Performance evaluation using accuracy and classification reports

Installation

Clone the repository:

git clone https://github.com/your-username/credit-scoring-model.git
cd credit-scoring-model

Install dependencies:

pip install -r requirements.txt

Dataset

The model uses two datasets:

train.csv: Training dataset containing labeled credit data.

test.csv: Test dataset for evaluating performance.

Important Features

Demographics: Age, employment status.

Financial Attributes: Annual income, outstanding debt, number of loans.

Credit History: Delayed payments, changed credit limit, monthly balance.

Usage

Load and preprocess the dataset:

python preprocess.py

Train the Random Forest model:

python train.py

Evaluate the model:

python evaluate.py

Make predictions on new data:

python predict.py --input sample_input.csv

Model Details

Algorithm: Random Forest Classifier.

Preprocessing:

Drops irrelevant columns (ID, Customer_ID, etc.).

Converts numerical columns stored as objects.

Handles missing values (mode for categorical, median for numerical).

Evaluation Metrics:

Accuracy.

Precision, Recall, F1-score.

Classification report.

Results

The model classifies individuals into three credit score categories:

Good Credit: Low risk, highly creditworthy.

Average Credit: Moderate risk, further assessment required.

Poor Credit: High risk, low creditworthiness.

Deployment

To deploy as an API:

Run the Flask/FastAPI app:

python app.py

Send a prediction request:

curl -X POST -H "Content-Type: application/json" -d '{"income": 50000, "credit_history": 2, "loan_amount": 10000}' http://localhost:5000/predict

