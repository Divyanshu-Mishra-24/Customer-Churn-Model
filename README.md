# Predictive Analysis of Customer Churn for a Subscription Service


## Project Overview
This project aims to develop a predictive model that can identify customers at high risk of churning from a subscription-based service using machine learning techniques. By analyzing customer data, we aim to understand key factors contributing to churn and create a model that helps businesses retain their valuable customers by predicting churn before it occurs.

## Objective 
- Build a predictive model to classify customers as high-risk or low-risk for churn.
- Identify important factors influencing churn (e.g., customer demographics, usage patterns, engagement).
- Provide actionable insights for improving customer retention.

## Technologies Used
 **Programming Language**: Python
- **Libraries**:
  - `pandas` for data manipulation and analysis
  - `numpy` for numerical operations
  - `matplotlib` for data visualization
  - `seaborn` for advanced statistical visualizations
  - `sklearn` for building machine learning models
  - `tensorflow` for building deep learning models
 
     - ## Data

The dataset consists of customer information for a subscription service, including the following features:

- **Gender** (`object`): Gender of the customer.
- **SeniorCitizen** (`int64`): Indicates whether the customer is a senior citizen (1 if yes, 0 if no).
- **Partner** (`object`): Whether the customer has a partner (Yes/No).
- **Dependents** (`object`): Whether the customer has dependents (Yes/No).
- **Tenure** (`int64`): The number of months the customer has been with the company.
- **PhoneService** (`object`): Whether the customer has phone service (Yes/No).
- **MultipleLines** (`object`): Whether the customer has multiple lines (Yes/No).
- **InternetService** (`object`): The type of internet service the customer has (DSL/Fiber optic/None).
- **OnlineSecurity** (`object`): Whether the customer has online security (Yes/No).
- **OnlineBackup** (`object`): Whether the customer has online backup (Yes/No).
- **DeviceProtection** (`object`): Whether the customer has device protection (Yes/No).
- **TechSupport** (`object`): Whether the customer has tech support (Yes/No).
- **StreamingTV** (`object`): Whether the customer has streaming TV (Yes/No).
- **StreamingMovies** (`object`): Whether the customer has streaming movies (Yes/No).
- **Contract** (`object`): The type of contract the customer has (Month-to-month/One year/Two year).
- **PaperlessBilling** (`object`): Whether the customer uses paperless billing (Yes/No).
- **PaymentMethod** (`object`): The customer's payment method (Electronic check/Mailed check/Bank transfer/credit card).
- **MonthlyCharges** (`float64`): The amount the customer pays monthly.
- **TotalCharges** (`object`): The total charges the customer has paid (might require data cleaning).
- **Churn** (`object`): Whether the customer has churned (Yes/No).

  ## Approach

1. **Data Preprocessing**:
   - Handle missing values, especially in `TotalCharges`.
   - Convert categorical columns to numerical representations.
   - Normalize or scale numerical features (e.g., `MonthlyCharges` and `Tenure`).

2. **Exploratory Data Analysis (EDA)**:
   - Visualize the distribution of key variables and churn rates.
   - Perform correlation analysis to identify key drivers of churn.

3. **Model Development**:
   - Train multiple machine learning models such as:
     - Logistic Regression
     - Decision Trees
     - Random Forest
     - Gradient Boosting Machines (GBM)
     - Neural Networks using `tensorflow`
   - Tune hyperparameters using grid search or random search.
   - Evaluate models using metrics like accuracy, precision, recall, F1-score, and AUC-ROC.

4. **Model Evaluation**:
   - Evaluate the final model on a test dataset.
   - Analyze confusion matrix to understand false positives and negatives.
   - Use SHAP or feature importance to identify key factors influencing churn.

## Results

- An overview of the performance of each model on the test set.
- Key factors influencing churn identified.
- Recommendations for retention strategies based on the analysis.
