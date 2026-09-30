
# 💳 Credit Card Fraud & Transaction Analytics

## Scenario

A financial institution processes a large number of credit card transactions every day across different cities and merchant categories.

The organization wants to develop a **Credit Card Fraud & Transaction Analytics System** to store, manage, and analyze customer, credit card, merchant, and transaction data using a structured SQL database.

The system maintains information about:

* Customers
* Credit Cards
* Merchants
* Transactions
* Fraud Alerts

The main purpose of the project is to understand **customer spending behavior, transaction patterns, merchant activity, and potentially fraudulent transactions**.

## 1. Customers

The system stores personal and basic information about every customer, including:

* Customer ID
* Customer Name
* Gender
* Age
* Phone
* Email
* City
* State
* Customer Status
* Registration Date

A customer can own one or more credit cards and can perform multiple transactions.

## 2. Credit Cards

Customers can have different types of credit cards.

The system stores:

* Card ID
* Customer ID
* Card Number
* Card Type
* Credit Limit
* Available Limit
* Issue Date
* Expiry Date
* Card Status

Card statuses can include:

* Active
* Blocked
* Expired
* Closed

A customer can have multiple cards, allowing analysis of card usage and customer spending behavior.

## 3. Merchants

The system stores information about merchants where credit card transactions take place.

For each merchant, the system stores:

* Merchant ID
* Merchant Name
* Merchant Category
* City
* State
* Contact Number
* Merchant Status

Merchant categories may include:

* Grocery
* Shopping
* Electronics
* Travel
* Restaurants
* Online Services
* Entertainment

A merchant can have many transactions from different customers.

## 4. Transactions

Customers use their credit cards to make purchases at different merchants.

For every transaction, the system stores:

* Transaction ID
* Card ID
* Merchant ID
* Transaction Date
* Transaction Time
* Transaction Amount
* Payment Method
* Transaction Status
* Location
* Is Fraud

Transaction status can include:

* Successful
* Failed
* Declined
* Pending

The **Is Fraud** field helps identify transactions that have been marked as potentially fraudulent.

## 5. Fraud Alerts

The system records alerts generated for suspicious transactions.

For each fraud alert, the system stores:

* Alert ID
* Transaction ID
* Risk Level
* Alert Reason
* Alert Date
* Alert Status

Risk levels can include:

* Low
* Medium
* High

This table helps analyze suspicious transactions and understand common fraud patterns.

# 💳 Credit Card Fraud & Transaction Analytics – SQL Business Analysis Question Bank

## 👥 Customer Analysis

1. What is the total number of customers?
2. How many customers are Active vs Inactive?
3. How are customers distributed across different cities?
4. Which cities have the highest number of customers?
5. How many customers registered each year?
6. Which customers have the highest total spending?

## 💳 Credit Card Analysis

1. How many credit cards are there by card type and status?
2. Which customers have multiple credit cards?
3. What is the total credit limit by customer?
4. Which customers have the highest credit limits?
5. What is the average credit limit for each card type?
6. How many cards are Active, Blocked, Expired, and Closed?

## 💰 Transaction Analysis

1. What is the total number and total amount of transactions?
2. What is the average transaction amount?
3. Which customers have the highest total transaction amount?
4. Which merchants have the highest transaction activity?
5. What is the monthly transaction amount trend?
6. Which merchant categories have the highest transaction amounts?
7. What are the most frequently used payment methods?

## 🚨 Fraud Analysis

1. What is the total number of fraudulent transactions?
2. What is the total amount involved in fraudulent transactions?
3. Which merchant categories have the highest number of fraud transactions?
4. Which cities have the highest number of fraudulent transactions?
5. Which customers have multiple fraudulent transactions?
6. What is the average amount of fraudulent transactions?
7. Which transactions have been classified as High Risk?
8. What are the most common reasons for fraud alerts?

## 🏪 Merchant Analysis

1. Which merchants have the highest number of transactions?
2. Which merchants have the highest transaction amount?
3. Which merchant categories have the highest fraud count?
4. Which merchants have both high transaction activity and fraud alerts?
5. Which cities have the highest merchant transaction activity?

