# E-Retail Customer Segmentation using K-Means Clustering

## Project Overview

Customer segmentation is a key technique in retail and marketing, helping businesses understand their customers better by grouping them based on purchasing behavior and characteristics. This project applies the K-Means clustering algorithm to segment customers from an e-retail dataset. The segmentation helps to identify distinct customer groups, which can then be targeted with tailored marketing strategies to improve customer retention and maximize revenue.

---

## Dataset Description

The dataset contains transactional data from an e-retail business, which includes:

* **InvoiceNo**: Invoice number (unique for each transaction)
* **StockCode**: Product code
* **Description**: Product description
* **Quantity**: Number of items purchased
* **InvoiceDate**: Date and time of transaction
* **UnitPrice**: Price per unit
* **CustomerID**: Unique identifier for each customer
* **Country**: Customer's country of residence

The data preprocessing steps involve cleaning missing values, removing canceled transactions (identified by invoice numbers starting with 'C'), and aggregating the data to compute relevant features for clustering.

---

## Objective

* Perform exploratory data analysis (EDA) to understand customer purchase behavior.
* Create meaningful features such as **Recency, Frequency, and Monetary value (RFM)** for each customer.
* Apply K-Means clustering to segment customers into distinct groups.
* Analyze the resulting clusters to draw actionable insights.

---

## Methodology

1. **Data Cleaning & Preprocessing**

   * Removed missing Customer IDs and canceled transactions.
   * Converted dates to datetime format.
   * Calculated total spend per transaction.

2. **Feature Engineering: RFM Metrics**

   * **Recency:** Number of days since last purchase.
   * **Frequency:** Number of transactions made.
   * **Monetary:** Total amount spent.

3. **Data Scaling**

   * Scaled RFM features using StandardScaler to normalize data.

4. **K-Means Clustering**

   * Applied the Elbow method to determine the optimal number of clusters.
   * Performed clustering and assigned cluster labels to each customer.

5. **Cluster Profiling**

   * Analyzed clusters by comparing average RFM values.
   * Interpreted clusters to identify loyal customers, potential churners, and high spenders.

---

## Results & Insights

* Identified **4 distinct customer segments** with varying buying behaviors:

  * **Cluster 0:** Loyal customers with high frequency and monetary value.
  * **Cluster 1:** Recent customers with moderate spending.
  * **Cluster 2:** Customers with low recency and frequency – likely inactive.
  * **Cluster 3:** Big spenders but infrequent buyers.

* These insights allow targeted marketing strategies:

  * Reward loyal customers.
  * Engage inactive customers with promotions.
  * Upsell to high-value but infrequent buyers.

---

## How to Use This Notebook

* Load the dataset.
* Run data cleaning and preprocessing cells.
* Perform EDA to explore trends.
* Compute RFM features.
* Run clustering and analyze results.
* Modify cluster count or features as needed for deeper analysis.

---

## Future Work

* Incorporate additional features like product categories or customer demographics.
* Use advanced clustering algorithms (e.g., DBSCAN, hierarchical clustering).
* Perform time-based segmentation for evolving customer behavior.
* Build predictive models based on customer segments.

---

## Requirements

* Python 3.x
* Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## References

* Kaggle tutorials on customer segmentation.
* [K-Means clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html) documentation.
* Marketing analytics resources on RFM analysis.

---

## 👤 Author

* 👨‍💻 **Rahul Kumar Sharma**
* 🎓 Bachelor of Technology, Mining Engineering
* 🏫 IIT (ISM) Dhanbad
* 📧 Email: [20je0749@iitism.ac.in](mailto:20je0749@iitism.ac.in)
* 📞 Contact: +91-9508476508
* 🌐 GitHub: [github.com/Rahul29999](https://github.com/Rahul29999)
* 🔗 LinkedIn: [linkedin.com/in/rahul-kumar-sharma-aa0b57233](https://linkedin.com/in/rahul-kumar-sharma-aa0b57233)
* 📊 Kaggle: [kaggle.com/oops26/code](https://www.kaggle.com/oops26/code)
