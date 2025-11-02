# Customer-Segmentation
*An **unsupervised ML** project using **K-Means Clustering** for **Customer Segmentation**. Groups customers into distinct profiles based on **Age**, **Annual Income**, and **Spending Score**. Highlights feature standardization and visualization for marketing and business strategy insights.*

## Overview
This project employs **unsupervised machine learning** to perform **Customer Segmentation**. It uses the **K-Means Clustering** algorithm to group customers into distinct, meaningful segments based on a combination of behavioral and demographic features: **Age**, **Annual Income**, and **Spending Score**. The output is crucial for businesses aiming to optimize marketing and personalization efforts.

## Goal
The goal is to discover underlying, non-obvious patterns in customer data by clustering individuals with similar attributes. This allows a business to define and characterize each segment (e.g., "High-Value Spenders" vs. "Budget-Conscious Individuals") for targeted strategic planning.

## Methodology
The clustering pipeline involves three critical stages:
1. **Feature Selection**: Identifying the numerical features essential for calculating distances between customers: `Age`, `Annual_Income(k$)`, and `Spending_Score(1-100)`.
2. **Data Preprocessing**: Applying StandardScaler to ensure all features are weighted equally. This normalization is mandatory for distance-based algorithms like K-Means.
3. **Clustering**: Running the **K-Means** algorithm (set to $k=3$) on the scaled data to assign each customer to a cluster.
4. **Analysis & Visualization**: Appending the cluster labels back to the original data and plotting the results to interpret the characteristics of the segments.

## Features
- **Unsupervised Learning**: Application of the **K-Means Clustering** algorithm.
- **Customer Segmentation**: Groups customers into distinct profiles for targeted analysis.
- **Feature Standardization**: Uses `StandardScaler` to ensure all features are weighted equally.
- **Visualization**: Generates scatter plots showing the clusters in the feature space for visual interpretation.

## Results and Metrics
Since K-Means is unsupervised, evaluation is based on internal metrics and visual inspection:
- **Cluster Labels**: Each data point is assigned a cluster ID (e.g., $0, 1, 2$), indicating its segment.
- **Visual Separation**: The scatter plots demonstrate the degree of separation and compactness of the generated clusters.
- **Segment Characteristics**: The final step involves inspecting the mean values of the features within each cluster to define the characteristics of the discovered segments.

## Tech Stack
The following libraries were used to implement the clustering solution:
| Tool | Purpose |
|------|---------|
|**Python**|Primary programming language for implementing clustering.|
|**`scikit-learn`**|Used for **K-Means Clustering** and the **`StandardScaler`** for normalization.|
|**`pandas`**|Used for handling the initial customer dataset and analysis.|
|**`matplotlib`**|Used for plotting the final clusters for analysis.|
|**`numpy`**|Core library for data manipulation.|

## Prerequisites
- **Python 3.x** environment.
- Required Python packages (listed in **Installation**).

## Installation
**Clone the repository and install the dependencies:**

1. #### Clone the repository
```bash
git clone https://github.com/Tanmay2923/Customer-Segmentation.git
```

2. #### Install necessary Python libraries
```bash
pip install pandas scikit-learn matplotlib numpy
```

## Running the Application
The analysis is executed via a Jupyter/Colab notebook.
1. Open the file `Customer Segmentation` in Google Colab or a local Jupyter Notebook environment.
2. Execute all cells sequentially to run the full pipeline, from data loading to cluster visualization.
