You can launch the project through arpit-customer-value-prediction.streamlit.app # Business Intelligence & Customer Value Prediction System

This project analyzes customer purchasing behavior using an online retail transaction dataset and predicts customer value segments using Machine Learning. The project combines Business Intelligence techniques with the RFM (Recency, Frequency, Monetary) framework to classify customers into High, Medium, and Low value groups.

A Streamlit web application is included to allow users to enter customer information and predict the customer segment in real time.

## Project Objectives

- Analyze customer purchasing behavior
- Clean and preprocess raw transaction data
- Perform customer segmentation using RFM analysis
- Train a Machine Learning classification model
- Deploy the model using Streamlit

## Dataset

The project uses the **Online Retail Dataset**, which contains transaction records from an online retail store.

### Dataset Features

| Feature | Description |
|---------|-------------|
| InvoiceNo | Transaction ID |
| StockCode | Product Code |
| Description | Product Name |
| Quantity | Quantity Purchased |
| InvoiceDate | Purchase Date |
| UnitPrice | Price per Unit |
| CustomerID | Customer ID |
| Country | Customer Country |

**Total Records:** 541,908

## Workflow

```text
Raw Transaction Data
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
- Removed invalid quantity values
- Removed invalid unit prices
- Removed missing Customer IDs
- Created a Revenue feature

Revenue = Quantity × UnitPrice

## Customer Segmentation

Customers were segmented using the RFM framework.

**Recency** – Number of days since the customer's last purchase.

**Frequency** – Total number of purchases made by the customer.

**Monetary** – Total amount spent by the customer.

Based on the RFM score, customers were classified into:

- High Value
- Medium Value
- Low Value

## Machine Learning Model

**Algorithm**

Logistic Regression

**Input Features**

- Recency
- Frequency
- Monetary

**Target**

Customer Value Segment

The model was evaluated using train-test split and cross-validation.

**Accuracy:** Approximately **88%**

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

```text
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
git clone https://github.com/arpitmadhure/business-intelligence-customer-value-prediction.git
```

Go to the project directory

```bash
cd business-intelligence-customer-value-prediction
```

Install the required libraries

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run app.py
```

## Future Improvements

- Improve prediction accuracy using advanced machine learning models
- Add interactive dashboards
- Support batch customer predictions
- Deploy the application using cloud services

## Author

**Arpit Madhure**

B.Tech Computer Science & Engineering (Data Science)

GitHub: https://github.com/arpitmadhure
