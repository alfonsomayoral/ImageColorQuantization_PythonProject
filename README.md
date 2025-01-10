# **Image Color Quantization Using K-means Clustering**

![Preview](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section3.1.png)

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/)  
[![Libraries](https://img.shields.io/badge/Libraries-Scikit--learn%2C%20Matplotlib%2C%20Seaborn%2C%20Numpy-green)](https://scikit-learn.org/)  
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen)](#)

---

## **📖 Overview**
This project explores the application of the K-means clustering algorithm and Principal Component Analysis (PCA) for data clustering and dimensionality reduction. A specific focus is placed on **image color quantization**, where K-means is utilized to simplify the number of colors in an image, improving compression and providing artistic rendering effects.

The implementation is structured in a clear and modular Jupyter Notebook, enabling seamless experimentation and visualization. This project showcases the application of **K-means clustering** and **Principal Component Analysis (PCA)** for the following tasks:

1. **Synthetic Dataset Clustering**: Using K-means to group data points into clusters and visualizing the cluster assignments and centroids for different \(K\) values.

2. **Evaluating K-means Performance**: Analyzing the impact of the number of clusters using the Sum of Squared Errors (SSE) and determining the optimal number of clusters using the "elbow method."

3. **Image Color Quantization**: Applying K-means to simplify the color palette of an image and visualizing the transformation for multiple \(K\) values.

4. **Dimensionality Reduction with PCA**: Reducing the RGB space of an image to 2D and investigating how PCA affects the clustering and quantization results.

---

## **📋 Table of Contents**
- 🚀 [Introduction](#-introduction)
- 🛠  [Implementation Details & Structure](#-implementation-details--structure)
- 📌 [How to Use](#-how-to-use)
- 📊 [Visual Results](#-visual-results)

---

### 🚀 **Introduction**
The project leverages **unsupervised machine learning techniques**:
1. **K-means clustering**: Partitioning data into clusters by minimizing intra-cluster variance.
2. **Principal Component Analysis (PCA)**: Reducing data dimensionality while retaining key variance.

This notebook demonstrates their integration for tasks like:
- Clustering synthetic datasets.
- Image compression and artistic transformation via color quantization.
- Dimensionality reduction for enhancing clustering performance.

---

### 🛠 **Implementation Details & Structure**
#### 1. **Introduction and Setup**
   - Key libraries: `NumPy`, `Scikit-learn`, `Matplotlib`, and `Seaborn`.
   - Overview of clustering (K-means) and dimensionality reduction (PCA) concepts.

#### 2. **K-means Clustering Implementation**
   - **Synthetic Data Generation**: Using `make_blobs` for creating visual datasets.
   - **Clustering Visualization**: Iterative application of K-means with varying cluster sizes (K=2 to K=8), highlighting intra-cluster dynamics.

#### 3. **Evaluating Clusters with SSE**
   - Analysis of the Sum of Squared Errors (SSE) to determine the optimal number of clusters using the **elbow method**.

#### 4. **Image Color Quantization**
   - Image preprocessing:
     - Resizing large images to manageable sizes.
     - Converting RGB pixel data to floating-point arrays.
   - Application of K-means for various cluster sizes (K = 2, 4, 8, ...).
   - Replacement of image colors with cluster centroids, creating "quantized" outputs.

#### 5. **Dimensionality Reduction via PCA**
   - Reduction of RGB dimensions to a 2D space.
   - Comparison of clustering and quantization results with and without PCA.

---

### 📌 **How to Use**

_Follow these step-by-step instructions to set up and run the project on your local machine._

1. Clone the repository and install the required libraries.
   ```bash
   git clone <repository_url>
   cd project_directory
   pip install -r requirements.txt

2. Install Required Dependencies
- Make sure you have Python 3.7 or later installed. Install the necessary libraries by running:
   ```bash
   pip install -r requirements.txt
- This will install dependencies such as: NumPy for numerical computations, Scikit-learn for implementing K-means and PCA, Matplotlib and Seaborn for data visualization, scikit-image for image processing.

3. Launch the Jupyter Notebook
- Run the following command to open the Jupyter Notebook interface:
   ```bash
   jupyter notebook Image_Color_Quatization_Using_Kmeans_Clustering.ipynb
- This will open the notebook in your default web browser.

4. Navigate Through the Notebook
- The notebook is structured into sections. Start by running the initial cells to set up the environment and import the required libraries.
- Each section includes explanations and visualizations. Run each cell sequentially to reproduce the results.

5. Test with Your Own Image
- To test the color quantization on your own image:
   1. Save your image file as photo.JPG.
   2. Place the image in the same directory as the notebook.
 
6. Experiment with Parameters
- Feel free to tweak parameters like:
   - Number of clusters (K): Modify the K values in the K-means clustering sections to see how the results change.
   - Image dimensions: Resize the image for faster processing or better results.
 
7.  Save the Outputs
- You can save the quantized images or plots generated during the execution by using the following commands:
   ```bash
   plt.savefig('output_image_name.png', dpi=300)

8. Troubleshooting
- If any library is missing, install it manually using:
   ```bash
   pip install <library_name>.
- Ensure that photo.JPG is correctly named and in the notebook’s directory.

**With these steps, you can fully explore and experiment with the project. Happy coding! 🚀**

---

### 📊 **Visual Results**

Below are visual results from each section of the notebook, showcasing the outputs generated during the implementation. This section highlights the progression and results from each stage of the project, providing a clear and visual understanding of the outcomes. 🎨

---

#### **1. Synthetic Dataset and K-means Clustering**
The synthetic dataset was clustered using K-means for various values of \( K \). Each cluster is represented with a different color, and centroids are marked with red crosses.

![K-means Clustering](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section1.png)

---

#### **2. Image Color Quantization (Original vs Quantized Images)**
The original image was quantized using K-means clustering for different values of \( K \). Below are comparisons for \( K = 4 \) and \( K = 16 \).

![Quantized Image K=4](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section3.1.png)

![Quantized Image K=16](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section3.2.png)

---

#### **3. Dimensionality Reduction with PCA**
The RGB pixel data of the image was reduced to 2D using PCA, visualized as a scatter plot. This reduced representation was then clustered using K-means, and the results were mapped back to the original RGB space.

![PCA Scatter Plot](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section4.1.png)

![PCA Quantized Image K](https://github.com/alfonsomayoral/ImageColorQuantization_PythonProject/blob/main/assets/Section4.2.png)

---

