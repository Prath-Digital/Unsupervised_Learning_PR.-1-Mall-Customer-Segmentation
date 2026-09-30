# 🛍️ Mall Customer Segmentation 🚀

### _Unsupervised Learning — Practical Report 1_

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Viz-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 🌟 Project Overview

Welcome to the **Mall Customer Segmentation** project! 🎯 This repository explores the powerful world of **Unsupervised Learning** to uncover hidden patterns within customer data. By leveraging advanced clustering algorithms, we aim to group customers into distinct segments based on their spending behavior and annual income.

### 🎯 Core Objectives

- 🔍 **Explore:** Deep dive into the Mall Customer dataset using EDA.
- ⚙️ **Preprocess:** Clean, encode, and scale data for optimal model performance.
- 🤖 **Cluster:** Implement and fine-tune **K-Means**, **Hierarchical**, and **DBSCAN** algorithms.
- ⚖️ **Compare:** Evaluate and compare the performance of different clustering approaches.
- 💡 **Insight:** Transform data patterns into actionable **Business Intelligence**.

### 🎓 Academic Context

| 🏫 Institute                    | 📚 Subject            | 📝 Project                | 📊 Domain        |
| :------------------------------ | :-------------------- | :------------------------ | :--------------- |
| **Red & White Skill Education** | Unsupervised Learning | Practical Report 1 (PR 1) | Retail Analytics |

---

## 📊 The Data Journey

### 📂 Dataset Details

The project utilizes the **Mall Customer Segmentation Dataset** from Kaggle.

- **Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) 🌐
- **Size:** 200 Rows | 5 Columns 📏
- **Quality:** 💎 0 Missing Values | 0 Duplicates

| 📋 Column        | 📝 Description                                   |
| :--------------- | :----------------------------------------------- |
| `CustomerID`     | Unique identifier (removed during preprocessing) |
| `Gender`         | Customer gender (encoded)                        |
| `Age`            | Customer age                                     |
| `Annual_Income`  | Annual income in thousands (k$)                  |
| `Spending_Score` | Mall-assigned spending score (1-100)             |

### 🛠️ Data Preprocessing Pipeline

1.  **🧹 Cleaning:** Removed `CustomerID` as it holds no predictive value.
2.  **🏷️ Renaming:** Standardized columns to `Annual_Income` and `Spending_Score`.
3.  **🔢 Encoding:** Transformed `Gender` into binary numerical format (0/1).
4.  **⚖️ Scaling:** Applied `StandardScaler` to normalize `Age`, `Annual_Income`, and `Spending_Score`.
5.  **🎯 Selection:** Focused on `Annual_Income` vs `Spending_Score` for clear 2D visualization.

---

## 🤖 Machine Learning Suite

We implemented three distinct clustering paradigms to capture different data structures:

### 1️⃣ K-Means Clustering (Centroid-Based) 🎯

- **Method:** Optimized using the **Elbow Method** and **Silhouette Score**.
- **Result:** Identified **5 optimal clusters**.
- **Strengths:** Fast, efficient, and highly interpretable segments.

### 2️⃣ Agglomerative Hierarchical Clustering (Connectivity-Based) 🌳

- **Method:** Used **Ward Linkage** to minimize within-cluster variance.
- **Result:** Confirmed the 5-cluster structure via **Dendrogram** analysis.
- **Strengths:** Reveals the hierarchical relationship between customer groups.

### 3️⃣ DBSCAN (Density-Based) 🌌

- **Method:** Tuned `eps` (0.4) and `min_samples` (3) using **k-NN distance plots**.
- **Result:** Found **4 dense clusters** and identified **10 noise points**.
- **Strengths:** Robust to outliers and identifies non-spherical shapes.

---

## 📈 Evaluation & Comparison

| 🚀 Algorithm     | 🔢 Clusters | 💎 Silhouette Score | 📉 Davies-Bouldin | ⚡ Calinski-Harabasz |
| :--------------- | :---------: | :-----------------: | :---------------: | :------------------: |
| **K-Means**      |      5      |      **0.555**      |       0.572       |       248.649        |
| **Hierarchical** |      5      |        0.554        |       0.578       |       244.410        |
| **DBSCAN**       |      4      |        0.395        |       0.601       |        97.172        |

> [!TIP]
> **K-Means** emerged as the winner for this dataset due to its superior silhouette score and highly interpretable cluster boundaries! 🏆

---

## 💡 Business Intelligence

### 👥 Customer Segments & Marketing Strategies

| 👑 Segment                         | 👤 Profile                | 🚀 Marketing Action                           |
| :--------------------------------- | :------------------------ | :-------------------------------------------- |
| **High Income, High Spenders**     | The "VIPs" 💎             | Exclusive loyalty programs & luxury rewards.  |
| **Low Income, High Spenders**      | The "Trendsetters" 🌟     | Social media flash sales & trending products. |
| **Middle Income, Middle Spenders** | The "Steady Core" 🛡️      | Seasonal promos & consistent value offers.    |
| **High Income, Low Spenders**      | The "Growth Potential" 📈 | Personalized high-value concierge services.   |
| **Low Income, Low Spenders**       | The "Budget Conscious" 💰 | Discount-led campaigns & essential bundles.   |

---

## 🛠️ Technical Deep Dive

### 💻 Tech Stack

- **Language:** 🐍 `Python`
- **Data:** 🐼 `Pandas`, 🔢 `NumPy`
- **ML:** 🤖 `Scikit-Learn`, 🧪 `SciPy`
- **Viz:** 🎨 `Matplotlib`, 🌊 `Seaborn`
- **Env:** 📓 `Jupyter Notebook`

### 🚀 Getting Started

1.  **Clone it:**
    ```bash
    git clone https://github.com/Prath-Digital/Unsupervised_Learning_PR.-1-Mall-Customer-Segmentation.git
    cd Unsupervised_Learning_PR.-1-Mall-Customer-Segmentation
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Analysis:**
    Launch the notebook and run all cells! 🚀
    ```bash
    jupyter notebook Mail_Customer_Segmentation.ipynb
    ```

---

## 🎬 Media & History

### 📸 Visualizations

The project includes comprehensive plots:
✅ Elbow & Silhouette plots | ✅ Dendrograms | ✅ Cluster Scatterplots | ✅ 3-Algorithm Comparison

### 📹 Project Video

[🎥 Click here to watch the walkthrough!](./video.mp4)

### 📜 Git History

- ✨ `Add EDA section with pairplot and correlation heatmap`
- ✨ `Build K-Means clustering with Elbow and Silhouette analysis`
- ✨ `Add Hierarchical Clustering and dendrogram analysis`
- ✨ `Add DBSCAN tuning and clustering comparison`
- ✨ `Add project documentation and requirements`

---

## ✅ Project Status

| 🧩 Component                               | 🚦 Status    |
| :----------------------------------------- | :----------- |
| Dataset Loading & Inspection               | ✅ Completed |
| Data Preprocessing                         | ✅ Completed |
| Exploratory Data Analysis                  | ✅ Completed |
| Clustering (K-Means, Hierarchical, DBSCAN) | ✅ Completed |
| Model Evaluation & Comparison              | ✅ Completed |
| Customer Segmentation & Insights           | ✅ Completed |
| Documentation                              | ✅ Completed |

---

## 👤 Author & License

**Prath Udhnawala**
🔗 [GitHub Profile](https://github.com/Prath-Digital)

---

_Built with ❤️ for Unsupervised Learning Education._

**License:** This project is created for academic and educational purposes. The Mall Customer Segmentation dataset is sourced from Kaggle and is used according to its applicable dataset license.
