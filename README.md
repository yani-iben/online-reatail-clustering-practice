# Customer Segmentation with K-Means Clustering  
**Using the Online Retail Dataset from UCI Machine Learning Repository**

## 📊 Overview
This project applies customer segmentation techniques on the **Online Retail dataset** provided by the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail). By leveraging **exploratory data analysis**, **data cleaning**, **outlier detection**, and **K-Means clustering**, the project identifies key customer clusters and generates tailored business recommendations based on their purchasing behavior.

---

## 🧠 Skills Demonstrated
- **Exploratory Data Analysis (EDA):** Visualized patterns in customer behavior, transaction trends, and purchasing frequency.
- **Data Cleaning:** Removed null values, duplicate entries, and erroneous data to ensure high-quality inputs.
- **Outlier Detection:** Identified and separated outlier customers to avoid skewing clustering results.
- **K-Means Clustering:** 
  - Applied K-Means to non-outlier customer data to detect meaningful groupings based on Recency, Frequency, and Monetary value (RFM).
  - Ran K-Means separately on outlier segments to investigate high-impact customer clusters.

---

## 📌 Dataset
- **Name:** Online Retail
- **Source:** UCI Machine Learning Repository
- **Records:** Transactions from a UK-based online retail store between 2010–2011.
- **Features Used:**  
  - `InvoiceNo`, `StockCode`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 📈 Project Workflow
1. **Data Import & Initial Exploration**
2. **Data Cleaning**
   - Removed rows with missing `CustomerID`s and non-positive `Quantity`
   - Converted date fields to datetime format
3. **Feature Engineering**
   - Calculated **Recency**, **Frequency**, and **Monetary Value** for each customer
4. **Outlier Detection**
   - Used visual and statistical methods to separate outliers from the main dataset
5. **Scaling & Clustering**
   - Standardized RFM values using `StandardScaler`
   - Determined optimal cluster number using the **elbow method** and **silhouette score**
   - Performed K-Means clustering on:
     - Non-outlier customers
     - Outlier customers
6. **Interpretation & Recommendations**
   - Generated insights and tailored strategies for each identified segment

---

## 💡 Key Takeaways & Business Recommendations
- **Segmented customers** into actionable groups, such as:
  - High-value loyal customers
  - At-risk or one-time buyers
  - Potentially high-value but inactive customers
- **Recommendations include:**
  - Loyalty programs for high-frequency customers
  - Re-engagement campaigns for inactive but previously high-spending customers
  - Personalized offers and priority support for top outlier spenders

---

## 🛠 Tools Used
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **scikit-learn (KMeans, StandardScaler, silhouette_score)**

---

## 📂 Repository Structure
