# Genetic Algorithm for Clustering

This repository contains the implementation of a **Genetic Algorithm (GA)** for clustering tasks. The goal of the project is to optimize the centroid positions of a clustering problem using the principles of **natural selection** and **evolutionary algorithms**.

The project was part of the **Artificial Intelligence** course at **Amirkabir University of Technology**. It demonstrates how **Genetic Algorithms** can be applied to improve clustering results by iteratively optimizing the location of centroids for better cluster separation.

---

## 📘 Project Overview

The Genetic Algorithm was used to solve a clustering problem by:
- Optimizing the centroids of clusters using evolutionary principles like **selection**, **crossover**, and **mutation**.
- Iterating through generations of potential solutions to refine the positions of the centroids and minimize intra-cluster distances.

The dataset used for clustering contains features of **dry beans**, and the task was to identify patterns and form well-separated clusters.

---

## ⚙️ Methodology

### 1. **Data Preprocessing:**
- Cleaned the dataset and removed irrelevant attributes.
- Normalized the data for stable convergence in the algorithm.
- Applied **IQR (Interquartile Range)** for outlier detection and removal.

### 2. **Genetic Algorithm Process:**
The algorithm used the following evolutionary steps:
- **Selection:** Based on the fitness function, the best solutions were selected to reproduce.
- **Crossover:** Parents exchanged information to produce offspring for the next generation.
- **Mutation:** A small random change was introduced to some solutions to explore new potential solutions.

### 3. **Fitness Function:**
The fitness function was designed to:
- Minimize the **sum of squared distances** within each cluster.
- Maximize the **distance between clusters**, ensuring they were well-separated in the feature space.

---

## 📊 Results and Analysis

### 🔹 Clustering Performance:
The **Genetic Algorithm** optimized the cluster centroids and improved the clustering results, outperforming traditional methods like **K-Means** by:
- Better separation between clusters.
- Improved intra-cluster distance reduction.

#### **Visualization of Clustering Results:**
The final clusters formed by the Genetic Algorithm are shown below:

![Clustering Results](docs/figures/clustering_results.png)

#### **Fitness Progress Over Generations:**
The fitness function improved across generations, demonstrating the algorithm's convergence towards optimal centroids.

![Fitness Progress](docs/figures/fitness_progress.png)

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/genetic-algorithm-clustering.git
   cd genetic-algorithm-clustering
