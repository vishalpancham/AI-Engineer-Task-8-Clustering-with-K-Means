# 🔍 Customer Segmentation using K-Means Clustering

This project uses the **K-Means Clustering** algorithm to group mall customers into distinct segments based on their **Annual Income** and **Spending Score**.

---

## 📁 Dataset

- **Name**: Mall Customers Dataset
- **Source**: Kaggle / provided file
- **Features Used**:
  - Annual Income (k$)
  - Spending Score (1–100)

---

## ✅ Workflow

### 📊 Step 1: Load and Explore Data
- Loaded `Mall_Customers.csv` into pandas DataFrame
- Checked structure and null values

### 🔍 Step 2: Feature Selection
- Selected only:
  - `Annual Income (k$)`
  - `Spending Score (1–100)`

### ⚖️ Step 3: Normalize Features
- Applied `StandardScaler` to scale both features for accurate distance calculation

### 📉 Step 4: Find Optimal K
- Used **Elbow Method** to find best value for K (number of clusters)
- WCSS (Within-Cluster Sum of Squares) plotted from K=1 to K=10

### 🤖 Step 5: K-Means Clustering
- Trained model using `K=5`
- Assigned cluster labels to each data point

### 📈 Step 6: Cluster Visualization
- Created scatter plot of clusters using Seaborn

### 🧠 Step 7: Silhouette Score
- Calculated Silhouette Score to evaluate clustering quality  
- **Result**: `0.55` → indicates good clustering

---

## 📊 Results

| Metric | Value |
|--------|--------|
| Optimal K | 5 |
| Silhouette Score | 0.5547 |
| Cluster Plot | Visualizes 5 distinct customer segments |

---

## 📂 Files Included

- `task_8_kmeans.ipynb` — Notebook with full code & plots
- `Mall_Customers.csv` — Dataset
- `README.md` — This file

