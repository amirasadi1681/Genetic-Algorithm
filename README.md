# Genetic Algorithm for Clustering

This repository contains the implementation of a **Genetic Algorithm (GA)** for clustering tasks.  
The goal of the project is to optimize the centroid positions of a clustering problem using the principles of **natural selection** and **evolutionary algorithms**.

The project was part of the **Artificial Intelligence** course at **Amirkabir University of Technology (Tehran Polytechnic)**.  
It demonstrates how **Genetic Algorithms** can be applied to improve clustering results by iteratively optimizing centroid locations for better cluster separation.

---

## 📘 Project Overview

The Genetic Algorithm was used to solve a clustering problem by:
- Optimizing the centroids of clusters using evolutionary principles like **selection**, **crossover**, and **mutation**.
- Iterating through multiple generations of candidate solutions to minimize intra-cluster distances and improve cluster separation.

The dataset used in this project consists of **dry bean features**, and the goal is to group similar samples into distinct clusters based on feature similarity.

---

## ⚙️ Methodology

### 1. **Data Preprocessing**
- Cleaned and normalized the dataset.  
- Removed irrelevant attributes and handled missing data.  
- Applied **IQR (Interquartile Range)** filtering to remove outliers.

### 2. **Genetic Algorithm Design**
The GA evolves potential solutions using:
- **Selection:** Chooses the best individuals (centroid sets) based on fitness.  
- **Crossover:** Combines two parent solutions to produce offspring.  
- **Mutation:** Introduces random variation to maintain diversity in the population.

### 3. **Fitness Function**
The fitness function evaluates how well the clusters are formed:
- Minimizes **intra-cluster distance** (compact clusters).  
- Maximizes **inter-cluster separation** (well-separated clusters).

---

## 📊 Results and Analysis

The **Genetic Algorithm** successfully improved cluster quality by refining centroid positions over generations.  
Compared to traditional methods like **K-Means**, GA-based clustering achieved:
- Better separation between clusters.  
- Lower average distance between points and their assigned centroids.  
- Improved convergence stability and reduced dependency on initialization.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/genetic-algorithm-clustering.git
   cd genetic-algorithm-clustering
