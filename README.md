# AstroClusterModel: Clustering Astronomical Images

**AstroClusterModel** is a machine learning pipeline that clusters astronomical FITS images based on structural and compositional features like planetary blobs, ring structures, and radial intensity profiles. It combines feature engineering, dimensionality reduction (UMAP/PCA), and clustering (K-Means) to uncover meaningful groupings in space imagery.

---

## 📁 Overview

- 🔍 Extracts **52 handcrafted features**: radial, blob, and ring features.
- 🔻 Reduces dimensions using **UMAP**/**PCA**.
- 📌 Clusters using **K-Means**.
- 🧠 Provides **cluster interpretations** and **sample images**.

---

## 📸 Sample Astronomical Images

![Sample Images](https://github.com/user-attachments/assets/4e409d6d-71ad-49a7-b728-962d6b917228)

---

## 📦 Pipeline Summary

### 🔹 1. Feature Extraction

| Feature Group    | Description |
|------------------|-------------|
| **Radial**       | Mean, std, peaks, zero-crossings in radial intensity profiles |
| **Blob**         | Count, average size, and intensity of blobs (planet-like regions) |
| **Ring**         | Count, radius, and concentricity of rings via Hough Circle Transform |

![Feature Types](https://github.com/user-attachments/assets/9382875b-d1f8-4743-9fd0-62b6b8a2a409)

---

### 🔹 2. Dimensionality Reduction

| Technique | Purpose |
|-----------|---------|
| **UMAP**  | Non-linear reduction for better visual cluster separation |
| **PCA**   | Linear reduction for easier interpretation |

---

### 🔹 3. Clustering

- Uses **K-Means** on reduced features.
- Automatically **interprets clusters** using statistical summaries.
- Displays **sample images** from each cluster.

---

## 📊 Results

### 📌 Cluster Distribution
![cluster_distribution](https://github.com/user-attachments/assets/b976d456-6936-45fc-abb9-5c53074bec9d)


### 🌌 2D Visualization (UMAP)
![2D Cluster Viz](https://github.com/user-attachments/assets/52b5a2db-93ee-4b6a-b003-952a56c3afca)

---

## 🧪 Cluster Summaries

### 🌀 Cluster 0
![Cluster 0 Samples](https://github.com/user-attachments/assets/5014f7de-d6d5-4181-93f4-8dc14d1e0e07)

---

### 🪐 Cluster 1
![Cluster 1 Samples](https://github.com/user-attachments/assets/ce72c658-6a96-422f-aee7-da710169ed8b)


---

### 🌗 Cluster 2
![Cluster 2 Samples](https://github.com/user-attachments/assets/68204b31-8836-45ce-96dd-531e889b3b49)


---

## 🔑 Project Use Cases

- Automatically categorize thousands of astronomical images without manual inspection
- Identify exoplanetary systems with similar structural patterns for comparative research
- Flag statistical outliers that may represent new astronomical phenomena or instrument errors
- Provide quantitative metrics for comparing morphological features across star systems
