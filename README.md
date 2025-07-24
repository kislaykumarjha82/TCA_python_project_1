
# Telco Customer Churn Prediction

Welcome to the **Telco Customer Churn Analysis** project! This repository contains scripts and data designed to explore, analyze, and model customer churn using a real-world telecom dataset.

<img width="1114" height="863" alt="Screenshot 2025-07-24 172643" src="https://github.com/user-attachments/assets/028de33e-02c9-4811-814d-bc4801a561a5" />
<img width="797" height="582" alt="Screenshot 2025-07-24 172634" src="https://github.com/user-attachments/assets/7a4cc13c-6cda-449f-8443-cf8b9450af30" />


## Project Overview

Customer churn is a critical metric for telecom companies, as it represents the loss of clients or subscribers. Accurately understanding and predicting churn helps to improve retention strategies, optimize marketing, and increase profitability.

This project includes:
- A detailed exploratory data analysis (EDA)
- Processing and cleaning of raw data
- Statistical summaries of key features
- A basis for building churn prediction models

## Dataset

The dataset contains detailed information about telco customers, such as demographics, services signed up for, account information, and whether they have churned.

### Key Columns

| Column             | Description                                     |
|--------------------|------------------------------------------------|
| customerID         | Unique identifier for each customer            |
| gender             | Male or Female                                 |
| SeniorCitizen      | 1 if senior citizen, 0 otherwise               |
| Partner            | Whether the customer has a partner             |
| Dependents         | Whether the customer has dependents            |
| tenure             | Number of months the customer has stayed       |
| PhoneService       | If the customer has phone service              |
| MultipleLines      | If the customer has multiple lines             |
| InternetService    | Type of internet service (DSL, Fiber optic, etc) |
| OnlineSecurity     | Whether the customer has online security       |
| DeviceProtection   | Whether the customer has device protection     |
| TechSupport        | Whether the customer has tech support          |
| StreamingTV        | If the customer has streaming TV               |
| StreamingMovies    | If the customer has streaming movies           |
| Contract           | Contract term (Month-to-month, One year, etc.) |
| PaperlessBilling   | If the customer has paperless billing          |
| PaymentMethod      | Billing payment method                         |
| MonthlyCharges     | The amount charged to the customer monthly     |
| TotalCharges       | The total amount charged                       |
| Churn              | Whether the customer churned (Yes/No)          |

### Dataset Snapshot

| customerID   | gender | SeniorCitizen | Partner | Dependents | tenure | PhoneService | MultipleLines       | InternetService | ... | DeviceProtection | TechSupport | StreamingTV | StreamingMovies | Contract        | PaperlessBilling | PaymentMethod           | MonthlyCharges | TotalCharges | Churn |
|--------------|--------|---------------|---------|------------|--------|--------------|---------------------|-----------------|-----|------------------|-------------|-------------|----------------|-----------------|------------------|-------------------------|----------------|-------------|-------|
| 7590-VHVEG   | Female | 0             | Yes     | No         | 1      | No           | No phone service    | DSL             | ... | No               | No          | No          | No             | Month-to-month  | Yes              | Electronic check        | 29.85          | 29.85       | No    |
| 5575-GNVDE   | Male   | 0             | No      | No         | 34     | Yes          | No                  | DSL             | ... | Yes              | No          | No          | No             | One year        | No               | Mailed check            | 56.95          | 1889.5      | No    |
| 3668-QPYBK   | Male   | 0             | No      | No         | 2      | Yes          | No                  | DSL             | ... | No               | No          | No          | No             | Month-to-month  | Yes              | Mailed check            | 53.85          | 108.15      | Yes   |
| 7795-CFOCW   | Male   | 0             | No      | No         | 45     | No           | No phone service    | DSL             | ... | Yes              | Yes         | No          | No             | One year        | No               | Bank transfer (automatic)| 42.30          | 1840.75     | No    |
| 9237-HQITU   | Female | 0             | No      | No         | 2      | Yes          | No                  | Fiber optic     | ... | No               | No          | No          | No             | Month-to-month  | Yes              | Electronic check        | 70.70          | 151.65      | Yes   |

## Data Summary

| Feature        | Count    | Mean      | Std        | Min      | 25%      | 50%     | 75%     | Max     |
|----------------|----------|-----------|------------|----------|----------|---------|---------|---------|
| SeniorCitizen  | 7,043    | 0.16      | 0.37       | 0        | 0        | 0       | 0       | 1       |
| tenure         | 7,043    | 32.37     | 24.56      | 0        | 9        | 29      | 55      | 72      |
| MonthlyCharges | 7,043    | 64.76     | 30.09      | 18.25    | 35.50    | 70.35   | 89.85   | 118.75  |
| TotalCharges   | 7,043    | 2,279.73  | 2,266.79   | 0.00     | 398.55   | 1,394.55| 3,786.60| 8,684.80|

## Requirements

- Python 3.7+
- Common data science libraries (pandas, numpy, matplotlib, etc.)
- Jupyter Notebook
- 
<img width="1114" height="863" alt="Screenshot 2025-07-24 172643" src="https://github.com/user-attachments/assets/f4bfa789-1ab4-4c6f-80fa-3424e8ae452f" />
<img width="1244" height="747" alt="Screenshot 2025-07-24 172552" src="https://github.com/user-attachments/assets/18f70fc3-9174-490c-902b-597f87e5adec" />
<img width="1052" height="756" alt="Screenshot 2025-07-24 172559" src="https://github.com/user-attachments/assets/acace2f4-8759-42d8-902c-df3a951e8971" />
<img width="973" height="718" alt="Screenshot 2025-07-24 172605" src="https://github.com/user-attachments/assets/c7df0657-3cf0-41be-b31a-ee3a599d4f15" />
<img width="852" height="666" alt="Screenshot 2025-07-24 172614" src="https://github.com/user-attachments/assets/28f4ea5d-eb0a-49d5-b8ee-a3589d803473" />
<img width="944" height="813" alt="Screenshot 2025-07-24 172623" src="https://github.com/user-attachments/assets/c6286885-47ed-4db8-8b42-d3e03bdebb85" />
<img width="1606" height="709" alt="Screenshot 2025-07-24 172649" src="https://github.com/user-attachments/assets/fd570746-e714-479a-96f6-74811043907b" />


## Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/telco-churn-analysis.git
   cd telco-churn-analysis
   ```
2. Open `TCA.ipynb` in Jupyter Notebook or another IDE.
3. Run the notebook step by step to:
   - Load and inspect the data
   - Perform EDA and generate summary statistics
   - Preprocess data for modeling

## Notebook Contents

- **Data Loading & Cleaning:** Handling missing values, formatting columns.
- **Exploratory Analysis:** Descriptive stats, visualizations, and insights into churn patterns.
- **Feature Overview:** Importance of customer demographics, contract type, and billing.
- **Ready for Modeling:** The notebook sets up the data for future predictive modeling tasks.

## Contributing

Contributions are welcome! Please:
- Fork the repository.
- Open pull requests for improvements or new features.
- Write clear commit messages.

## License

This project is licensed under the MIT License—see the LICENSE file for details.

*Empower your organization to reduce churn and boost customer satisfaction using data!*

Linkedin=https://www.linkedin.com/in/kislay-kumar-jha-7421b52a5/
instagram=https://www.instagram.com/priyanshujha82/?igsh=aGt6NDVhcHlhanpi#
