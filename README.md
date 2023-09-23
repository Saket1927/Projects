# Telco-customer-churn-prediction
A classification machine learning problem for predicting customers churn from the company based on customers who left within the last month labeled by 'yes' or 'no'

The dataset used in this project is obtained from [Kaggle - Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)\
The data set includes information about:
- Customers who left within the last month – the column is called Churn
- Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies.
- Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
- Demographic info about customers – gender, age range, and if they have partners and dependents

## Methodology

## Data cleaning
* Convert 'TotalCharges' column which is of object type to float type using pd.to_numeric() with errors parameter set to 'coerce' to parse invalid data to NaN.
* Eight missing values were found in the 'TotalCharges' column and were imputed by the mean() value.
* Data has no duplicates.

## Exploratory data analysis

-Data Understanding
-Summary Statistics
-Missing Values
-Unique values in collumn and their count.
-Total Churn vs Total Customers
-Churn rate by Gender
-Churn rate by Senior Citizen
-Based on Partner status
-Based on Dependent status

## Feature encoding 
Several encoding techniques were tested on each categorical feature separately and One-Hot encoding all the categorical features gave the best results.

## Feature engineering
Binning 'tenure' feature into 6 ranges:
* 0-12 months --> '0-1 years'
* 12-24 months --> '1-2 years'
* 24-36 months --> '2-3 years'
* 36-48 months --> '3-4 years'
* 48-60 months --> '4-5 years'
* More than 60 months --> 'more than 5 years'

## Key Highlights


>> Based on the observations made so far, the key takeaways or highlights are:

>> Tenure and Contract duration seems to be strong factors in determining churn.

>> Among service types, phone service seems to be most popular.

>> CSP should investigate if customers receiving digital invoice have any concern with understanding the bill details.

>> Also, they should encourage customers to move to automated payment modes to improve customer experience.

>> Gender does not play an important role. However, CSPs should take care of the experience of senior citizens.

  
