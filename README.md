## 🌍 Country Clustering with Unsupervised Learning

This project applies unsupervised machine learning techniques to identify natural groupings of countries based on socio-economic indicators. By leveraging clustering algorithms, we aim to uncover hidden patterns that reflect similarities in development, health, and economic profiles among nations.

---

### 📝 Project Overview

We utilize multiple clustering algorithms to group countries based on socio-economic metrics such as income, child mortality, health expenditure, and more. This allows us to gain insights into global development disparities and potentially guide policy planning and decision-making.

Unsupervised learning is particularly useful here, as we do not provide the model with predefined country categories. Instead, clusters are formed based on inherent data similarities.

---

### 📂 Dataset

* **Source:** [Kaggle - Unsupervised Learning on Country Data](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data)
* **Format:** CSV, includes features such as:

  * `child_mort`: Death of children under 5 per 1000 births
  * `exports`, `imports`: % of GDP
  * `health`: % of GDP spent on health
  * `income`: Net income per person
  * `inflation`: % annual inflation
  * `life_expec`: Life expectancy
  * `gdpp`: GDP per capita
  * And more...

---

### 🔄 Data Processing Workflow

#### 1️⃣ Data Loading & Cleaning

* Dataset is loaded using Pandas.
* Missing values are handled.
* Outliers are checked and treated where needed.

#### 2️⃣ Exploratory Data Analysis (EDA)

* Visualizations created using Seaborn, Matplotlib, and Plotly.
* Correlation heatmaps and pairplots to understand relationships.
* Feature distributions reviewed to guide scaling and modeling.

#### 3️⃣ Preprocessing

* Features scaled using `StandardScaler` to ensure fair distance measures.
* Dimensionality reduction via **PCA** for 2D visualization of clusters.

#### 4️⃣ Clustering Models

We experimented with the following unsupervised clustering techniques:

* **K-Means Clustering**
* **Agglomerative Hierarchical Clustering**
* **DBSCAN (Density-Based Clustering)**

Each model was tested and visualized to compare performance.

#### 5️⃣ Evaluation

* **Silhouette Score** used as the main metric to assess clustering quality.
* Cluster visualizations via scatter plots and PCA projections.
* Cluster characteristics analyzed by comparing feature means per group.

---

### 📊 Results & Insights

Among all clustering methods tested, only Hierarchical Clustering with average linkage produced well-defined results, achieving a Silhouette Score of 0.72. This indicates strong cluster separation and a good fit for the data.

Other algorithms like K-Means, Fuzzy C-Means, and Mean Shift scored between 0.55 and 0.60, showing weaker clustering performance.
DBSCAN failed to form valid clusters (score = 0), likely due to the dataset’s structure and lack of dense regions.

Overall, hierarchical clustering provided the most meaningful grouping of countries based on socio-economic and health-related indicators.
---


### 📌 Conclusion

This project demonstrates the power of unsupervised learning to reveal global socio-economic patterns. It shows how clustering, combined with solid preprocessing and visualization, can uncover meaningful insights — without requiring labeled data.
