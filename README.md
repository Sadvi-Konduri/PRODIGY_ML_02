# Task 02 : Customer Segmentation using K-means Clustering

## Objective
The objective of this task is to implement a K-means clustering algorithm to group customers of a retail store based on their purchase history. 

## Dataset
The dataset used in this project is `Mall_Customers.csv`, which contains information about customers, including:
- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

## Steps Implemented

### 1. Data Loading and Exploration
- Loaded the `Mall_Customers.csv` dataset using Pandas.
- Explored the structure and content of the dataset to understand the features.

### 2. Data Preprocessing
- Checked for missing values and handled them by forward filling.
- Checked for infinite values and ensured data integrity.
- Selected relevant features (`Annual Income (k$)` and `Spending Score (1-100)`).
- Standardized the features using `StandardScaler`.

### 3. Optimal Number of Clusters
- Used the elbow method to determine the optimal number of clusters by plotting the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters.

### 4. K-means Clustering
- Applied K-means clustering with the optimal number of clusters (K=5).
- Assigned clusters back to the original data.

### 5. Cluster Visualization
- Visualized the clusters with different colors and centroids.

### 6. Cluster Analysis
- Displayed sample data points from each cluster.
- Calculated and displayed summary statistics for each cluster.

## Visualization
The project includes detailed visualizations such as:
- Elbow curve to determine the optimal number of clusters.
- Scatter plot of clusters with different colors and centroids.

## Summary Statistics
The project calculates summary statistics for each cluster, including:
- Mean and standard deviation of Age
- Mean and standard deviation of Annual Income
- Mean and standard deviation of Spending Score
- Number of customers in each cluster

## Results
The `Mall_Customers_Clustered.csv` file contains the customer data with the added cluster information. Each row includes:
- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer in thousands of dollars.
- **Spending Score (1-100)**: Spending score assigned to the customer.
- **Cluster**: The cluster assignment for each customer, indicating which group they belong to based on the K-means clustering.
