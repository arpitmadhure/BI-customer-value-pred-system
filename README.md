# Business Intelligence & Customer Value Prediction System

This project focuses on analyzing customer purchasing behavior using historical online retail transaction data. Customers are segmented into different value groups using the RFM (Recency, Frequency, Monetary) framework, and a Machine Learning model is trained to predict customer value based on these features.

A Streamlit application has also been developed to allow users to enter customer information and instantly predict the customer segment.

## Project Objectives

- Analyze customer purchasing behavior
- Perform data cleaning and preprocessing
- Generate customer segments using RFM analysis
- Train a Machine Learning classification model
- Build an interactive Streamlit application for prediction

## Dataset

The project uses the **Online Retail Dataset**, which contains transactional data from an online retail store.

The dataset includes:

- Invoice Number
- Product Code
- Product Description
- Quantity
- Unit Price
- Invoice Date
- Customer ID
- Country

Total Records: **541,908**

## Project Workflow

```
Raw Data
    ↓
Data Cleaning
    ↓
Exploratory Data Analysis
    ↓
RFM Feature Engineering
    ↓
Customer Segmentation
    ↓
Model Training
    ↓
Model Evaluation
    ↓
Streamlit Deployment
```

## Data Preprocessing

The following preprocessing steps were performed before training the model:

- Removed cancelled transactions
- Removed invalid quantities and prices
- Removed missing Customer IDs
- Created a Revenue feature
- Prepared customer-level RFM features

## RFM Analysis

Customers were evaluated using three metrics:

**Recency** – Number of days since the last purchase

**Frequency** – Total number of purchases

**Monetary** – Total amount spent by the customer

Based on the RFM score, customers were classified into:

- High Value
- Medium Value
- Low Value

## Machine Learning Model

**Algorithm Used**

- Logistic Regression

**Input Features**

- Recency
- Frequency
- Monetary

**Target Variable**

- Customer Segment

The model was evaluated using train-test split and cross-validation.

**Model Accuracy:** Approximately **88%**

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Streamlit
- Joblib

## Project Structure

```
Business-Intelligence-Customer-Value-Prediction/

│── app.py
│── model.pkl
│── encoder.pkl
│── requirements.txt
│── notebook.ipynb
│── README.md
```

## How to Run

Clone the repository

```bash
git clone https://github.com/your-github-username/business-intelligence-customer-value-prediction.git
```

Move into the project folder

```bash
cd business-intelligence-customer-value-prediction
```

Install the required libraries

```bash
pip install -r requirements.txt
```

Run the Streamlit application

```bash
streamlit run app.py
```

## Future Improvements

- Improve model performance using advanced algorithms
- Add interactive business dashboards
- Include additional customer behavior features
- Deploy the application on Streamlit Cloud

## Author

**Arpit Madhure**

B.Tech Computer Science & Engineering (Data Science)

GitHub: https://github.com/your-github-username
