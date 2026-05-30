# Banking Transaction Fraud Detection and Risk Analytics

<img width="1449" height="804" alt="Frau detection dashbord" src="https://github.com/user-attachments/assets/ab4483fb-69ff-4a4e-a0a8-b28e1f814165" />

## Project Overview

This project analyzes banking transaction data to identify fraud patterns, classify transaction risk, and build a machine learning-driven fraud detection workflow using Python and Power BI.

The goal was to move beyond basic reporting and create a full analytics pipeline covering:

- Data cleaning
- Exploratory data analysis
- Fraud pattern discovery
- Risk segmentation
- Machine learning fraud prediction
- Power BI dashboard reporting

## Dataset Overview

The dataset contains banking transaction records with customer activity, transaction behavior, device risk, authentication details, and fraud indicators.

Key fields included:

- transaction_id
- transaction_amount
- login_attempts
- device_risk_score
- transfer_frequency
- anomaly_score
- account_age_days
- transaction_time_hour
- failed_transactions_last_30d
- avg_monthly_balance
- daily_transaction_count
- geo_distance_km
- session_duration_minutes
- transaction_velocity_score
- payment_channel
- authentication_type
- card_present_flag
- international_transaction_flag
- suspicious_ip_flag
- fraud_flag

The target column was `fraud_flag`, which identifies whether a transaction was fraudulent or non-fraudulent.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Power BI
- DAX

## Python Workflow

### 1. Data Loading and Inspection

The dataset was loaded using Pandas and inspected to understand:

- Number of rows and columns
- Column names
- Data types
- Missing values
- Duplicate records

### 2. Data Cleaning

The cleaning process included:

- Removing duplicate records
- Checking missing values
- Creating readable fraud categories
- Creating risk-level segmentation
- Preparing the dataset for dashboard reporting

### 3. Exploratory Data Analysis

Python was used to analyze:

- Total transactions
- Fraud transactions
- Fraud rate
- Fraud amount
- Average transaction value
- Fraud by payment channel
- Fraud by authentication type
- Fraud by hour of day
- Risk-level distribution

### 4. Machine Learning Model

A Random Forest Classifier was trained to predict fraudulent transactions.

The model workflow included:

- Feature selection
- Encoding categorical variables
- Train-test split
- Model training
- Prediction
- Accuracy evaluation
- Classification report
- Confusion matrix
- Feature importance analysis

The model helped identify the strongest fraud prediction factors such as anomaly score, transaction velocity, device risk, suspicious IP activity, and failed transactions.

### 5. Export for Power BI

The cleaned dataset was exported from Python with additional prediction fields such as:

- predicted_fraud
- fraud_probability
- fraud_probability_percent
- predicted_fraud_category
- ml_risk_band

This final dataset was used to build the Power BI dashboard.

## Power BI Dashboard

The Power BI dashboard provides a clear executive view of banking fraud risk.

### Dashboard KPIs

The top KPI cards show:

- Total Transactions
- Fraud Transactions
- Fraud Rate %
- Fraud Amount
- Average Transaction
- High Risk Alerts

### Dashboard Visuals

The dashboard includes:

- Fraud Overview
- Fraud by Payment Channel
- Fraud by Authentication Type
- Fraud by Hour of Day
- Fraud Risk Level Cards
- Fraud by Risk Level

## Key Insights

- Out of 10,000 transactions, 1,251 were flagged as fraudulent.
- The overall fraud rate was 12.51%.
- Fraud exposure reached $15.66M.
- Mobile App transactions recorded the highest fraud count.
- OTP authentication had the highest fraud occurrence among authentication methods.
- Critical Risk transactions formed a major share of fraud risk alerts.
- Fraud activity varied significantly by hour of day, showing time-based risk patterns.

## Business Value

This project helps financial institutions:

- Detect suspicious transactions earlier
- Monitor fraud exposure by channel
- Identify weak authentication methods
- Prioritize high-risk alerts
- Support fraud investigation teams
- Improve risk-based decision-making
- Combine machine learning with business intelligence reporting

## Project Files

- Python Notebook: Fraud detection, EDA, machine learning, and export process
- Power BI Dashboard: Executive fraud risk monitoring dashboard
- CSV Dataset: Banking transaction data
- Dashboard Image: Final Power BI dashboard screenshot

## Author

**Ekisa Joel Jenkins**  
Data and Business Analyst  
Email: joeljenkinsekisa@gmail.com  
GitHub: https://github.com/joeljenkinsekisa
