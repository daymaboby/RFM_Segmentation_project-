# RFM Segmentation & Retention Strategy

## Project Overview

This project builds customer segments using RFM (Recency, Frequency, Monetary) analysis combined with additional behavioral signals. The objective is to identify customers who should receive retention attention before deploying a machine learning churn model.

## Dataset

The analysis uses customer, order, support ticket, web activity, campaign, and churn-related datasets provided in the assignment package.

## Project Structure

├── data/
│   ├── customers.csv
│   ├── orders.csv
│   ├── tickets.csv
│   ├── web.csv
│   ├── campaigns.csv
│   └── churn.csv
│
├── rfm_segmentation.ipynb
├── segments.csv
├── retention_strategy.md
├── manual_review_cases.md
├── requirements.txt
└── README.md

## Methodology

### 1. Data Preparation

* Loaded all datasets
* Checked missing values
* Converted date fields
* Verified data consistency

### 2. RFM Feature Creation

* Recency: Days since last purchase
* Frequency: Number of orders
* Monetary: Total customer spending

### 3. Additional Signals

* Support ticket count
* Refund/return rate
* Web activity
* Campaign engagement

### 4. Customer Segmentation

Customers were grouped into business-oriented segments including:

* Champions
* Loyal Customers
* At-Risk Customers
* Dormant Customers
* Discount-Sensitive Customers
* High-Value but Unhappy Customers

### 5. Retention Strategy

Each segment received a targeted retention recommendation based on spending, engagement, support history, and churn risk.

## Output Files

### segments.csv

Contains customer-level features and final segment assignments.

### retention_strategy.md

Business recommendations and campaign prioritization.

### manual_review_cases.md

Manual review of ambiguous customer cases requiring business judgment.

## Key Business Goal

Identify high-value customers, reduce churn risk, improve retention efficiency, and allocate retention budget to customers with the highest expected business impact.
initial commit
initial commit
