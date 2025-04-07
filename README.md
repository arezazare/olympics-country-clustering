# 🏅 Olympic Country Clustering Project

## 📌 Overview
This project applies **unsupervised machine learning (clustering)** to analyze and group countries based on their **Olympic medal performance**. Using **KMeans**, **DBSCAN**, and **Agglomerative Clustering**, we reveal patterns in Olympic success — separating elite countries from medium performers and occasional participants.

---

## 💡 Objectives
- Clean and prepare Olympic data from multiple Excel sheets  
- Perform EDA to uncover trends and outliers  
- Engineer features (e.g., medal ratios) and normalize data  
- Apply and compare three clustering algorithms  
- Visualize clusters in 2D and 3D space using PCA and Plotly  
- Analyze the role of each feature in cluster formation  

---

## 🔧 Tools & Libraries
- **Python**
- `pandas`, `numpy`, `seaborn`, `matplotlib`, `plotly`
- `scikit-learn` (for clustering, scaling, PCA)
- `scipy` (for dendrograms)
- `joblib` (for saving models and scalers)

---

## 🧼 Steps in the Pipeline

### 1. Data Exploration & Cleaning
- Combined all sheets from an Excel file into a single DataFrame  
- Removed irrelevant columns (e.g., Edition)  
- Handled missing values & duplicates  
- Cleaned up inconsistent country names  

### 2. Exploratory Data Analysis (EDA)
- Histograms, violin plots, and KDEs to show distribution  
- Correlation heatmaps and pairplots  
- Outlier detection using the IQR method  

### 3. Feature Engineering & Preprocessing
- Created medal ratios: `Gold_Ratio`, `Silver_Ratio`, `Bronze_Ratio`  
- Normalized data using `StandardScaler`  
- Prepared dataset for clustering  

### 4. Clustering Models

| Model          | Strengths                                   |
|----------------|----------------------------------------------|
| **KMeans**     | Simple, interpretable, good for spherical clusters |
| **DBSCAN**     | Detects arbitrary shapes & outliers         |
| **Agglomerative** | Builds a hierarchy, visualized via dendrogram |

### 5. Evaluation
- **Elbow Method** and **Silhouette Score** for KMeans  
- **Dendrogram** for Agglomerative Clustering  
- **Noise detection** in DBSCAN  
- **3D PCA Plot** for interactive cluster visualization  

---

## 📊 Results & Interpretation

### Cluster Descriptions
- **Cluster 0** → Low/average medal performers  
- **Cluster 1** → A few strong nations (e.g., Russia)  
- **Cluster 2** → Top elite (USA dominates)  

### Clustering Method Comparison

| Clustering Method     | Insights                                      |
|------------------------|-----------------------------------------------|
| **KMeans**             | Clear performance tiers                      |
| **DBSCAN**             | Identified noise and denser groups           |
| **Agglomerative**      | Confirmed structure with hierarchical relationships |

---

## 📌 Conclusion
This project highlights how **clustering can uncover hidden structures** in real-world datasets — in this case, showing how countries perform and group in Olympic history.

---

## 🚀 Future Improvements
- Add recent Olympic data (e.g., **Tokyo 2020**)  
- Cluster by **sport categories** (e.g., Athletics vs. Swimming)  
- Merge with **GDP, population, or region** for deeper insights  
"""

---

👏 Author
Reza — Full ML pipeline implemented from scratch.

---

📎 Credits
Dataset sourced from Kaggle for educational and research purposes. All rights to the original dataset belong to the respective uploader.
