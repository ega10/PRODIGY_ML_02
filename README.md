# Customer Segmentation using K-Means Clustering

This project implements **K-means clustering** to segment customers of a retail store based on their features, such as **Age**, **Annual Income**, and **Spending Score**. The goal is to group customers into different segments that exhibit similar purchasing behaviors and characteristics.

## Objective

The objective of this project is to segment customers using clustering techniques, specifically K-means, to help retailers understand customer behavior and tailor marketing strategies accordingly.

## Features Used:
- **Age**: Age of the customer.
- **Annual Income (k$)**: The annual income of the customer (in thousands).
- **Spending Score (1-100)**: A score assigned to customers based on their purchasing behavior.

## Steps Involved:

1. **Data Preprocessing**:
   - Load customer data from a CSV file.
   - Clean the data by removing any irrelevant or non-numeric columns (e.g., `CustomerID`, `Gender`).
   - Handle missing values (if any) by removing or imputing them.
   - Standardize the features using `StandardScaler` to ensure that the K-means algorithm performs well.

2. **K-Means Clustering**:
   - Use the **Elbow Method** to determine the optimal number of clusters (`K`).
   - Apply the K-means algorithm to segment the customers into clusters.
   - Assign cluster labels to each customer.

3. **Visualizations**:
   - **Elbow Method**: Plot WCSS (Within-cluster sum of squares) to find the optimal number of clusters.
   - **2D Scatter Plot**: Visualize the customer segments based on `Age` and `Spending Score`.
   - **Cluster Centers**: Plot the cluster centers on the scatter plot.
   - **Pairplot**: Visualize relationships between features for different customer clusters.
   - **Correlation Heatmap**: Explore the correlation between `Age`, `Annual Income`, and `Spending Score`.
   
4. **Evaluation**:
   - Calculate the **Silhouette Score** to evaluate the quality of the clusters.

## Required Libraries:

- **pandas**: For data manipulation and loading CSV files.
- **matplotlib**: For creating visualizations like plots and scatter diagrams.
- **seaborn**: For advanced visualizations like pair plots and heatmaps.
- **scikit-learn**: For implementing the K-means clustering and scaling features.

To install the required libraries, use the following command:

```bash
pip install pandas matplotlib seaborn scikit-learn
