# CryptoClustering Project

## Table of Contents

### 🚀 Live Deployment

### 📌 Overview

### 🎯 Objectives

### 📝 Long-Form Answers with Visuals

### ✅ Explicit Answers to Challenge Questions

### 📂 Project Deliverables

### 🛠️ Technologies Used

### 📖 Steps to Reproduce

### 📁 Repository Structure

### 📜 Reference Section

### 🏆 Badges

### 🏆 Acknowledgments](#🏆-acknowledgments)

---

## 🚀 Live Deployment
🔗 **[GitHub Repository Link](https://github.com/Oceanpro00/CryptoClustering)**

## 📌 Overview

This project was completed as part of my **University of Toronto Data Analytics Bootcamp (Module 19 Challenge)**. The goal of this challenge was to use Python and unsupervised learning techniques to analyze cryptocurrency data and predict whether cryptocurrencies are affected by 24-hour or 7-day price changes. The challenge focused on clustering the data with K-Means both in its scaled form and after dimensionality reduction with Principal Component Analysis (PCA).

---

## 🎯 Objectives

- Load and analyze cryptocurrency market data.
- Normalize data using **StandardScaler()**.
- Find the best value for **k** using the elbow method.
- Cluster cryptocurrencies using **K-Means** on scaled data.
- Apply **PCA** to reduce features to three principal components.
- Cluster the PCA-reduced data and compare results.
- Visualize all findings with scatter plots and elbow curves using **hvPlot**.

---

## 📝 Long-Form Answers with Visuals

### 1️⃣ What is the best value for k (original scaled data)?
**Answer:** Looking at the Elbow Chart for the Crypto Market Data, the optimal value for k is **4**, as beyond this point the improvements in model fit become minimal.

![Regular vs PCA Elbow Comparison](Resources/Regular_vs_PCA_Data_Elbow_Method_Comparison_Chart.png)

### 2️⃣ What is the total explained variance of the three principal components?
**Answer:** The total explained variance of the three principal components is **0.895** (89.5%). This means that these three components capture approximately 90% of the data's variability, which is relatively good given the volatility of cryptocurrency data.

### 3️⃣ What is the best value for k using the PCA data, and does it differ from the original?
**Answer:** The best value for k using PCA data is also **4**. The elbow plots look almost identical with and without PCA, which suggests that PCA preserves enough structure to reliably determine cluster counts.

### 4️⃣ Impact of using fewer features (PCA) in clustering:
**Answer:** The PCA reduces complexity while maintaining structure. Outliers become more visible, and clusters show clear separation. However, it slightly reduces the total variance captured. Using PCA made it easier to identify outliers and visually interpret the clusters. Clusters 1 and 3, for example, appeared more distinct in PCA space.

![Regular vs PCA Clustering Comparison](Resources/Regular_vs_PCA_Scatter_Data_Clustering_Comparison_Chart.png)

---

## ✅ Explicit Answers to Challenge Questions

- **Best k value (original scaled data):** 4  
- **Total explained variance (3 principal components):** 89.5%  
- **Best k value (PCA data):** 4 (same as original)  
- **Impact of PCA:** Outliers become more visible, cluster separation is more apparent, but with slightly less total variance captured in the clustering.

---

## 📂 Project Deliverables

### **1️⃣ Project Setup**
- Created a new GitHub repository: `CryptoClustering`.
- Cloned the repository and added all starter and working files.
- Pushed commits regularly with clear, descriptive messages.

### **2️⃣ Data Preparation & Exploration**
- Loaded `crypto_market_data.csv` into a Pandas DataFrame.
- Generated summary statistics.
- Visualized initial data using line charts to understand market variations.

### **3️⃣ Normalization & Clustering (Original Data)**
- Normalized the data using **StandardScaler()**.
- Applied the **Elbow Method** to find the optimal value of **k** (identified as **k=4**).
- Created clusters using **K-Means**.
- Visualized clusters with scatter plots.

### **4️⃣ Dimensionality Reduction (PCA)**
- Performed PCA to reduce features to 3 components.
- Verified that **89.5%** of the total variance was explained by the 3 principal components.

### **5️⃣ Clustering & Visualization (PCA Data)**
- Re-ran the Elbow Method on PCA data (optimal **k=4**).
- Clustered PCA-transformed data using **K-Means**.
- Created scatter plots for PCA clustering results.

### **6️⃣ Comparison & Visual Previews**
- Created a composite Elbow Method plot using `+` and `*` overlays. I used the `*` operator because it allowed me to see both lines clearly on top of each other.
- Decided not to overlay clustering plots using `*` because it made the results too cluttered and indistinguishable.
- **Screenshots added for visual reference:**
  - ![Regular vs PCA Elbow Comparison](Resources/Regular_vs_PCA_Data_Elbow_Method_Comparison_Chart.png)
  - ![Regular vs PCA Clustering Comparison](Resources/Regular_vs_PCA_Scatter_Data_Clustering_Comparison_Chart.png)

---

## 🛠️ Technologies Used

### **Libraries & Tools**
- **Pandas** – Data analysis and manipulation.
- **Scikit-learn** – StandardScaler, KMeans, PCA.
- **hvPlot** – Interactive visualizations.
- **Jupyter Notebook** – Development and analysis environment.

### **Key Techniques Applied**
- Data scaling and standardization.
- Elbow Method implementation for finding optimal **k**.
- Unsupervised clustering with **K-Means**.
- Dimensionality reduction with **PCA**.
- Visual interpretation and analysis of clustering results.

---

## 📖 Steps to Reproduce

### **1️⃣ Clone Repository**
```bash
git clone git@github.com:Oceanpro00/CryptoClustering.git
cd CryptoClustering
```

### **2️⃣ Run the Analysis Locally**
- Open the `Crypto_Clustering.ipynb` notebook in Jupyter Lab or VSCode.
- Execute cells step by step.
- Visualizations will generate inline.

### **3️⃣ Deployment & Submission**
- Commit changes regularly:
```bash
git add .
git commit -m "Add PCA clustering and visualizations"
git push origin main
```
- Submit both the GitHub repository link and final notebook.

---

## 📁 Repository Structure
```
CryptoClustering/
│-- Resources/
│   ├── crypto_market_data.csv  # Source data file
│   ├── Regular_vs_PCA_Data_Elbow_Method_Comparison_Chart.png  # Visual comparison
│   └── Regular_vs_PCA_Scatter_Data_Clustering_Comparison_Chart.png  # Visual comparison
│-- Crypto_Clustering.ipynb  # Completed Jupyter notebook with analysis
│-- README.md  # Project documentation
```

---

## 📜 Reference Section
- **Dataset:** Provided by edX Boot Camps LLC for educational purposes.
- No external code was used beyond official library documentation examples.

---

## 🏆 Badges

![GitHub Repo Size](https://img.shields.io/github/repo-size/Oceanpro00/CryptoClustering)  
![Last Commit](https://img.shields.io/github/last-commit/Oceanpro00/CryptoClustering)  
![Top Language](https://img.shields.io/github/languages/top/Oceanpro00/CryptoClustering)  

---

## 🏆 Acknowledgments

This project was developed by **Sean Schallberger** as part of the **University of Toronto Data Analytics Bootcamp**.

---
