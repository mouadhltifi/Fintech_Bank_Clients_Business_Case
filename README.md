# Fintech Bank Clients Business Case

This repository contains the code and analysis for a banking client segmentation project based on a business case study in the fintech domain. We use advanced clustering techniques—including K-Medoids with custom distance metrics—to segment bank clients, extract actionable insights, and develop tailored financial personas.

---

## Overview

The project aims to enable banks to better understand and serve their clients by:
- **Preprocessing Data:**  
  Cleaning and transforming raw bank client data using techniques such as winsorization, correlation-based feature reduction, scaling, and dimensionality reduction (PCA).
  
- **Custom Distance Metrics:**  
  Developing and applying several custom distance metrics (e.g., Tanimoto + Cityblock new, Hamming + Cityblock new, Euclidean + Jaccard, Mahalanobis + Hamming) to effectively capture similarities among clients with mixed data types.

- **Clustering:**  
  Using K-Medoids clustering (from scikit-learn-extra) with precomputed distance matrices to segment clients into distinct groups. The optimal number of clusters (k=3) was determined based on multiple evaluation metrics.

- **Evaluation & Visualization:**  
  Assessing clustering quality with metrics like Calinski-Harabasz, Davies-Bouldin, Silhouette, Dunn Index, and WCSS. Visualizations (including high-resolution t-SNE plots) help interpret the cluster structure.

- **Persona Development:**  
  Translating the clustering outcomes into three well-defined client personas (Urban High-Earners, Retired Traditionalists, and Midlife Moderates) along with detailed value propositions and service models.

---

## Repository Structure

- **`data/`**  
  Contains the input datasets and metadata files (e.g., `Dataset1_BankClients.xlsx`).

- **`notebooks/`**  
  Jupyter notebooks for data preprocessing, clustering analysis, visualization, and persona development.

- **`src/`**  
  Python scripts that implement custom distance functions, clustering evaluation routines, and visualization tools.

- **`README.md`**  
  This file.

---

## Installation

This project requires Python 3.7 or higher. To install the necessary dependencies, run:

```bash
pip install -r requirements.txt
