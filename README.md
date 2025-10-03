# Customer Segmentation using K-Means Clustering
  - This repository contains a machine learning project that performs **customer segmentation** for a retail store using the **K-means clustering algorithm**. The model groups customers based on their **annual income** and **spending score**, identifying distinct personas for targeted marketing.

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Methodology](#methodology)
- [Results and Interpretation](#results-and-interpretation)
- [How to Run](#how-to-run)
- [Libraries Used](#libraries-used)

---

## 📌 Project Overview
  - The goal of this project is to apply **unsupervised machine learning** to segment customers into different groups based on their purchasing behavior.  
  - By understanding these segments, a retail business can develop more effective and **personalized marketing strategies**.  
  - The notebook walks through the entire process, from **data exploration** to **cluster interpretation**.

---

## 📊 Dataset
The dataset used is the **Mall Customer Segmentation Data**, sourced from [Kaggle](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python).  

It contains basic demographic and behavioral information about mall customers.  

**Features used for clustering:**
- **Annual Income (k$)**
- **Spending Score (1–100):** A score assigned to customers based on their spending behavior.

---

## ⚙️ Methodology
The project is structured into the following key steps:

1. **Data Loading and Exploration**  
   - Load the dataset, inspect data quality, and visualize distributions.

2. **Optimal Cluster Determination**  
   - Use the **Elbow Method** to determine the best number of clusters (K).  
   - The Within-Cluster Sum of Squares (WCSS) is calculated for different values of K.

3. **Model Training**  
   - Train a **KMeans model (scikit-learn)** with the optimal number of clusters (K=5).

4. **Cluster Visualization**  
   - Visualize customer segments using scatter plots, with each cluster **color-coded**.

---

## 📈 Results and Interpretation
The K-means algorithm successfully identified **5 distinct customer segments**:

| Cluster | Persona   | Characteristics                | Marketing Strategy |
|---------|-----------|--------------------------------|--------------------|
| 1       | Careful   | High Income, Low Spending      | Focus on quality, durability, and investment value |
| 2       | Standard  | Average Income, Average Spending | Target with standard promotions and loyalty programs |
| 3       | Target (VIPs) | High Income, High Spending  | Offer exclusive deals and early access to new items |
| 4       | Careless  | Low Income, High Spending      | Promote sales, credit options, and frequent-buyer rewards |
| 5       | Sensible  | Low Income, Low Spending       | Attract with discounts and value-for-money offers |

---

## 🚀 How to Run

**Clone this repository:**
   ```bash
   git clone https://github.com/KrishShah1912/PRODIGY-ML-TASK-2.git

   cd PRODIGY-ML-TASK-2

   pip install numpy pandas matplotlib seaborn scikit-learn

  jupyter notebook ML2.ipynb
   ```

---

## 📚 Libraries Used
  * numpy
  * pandas
  * matplotlib
  * seaborn
  * scikit-learn   
