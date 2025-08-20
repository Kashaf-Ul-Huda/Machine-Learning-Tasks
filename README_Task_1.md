# Task 1: Customer Segmentation

## Project Overview
This project performs **customer segmentation** using clustering techniques on a mall customer dataset. The goal is to categorize customers based on their **Annual Income** and **Spending Score** to identify distinct customer segments for targeted marketing strategies.

---

## Dataset
**Source:** Elevvo Pathways Internship Project  
**File:** `Mall_Customers.csv`  

**Key Columns:**
- `CustomerID` – Unique customer identifier  
- `Gender` – Male/Female (encoded as 0/1)  
- `Age` – Customer age  
- `Annual Income (k$)` – Annual income in thousand dollars  
- `Spending Score (1-100)` – Score assigned by the mall based on spending behavior  

**Notes:**  
- Dataset contains 200 entries.  
- No missing values in any column.  

---

## Exploratory Data Analysis (EDA)
- Descriptive statistics (mean, median, min, max) of numerical features.  
- Visualization of **Annual Income** and **Spending Score** distributions using histograms.  
- Gender encoded as **0 (Male) / 1 (Female)** for numeric processing.

---

## Feature Scaling
- Features `Annual Income` and `Spending Score` were **standardized** using `StandardScaler` for clustering algorithms.

---

## Clustering Methods
### 1. K-Means Clustering
- Optimal number of clusters determined using the **Elbow Method**.  
- `k = 5` clusters chosen.  
- Customers assigned to clusters based on similarity of income and spending score.  
- Visualized clusters using a **scatter plot** with pastel-themed colors (`Set2` palette).  

### 2. DBSCAN (Density-Based Clustering)
- **DBSCAN** used for density-based clustering to detect arbitrarily shaped clusters.  
- Parameters: `eps = 0.5`, `min_samples = 5`.  
- Visualized clusters using scatter plot (`tab10` palette).  

---

## Cluster Analysis
- Average income and spending score per cluster:

| Cluster | Annual Income (k$) | Spending Score (1-100) |
|---------|------------------|------------------------|
| 0       | 55.30            | 49.52                  |
| 1       | 86.54            | 82.13                  |
| 2       | 25.73            | 79.36                  |
| 3       | 88.20            | 17.11                  |
| 4       | 26.30            | 20.91                  |

- Cluster sizes (K-Means):

| Cluster | Number of Customers |
|---------|------------------|
| 0       | 81               |
| 1       | 39               |
| 2       | 22               |
| 3       | 35               |
| 4       | 23               |

---

## Visualizations
- Histograms of **Annual Income** and **Spending Score**.  
- Scatter plots showing customer segments for **K-Means** and **DBSCAN** clusters.  

---

## Libraries & Tools
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn (`StandardScaler`, `KMeans`, `DBSCAN`)  

---

## Key Learnings
- How to perform **customer segmentation** using clustering techniques.  
- Feature scaling is crucial for distance-based algorithms like K-Means and DBSCAN.  
- Evaluating clusters with **silhouette scores** and **visualizations**.  
- Comparison of K-Means vs DBSCAN for segmentation purposes.  

---
