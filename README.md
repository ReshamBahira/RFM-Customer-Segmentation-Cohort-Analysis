# RFM-Customer-Segmentation-Cohort-Analysis
Here is the final **copy-paste ready** README.md — *no emojis, no extra formatting issues*.
You can paste this directly into your GitHub README editor.

---

# RFM Customer Segmentation and Cohort Analysis

Capstone Project Series – Project 1

This project presents an end-to-end workflow for performing RFM (Recency, Frequency, Monetary) Analysis, Customer Segmentation, K-Means Clustering, and Cohort Analysis using the Online Retail dataset from the UCI Machine Learning Repository. The project was completed by building my own analysis pipeline, with some inspiration taken from publicly available Kaggle notebooks.

---

## Project Overview

The goal of this project is to analyze transactional retail data to understand customer purchasing behavior and segment customers using both rule-based and machine learning methods. The project includes:

* Data cleaning and preprocessing
* Exploratory data analysis
* RFM feature engineering
* Manual customer segmentation using RFM rules
* K-Means clustering for unsupervised segmentation
* Cohort creation and retention analysis

This project helps demonstrate how data can be used to measure customer value, identify behavior patterns, and support marketing strategy.

---

## Dataset Information

Source: UCI Machine Learning Repository
Period: 01/12/2010 – 09/12/2011

The dataset includes the following fields:

* InvoiceNo: Unique invoice number (invoices starting with "C" indicate cancellations)
* StockCode: Product identifier
* Description: Product name
* Quantity: Number of units purchased
* InvoiceDate: Timestamp of the transaction
* UnitPrice: Price per unit
* CustomerID: Unique customer identifier
* Country: Customer’s country of residence

---

## Project Structure and Workflow

### 1. Data Cleaning and Exploratory Data Analysis

* Removed missing values and duplicates
* Filtered out cancellations and invalid quantities
* Analyzed customers, orders, products, and country-level sales
* Observed that the UK accounts for most transactions and revenue; therefore, all further analysis focuses on UK customers

---

### 2. RFM Analysis

* Calculated:

  * Recency: Days since last purchase
  * Frequency: Number of completed transactions
  * Monetary: Total spending
* Created an RFM metrics table for all UK customers
* Visualized RFM distributions to understand customer behavior

---

### 3. Rule-Based Customer Segmentation

Created customer groups using RFM scores and custom segmentation rules.
Examples of segments include:

* Champions
* Loyal Customers
* Big Spenders
* At-Risk Customers
* Lost Customers

---

### 4. K-Means Clustering

* Normalized RFM features
* Determined the optimal number of clusters using:

  * Elbow Method
  * Silhouette Score
* Trained K-Means model to segment customers
* Compared clustering results to rule-based segmentation
* Visualized clusters using scatter plots and boxplots

---

### 5. Cohort Analysis

* Created cohorts based on customer acquisition month
* Built cohort tables and retention matrices
* Analyzed month-over-month retention
* Visualized cohort retention trends

---

## Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Key Insights

* RFM scoring effectively highlights high-value customers
* K-Means clustering provides an alternative segmentation approach that aligns with business-defined segments
* Cohort analysis reveals customer retention trends and purchasing longevity
* The UK market drives the majority of revenue and customer activity


---

If you want, I can also prepare a requirements.txt file, a short LinkedIn summary, or a project banner for your GitHub repository.
