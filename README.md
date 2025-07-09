# 🧠 K-Means Clustering: Customer Segmentation

This project implements **K-Means Clustering** to segment customers based on their **Annual Income** and **Spending Score**. The goal is to identify distinct customer groups to help businesses tailor their marketing strategies.

---

## 📌 Objective

To apply unsupervised learning (K-Means) to identify hidden patterns in customer behavior without using labeled data.

---

## 🗂 Dataset

- **Source:** `Mall_Customers.csv`
- **Selected Features:**
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

## 🔧 Tools & Libraries Used

- Python
- pandas
- scikit-learn
- matplotlib
- seaborn

---

## 🚀 Project Workflow

1. **Load Dataset**  
   Loaded customer data into a DataFrame.

2. **Preprocessing**
   - Selected relevant features.
   - Scaled features using `StandardScaler`.

3. **Apply K-Means**
   - Used Elbow Method to find optimal `k` (number of clusters).
   - Applied `KMeans` from scikit-learn.

4. **Cluster Assignment**
   - Added a `Cluster` column to the dataset indicating each customer’s segment.

5. **Visualization**
   - Plotted clusters using a 2D scatter plot for clear interpretation.

6. **Interpretation**
   - Used `groupby('Cluster').mean()` to analyze average income and spending behavior per cluster.

---

## 📊 Results Summary

- **Optimal Clusters:** 5
- **Example Cluster Insights:**
  - Cluster 0: High income, low spending
  - Cluster 1: Average income, high spending
  - Cluster 2: Low income, low spending
  - etc.

These insights help businesses identify and target high-value or cost-sensitive customer groups.

---

## 📈 How to Run

```bash
pip install pandas scikit-learn matplotlib seaborn
