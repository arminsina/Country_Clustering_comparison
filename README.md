# Country Clustering with Unsupervised Learning

This project applies unsupervised machine learning techniques to cluster countries based on a variety of socio-economic indicators. The goal is to uncover natural groupings among countries without using any predefined labels.

## 📊 Project Overview

Using a publicly available dataset from Kaggle, we explore and cluster countries based on features such as income, child mortality, health expenditure, and more. The clustering results can offer insights into patterns among nations and guide policy or economic strategies.

## 🔍 Steps and Methodology

1. **Data Collection**

   * The dataset is downloaded from Kaggle and contains country-level metrics relevant for socio-economic analysis.

2. **Exploratory Data Analysis (EDA)**

   * We begin by examining distributions, identifying missing values, and understanding relationships through visualizations.
   * Tools used include Pandas, Seaborn, Matplotlib, and Plotly Express.

3. **Preprocessing**

   * Missing values are handled appropriately.
   * Features are scaled to ensure fair treatment in clustering algorithms.

4. **Modeling**

   * Several clustering algorithms are applied and compared:

     * K-Means Clustering
     * Agglomerative Clustering
     * DBSCAN
   * We use dimensionality reduction (e.g., PCA) for visualization when needed.

5. **Model Evaluation**

   * Clustering results are evaluated using the **Silhouette Score** to measure how well-defined the clusters are.
   * Visual plots help validate and interpret cluster groupings.

6. **Insights**

   * Final clusters reveal groups of countries with similar economic and health profiles.
   * These insights can help international organizations or policy analysts identify patterns in development.
