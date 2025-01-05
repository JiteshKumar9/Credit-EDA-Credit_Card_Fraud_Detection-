# Credit-EDA-Credit_Card_Fraud_Detection-

# Loan Application Data Analysis

## Project Overview

This repository contains an analysis of loan application data. The dataset used includes various attributes of applicants, such as personal details, credit history, and application information. The goal of this project is to explore and analyze the data, uncover patterns, and provide insights into loan application behaviors, defaults, and approvals.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Data Analysis and Exploration](#data-analysis-and-exploration)
- [Key Insights](#key-insights)
- [Data Visualizations](#data-visualizations)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Dataset Description

The dataset contains information about loan applications, including:

- **Applicant Information**: Gender, marital status, education, family status, etc.
- **Loan Information**: Credit amount, loan type, annuity, etc.
- **Application Status**: The outcome of the loan application (approved, refused, etc.)
- **Time Variables**: Application start time, weekday, hour, etc.

### Columns:
- `AMT_INCOME_TOTAL`: Total income of the applicant.
- `AMT_CREDIT`: Credit amount requested by the applicant.
- `AMT_ANNUITY`: Annuity for the loan.
- `AMT_GOODS_PRICE`: Goods price associated with the loan.
- `NAME_CONTRACT_STATUS`: Status of the loan application (approved, refused, etc.)
- `WEEKDAY_APPR_PROCESS_START`: Weekday when the application was processed.
- `HOUR_APPR_PROCESS_START`: Hour when the application was processed.

## Data Analysis and Exploration

The analysis involves several key steps:

1. **Data Cleaning**: 
   - Missing values were handled by dropping irrelevant columns and imputing data where necessary.
   - Outliers were identified in columns like `AMT_INCOME_TOTAL`, `AMT_CREDIT`, and `AMT_ANNUITY`.

2. **Exploratory Data Analysis (EDA)**:
   - Univariate analysis of numerical and categorical variables to understand the distribution of data.
   - Bivariate analysis to explore relationships between variables like `AMT_CREDIT` and `AGE_CATEGORY`.
   - Correlation analysis to identify patterns between different financial attributes.

3. **Categorization**:
   - `AMT_CREDIT` was categorized into bins to understand the credit distribution among applicants.
   - `AMT_GOODS_PRICE` was categorized based on quantiles for better insight into goods pricing.

4. **Data Imbalance**:
   - Identified a significant imbalance in the target variable, with most applications being approved.

## Key Insights

- **Data Imbalance**: A significant imbalance exists in the target variable, with most applications being approved, and a small percentage of applications being refused or canceled.
- **Income and Credit Amount**: Applicants with higher income tend to request higher credit amounts.
- **Time of Application**: Applications submitted during specific hours and weekdays show trends that could influence loan approval.
- **Age and Credit Amount**: Younger applicants tend to request lower credit amounts compared to older applicants.

## Data Visualizations

The following visualizations were created to better understand the data:

- **Pie Charts**: To show the distribution of categorical variables like `NAME_CONTRACT_STATUS`, contract type, etc.
- **Histograms**: To visualize the distribution of numerical variables like `AMT_CREDIT`, `AMT_INCOME_TOTAL`, and `AMT_ANNUITY`.
- **Correlation Heatmaps**: To visualize the relationships between numerical variables.
- **Box Plots**: To detect outliers in financial variables like `AMT_CREDIT`, `AMT_ANNUITY`, etc.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/loan-application-analysis.git
2. Navigate to the project directory:
  ```bash
  
  `cd loan-application-analysis

3. Install the required dependencies:
  ```bash
  pip install -r requirements.txt

4. Usage
  Once the dependencies are installed, you can run the analysis by executing the following Python script:
  ```bash
  python loan_application_analysis.py
This will execute the data analysis and generate visualizations based on the dataset.

## **Contributing**
If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Please make sure to follow the coding standards and write tests for any new functionality you add.