## 👤 Customer Spending & Fraud Relationship

1. Which customers have high spending but no fraud alerts?
2. Which customers have both high spending and fraud transactions?
3. Which customers have multiple credit cards?
4. Which customers have transactions above the average transaction amount?
5. Which customers have transactions from multiple cities?
6. Which customers have frequent transactions within a short period?

## 🧩 Customer Segmentation & Classification

1. Categorize customers into **Low, Medium, and High Spenders** based on total spending.
2. Categorize transactions into **Low, Medium, and High Value** based on transaction amount.
3. Categorize transactions into **Low, Medium, and High Risk**.
4. Classify customers based on their fraud activity.
5. Classify customers based on their credit card usage.

## 🔎 Advanced SQL & Fraud Insights

1. Rank customers by their total transaction amount.
2. Find the top 3 customers by spending in each city.
3. Find transactions whose amount is above the overall average.
4. Find customers who have more than one fraud transaction.
5. Find merchants having both high transaction activity and fraud activity.
6. Create a consolidated view showing customer, card, merchant, and transaction information.

## 📈 Financial & Fraud Performance Analysis

1. Which merchant categories have the highest total transaction amount?
2. Which card types have the highest average transaction value?
3. Which cities have the highest total spending?
4. Which cities have the highest fraud transaction amount?
5. What percentage of total transactions are fraudulent?
6. Compare successful, failed, declined, and fraudulent transactions.

## 📅 Transaction Trends & Operations

1. How many transactions were performed each month?
2. What is the monthly fraud transaction trend?
3. Which year had the highest transaction activity?
4. Which year had the highest fraud amount?
5. On which days of the week are transactions most frequently performed?
6. During which time of day do most suspicious transactions occur?
7. What is the monthly average transaction amount?



## 📊 Key Performance Indicators

* **Total Customers:** 1,000
* **Total Credit Cards:** 1,250
* **Total Transactions:** 10,000
* **Total Transaction Amount:** ₹4.85 Cr
* **Total Fraud Transactions:** 320
* **Total Fraud Amount:** ₹18.75 Lakh
* **Average Transaction Value:** ₹4,850
* **Fraud Transaction Rate:** 3.2%
* **High-Risk Transactions:** 185
* **Active Credit Cards:** 1,080

## 🎯 Project Conclusion

The **Credit Card Fraud & Transaction Analytics SQL project** provides a structured way to analyze customer spending, credit card usage, merchant activity, and transaction behavior.

The analysis can help identify **unusual transaction patterns, high-value transactions, frequently used merchants, high-risk transactions, and fraud-related activity**.

Using different SQL concepts such as **JOIN, GROUP BY, aggregate functions, CASE, subqueries, CTEs, window functions, and views**, the project can convert raw transaction data into useful analytical insights.

Overall, this project demonstrates how SQL can be used for **financial data analysis and fraud monitoring** while covering a wide range of SQL concepts.

# 💳 Credit Card Fraud & Transaction Analytics

        CREDIT CARD FRAUD & TRANSACTION ANALYTICS
                         │
                         ▼
                  SQL DATABASE
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ├── Customers  ├── Credit Cards
          ├── Merchants  └── Transactions
          │
          └── Fraud Alerts
                         │
                         ▼
                  DATA VALIDATION
                         │
          ├── Duplicate Checks
          ├── NULL Checks
          ├── Foreign Key Validation
          ├── Amount Validation
          └── Date Validation
                         │
                         ▼
                    SQL ANALYSIS
                         │
          ├── SELECT / WHERE
          ├── DISTINCT / ORDER BY
          ├── GROUP BY / HAVING
          ├── Aggregate Functions
          ├── JOIN
          ├── CASE
          ├── SUBQUERIES
          ├── WINDOW FUNCTIONS
          ├── SELF JOIN
          └── VIEWS
                         │
                         ▼
                  BUSINESS INSIGHTS
                         │
          ├── Customer Spending Insights
          ├── Credit Card Usage Insights
          ├── Transaction Insights
          ├── Fraud Detection Insights
          ├── Merchant Analysis
          └── Risk & Financial Insights
```


