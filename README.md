# Mall Customer Segmentation using K-Means Clustering

![GitHub](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-orange)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-yellow)

## Table of Contents
1. [Overview](#overview)
2. [Problem Statement](#problem-statement)
3. [Dataset Description](#dataset-description)
4. [Objectives](#objectives)
5. [Methodology](#methodology)
   - [Data Preprocessing](#data-preprocessing)
   - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - [Modeling](#modeling)
6. [Results](#results)
7. [Future Work](#future-work)

---

## Overview

Customer segmentation is a critical marketing strategy that enables businesses to identify distinct customer groups based on their behaviors and characteristics. In this project, we use the **K-Means clustering algorithm** to group mall customers based on their **Annual Income** and **Spending Score**. The goal is to help businesses tailor their marketing efforts to specific customer segments.

---

## Problem Statement

Understanding customer behavior is key to improving marketing strategies, optimizing product placement, and increasing overall sales. This project addresses the need for segmenting mall customers into meaningful groups to enable targeted marketing campaigns based on income and spending patterns.

---

## Dataset Description

The dataset used in this project contains information about mall customers, including their **Age**, **Annual Income**, and **Spending Score**. The key attributes are:

- **CustomerID**: Unique identifier for each customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Customer's annual income in thousands of dollars.
- **Spending Score (1-100)**: A score assigned based on spending behavior, ranging from 1 to 100.

---

## Objectives

1. **Perform customer segmentation** using the K-Means clustering algorithm.
2. **Identify distinct customer segments** based on their spending behavior and income.
3. **Visualize the clusters** to provide insights into customer types.

---

## Methodology

### Data Preprocessing
- **Handling Missing Values:** The dataset was checked for missing values and imputed using appropriate strategies where necessary.
- **Feature Scaling:** Data normalization was performed using `StandardScaler` to ensure that income and spending score features were on a similar scale.
- **Data Transformation:** The dataset was prepared and split for training, with the relevant features selected for clustering.

### Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** Basic statistics (mean, median, etc.) were used to understand the distributions of age, income, and spending scores.
- **Visualizations:** Visualizations like scatter plots and histograms were created to observe the relationships between income and spending score.

### Modeling
- **K-Means Clustering:** The K-Means algorithm was applied to the dataset to cluster customers based on their annual income and spending scores.
- **Optimal K Selection:** The optimal number of clusters (K) was determined using the Elbow Method, analyzing the inertia values.

---

## Results

### Model Performance
- **Cluster Characteristics:** The K-Means algorithm successfully divided customers into distinct clusters based on spending behavior and income.
- **Cluster Visualization:** A scatter plot was used to visualize customer segments with different colors indicating each cluster.

### Key Insights
- The clusters revealed distinct groups, such as:
  - **Low Spend, Low Income**: Customers with low spending scores and lower income.
  - **High Spend, High Income**: Customers with high spending scores and higher income.
  - **Moderate Spend, Moderate Income**: Customers with moderate levels of spending and income.
  
These insights help businesses target specific groups with tailored marketing strategies.

---

## Future Work

- **Test with More Features:** Incorporate additional features such as shopping frequency and customer preferences for a more detailed segmentation.
- **Experiment with Other Algorithms:** Compare K-Means with other clustering algorithms like DBSCAN or Hierarchical Clustering to evaluate performance.
- **Deploy the Model:** Develop an application or API to predict customer segments in real-time based on new customer data.
