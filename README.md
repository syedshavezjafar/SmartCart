# SmartCart Customer Segmentation using Unsupervised Learning

## Project Overview

Modern e-commerce platforms collect large volumes of customer data, but extracting meaningful insights from this data is a major challenge.

This project builds an **Intelligent Customer Segmentation System** using **Unsupervised Machine Learning** techniques to identify hidden patterns in customer behaviour.

By clustering customers based on **purchase history, demographics, engagement, and spending behaviour**, businesses can design personalized marketing strategies, improve customer retention, and identify high-value customers.

The dataset contains **2240 customer records with 22 attributes**, including demographic information, purchasing behaviour, and customer engagement.

---

## Problem Statement

SmartCart is an e-commerce platform operating across multiple countries.

Currently, the company applies **generic marketing strategies to all customers**, which results in:

- Inefficient marketing campaigns
- Poor targeting of high-value customers
- Missed opportunities to retain loyal customers
- Difficulty identifying churn-prone users

To solve this problem, the goal of this project is to build an **intelligent customer segmentation system** using **unsupervised machine learning clustering algorithms**.

These clusters help businesses implement **data-driven marketing strategies**.

---

## Dataset Description

Each row in the dataset represents a **single customer**.

### Customer Demographics

| Feature | Description |
|------|------|
| ID | Unique customer identifier |
| Year_Birth | Year of birth of the customer |
| Education | Highest education level achieved |
| Marital_Status | Marital status of the customer |
| Income | Yearly household income |
| Kidhome | Number of small children in household |
| Teenhome | Number of teenagers in household |
| Dt_Customer | Date when customer enrolled |

---

### Purchase Behaviour (Amount Spent)

| Feature | Description |
|------|------|
| MntWines | Amount spent on wine products |
| MntFruits | Amount spent on fruits |
| MntMeatProducts | Amount spent on meat products |
| MntFishProducts | Amount spent on fish products |
| MntSweetProducts | Amount spent on sweet products |
| MntGoldProds | Amount spent on gold products |

---

### Purchase Behaviour (Frequency)

| Feature | Description |
|------|------|
| NumDealsPurchases | Purchases made using discounts |
| NumWebPurchases | Purchases made through website |
| NumCatalogPurchases | Purchases made through catalog |
| NumStorePurchases | Purchases made in physical stores |
| NumWebVisitsMonth | Number of visits to website per month |

---

### Customer Feedback

| Feature | Description |
|------|------|
| Recency | Number of days since last purchase |
| Complain | Customer complained in last 2 years (1 = Yes, 0 = No) |

---

## Machine Learning Approach

Since there are **no predefined labels**, the problem is solved using **unsupervised learning techniques**.

### Project Workflow

1. Data Cleaning
2. Feature Engineering
3. Data Preprocessing
4. Feature Scaling
5. Dimensionality Reduction (PCA)
6. Clustering
7. Cluster Evaluation
8. Visualization of results

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Data Preprocessing

The following preprocessing steps were applied:

- Handling missing values
- Encoding categorical variables
- Removing unnecessary columns
- Feature scaling using **StandardScaler**

Scaling is important because clustering algorithms rely on **distance-based calculations**, and features with larger values could dominate the clustering results.

---

## Dimensionality Reduction

To visualize high-dimensional data, **Principal Component Analysis (PCA)** was used.

Benefits of PCA:

- Reduces dimensionality
- Helps visualize clusters
- Improves clustering performance

---

## Clustering Algorithms Used

### K-Means Clustering

K-Means groups customers into clusters based on similarity.

Steps:

1. Choose number of clusters (k)
2. Assign each data point to nearest centroid
3. Update centroid positions
4. Repeat until convergence

Evaluation techniques used:

- Elbow Method
- Silhouette Score

---

### Agglomerative Hierarchical Clustering

Agglomerative clustering follows a **bottom-up approach**:

1. Each data point starts as its own cluster
2. Closest clusters are merged
3. Process continues until the required clusters are formed

This method helps understand **hierarchical relationships between customer groups**.

---

## Results and Insights

The clustering model identifies different customer groups such as:

- High-value loyal customers
- Discount-driven buyers
- Low engagement customers
- Frequent website visitors
- Potential churn customers

These insights help businesses:

- Personalize marketing campaigns
- Improve customer retention
- Increase marketing efficiency
- Target high-value customers effectively

---

## Project Structure
SmartCart-Customer-Segmentation
│
├── data/
│ └── marketing_campaign.csv
│
├── notebooks/
│ └── customer_segmentation.ipynb
│
├── images/
│ └── cluster_visualization.png
│
├── README.md
└── requirements.txt

---

## How to Run the Project

### Clone the Repository
git clone https://github.com/yourusername/SmartCart-Customer-Segmentation.git


### Navigate to the Project Folder
cd SmartCart-Customer-Segmentation


### Install Dependencies
pip install -r requirements.txt


### Run the Notebook
Open the Jupyter notebook:
customer_segmentation.ipynb

---

## Future Improvements

Possible enhancements include:

- Implementing **DBSCAN clustering**
- Building an **interactive dashboard**
- Deploying the model as a **web application**
- Integrating real-time customer data
- Building a **recommendation system**

---

## Learning Outcomes

This project demonstrates:

- Unsupervised Machine Learning
- Customer Segmentation
- Clustering Algorithms
- Feature Engineering
- PCA for dimensionality reduction
- Data visualization

---

## Author

**Syed Shavez Jafar**  
Machine Learning & AI Enthusiast  

Minor Project – Unsupervised Machine Learning  
Customer Segmentation using Clustering