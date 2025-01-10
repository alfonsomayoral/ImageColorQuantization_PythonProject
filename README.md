# **🎨 Image Color Quantization and Clustering Using K-means**

![Project Preview](./assets/banner_image.jpg)  
*A visual exploration of K-means clustering and PCA applied to image processing.*

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)  
[![Libraries](https://img.shields.io/badge/Libraries-Scikit--learn%2C%20Matplotlib%2C%20Numpy-green)](https://scikit-learn.org/)  
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen)](#)

---

## **📖 Overview**
This project showcases the application of **K-means clustering** and **Principal Component Analysis (PCA)** for the following tasks:

1. **Synthetic Dataset Clustering**:
   - Using K-means to group data points into clusters.
   - Visualizing the cluster assignments and centroids for different \(K\) values.

2. **Evaluating K-means Performance**:
   - Analyzing the impact of the number of clusters using the Sum of Squared Errors (SSE).
   - Determining the optimal number of clusters using the "elbow method."

3. **Image Color Quantization**:
   - Applying K-means to simplify the color palette of an image.
   - Visualizing the transformation for multiple \(K\) values.

4. **Dimensionality Reduction with PCA**:
   - Reducing the RGB space of an image to 2D.
   - Investigating how PCA affects the clustering and quantization results.

This notebook provides both theoretical insights and practical applications, making it suitable for data science enthusiasts and developers interested in clustering and image processing.

---

## **📋 Table of Contents**
1. [Introduction](#introduction)  
2. [Implementation Details](#implementation-details)  
3. [How to Use](#how-to-use)  
4. [Visual Results](#visual-results)  
5. [Conclusion and Insights](#conclusion-and-insights)  

---

## **🚀 Introduction**
- **K-means clustering**: A fundamental unsupervised learning algorithm that partitions data into \(K\) clusters by minimizing intra-cluster variance.  
- **Principal Component Analysis (PCA)**: A dimensionality reduction technique that transforms high-dimensional data into a lower-dimensional space while preserving the most variance.  
- **Image color quantization**: A practical application that reduces the number of colors in an image while retaining its visual coherence.

---

## **🛠 Implementation Details**

### **1. K-means Clustering**
- Synthetic datasets are generated and clustered using K-means for \(K = 2\) to \(8\).
- Each clustering result visualizes the data points, their cluster assignments, and the centroids.

#### **Screenshot Instructions:**
Insert the following image showing clustering results for \(K = 5, 6, 7\):  
**Path:** `./assets/kmeans_results_k5_k6_k7.png`  
**Caption:** "Clustering results for \(K = 5, 6, 7\), with centroids marked as red crosses."

---

### **2. Evaluating K-means with SSE**
- The Sum of Squared Errors (SSE) measures clustering performance.
- The "elbow method" is used to identify the optimal number of clusters.

#### **Screenshot Instructions:**
Insert the SSE plot image:  
**Path:** `./assets/sse_elbow_plot.png`  
**Caption:** "SSE vs. \(K\), showing the optimal \(K\) where the curve bends."

---

### **3. Image Color Quantization**
- Each pixel's RGB color is treated as a data point.
- K-means groups similar colors into clusters, and the resulting image is quantized using the centroids.

#### **Screenshot Instructions:**
1. Insert an image comparing the original photo and quantized photo for \(K = 4\):  
   **Path:** `./assets/original_vs_quantized_k4.png`  
   **Caption:** "Original vs. quantized image for \(K = 4\)."

2. Insert an image comparing quantized photos for \(K = 2, 4, 8\):  
   **Path:** `./assets/quantized_images_k2_k4_k8.png`  
   **Caption:** "Quantized images for \(K = 2, 4, 8\), showing how increasing \(K\) improves quality."

---

### **4. Principal Component Analysis (PCA)**
- Reduces RGB pixel space to 2D for efficient clustering.
- Clusters are mapped back to RGB space to reconstruct the quantized images.

#### **Screenshot Instructions:**
1. Insert a scatter plot showing PCA-transformed pixel data:  
   **Path:** `./assets/pca_scatter_plot.png`  
   **Caption:** "2D scatter plot of RGB pixel data after PCA transformation."

2. Insert a comparison of the original image and PCA-based quantized images for \(K = 2, 4, 8\):  
   **Path:** `./assets/pca_quantized_images_k2_k4_k8.png`  
   **Caption:** "Original vs. PCA-quantized images for \(K = 2, 4, 8\)."

---

## **📌 How to Use**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/image-quantization.git
