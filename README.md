# Customer Segmentation Analysis for E-commerce Company

## 📌 Project Overview

This project focuses on **Customer Segmentation Analysis** for an e-commerce company using real customer transaction data. The primary goal is to segment customers based on their purchasing behavior and demographics to inform **targeted marketing strategies**, **increase customer satisfaction**, and **optimize business decisions**.

The project leverages data preprocessing, feature engineering, exploratory data analysis (EDA), clustering with K-Means, and dimensionality reduction using PCA. Final results were exported and visualized in a **Power BI interactive dashboard**.

---

## 🧰 Technologies & Libraries Used

* **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
* **Machine Learning**: StandardScaler, KMeans, PCA, Silhouette Analysis
* **Power BI**: For interactive visualizations and reporting

---

## 📂 Dataset

* Dataset source: [Kaggle Notebook](https://www.kaggle.com/code/analystoleksandra/marketing-analytics-customer-segmentation?scriptVersionId=148503162&cellId=6)
* File used: `ifood_df.csv`: https://github.com/Progati00/Customer-Segmentation-Analysis/blob/main/data/ifood_df.csv
  
* Contains customer demographic details, purchase behaviors, campaign responses, and spending history.

---

## ✅ Key Steps Performed

### 1. **Data Loading & Initial Analysis**

* Imported dataset using Pandas.
* Checked dataset info, missing values (none found), and unique values.
* Summarized basic statistics using `.describe()`.

### 2. **Feature Engineering & KPI Calculation**

* Created key metrics:

  * **Average Purchase Value**: `562.76`
  * **Purchase Frequency**: `~14.89`
* Generated new features:

  * `In_relationship`: Indicates if the customer is married or in a relationship.
  * `Marital`: Combined multiple binary columns into a readable status.

### 3. **Exploratory Data Analysis**

* Box plots were used to detect and remove **outliers** in `MntTotal`.
* Additional visualizations:

  * **Spending by Marital Status**
  * **Income Distribution**

### 4. **Clustering Analysis**

* **Selected Features**: `Income`, `Recency`, `In_relationship`, `MntTotal`
* Applied **StandardScaler** for normalization.
* Used **Principal Component Analysis (PCA)** to reduce dimensions for visualization.
* **K-Means Clustering**:

  * Used **Elbow Method** and **Silhouette Score** to determine optimal number of clusters (`K = 4`).
  * Created final customer clusters and added `Cluster` column.

### 5. **Cluster Evaluation & Insights**

* Plotted clusters using PCA components.
* Analyzed product consumption by cluster (bar plot).
* Visualized cluster sizes and behavioral breakdown (relationship status, spending).

### 6. **Power BI Dashboard**

Exported cleaned and enriched dataset (`segmented_ifood.csv`) for visualization in Power BI.
* **Dataset**: https://github.com/Progati00/Customer-Segmentation-Analysis/blob/main/data/segmented_ifood.xls
* **Dashboard**: https://github.com/Progati00/Customer-Segmentation-Analysis/blob/main/dashboards/Customer%20segmentation%20analysis.pbix
  
https://github.com/Progati00/Customer-Segmentation-Analysis/blob/main/dashboards/Customer%20segmentation%20analysis.pdf

This PDF provides a static view of the Power BI dashboard for easier access and preview, especially for users who do not have Power BI installed.


### 🔍 Power BI Dashboard Includes:

* **Cards**: Average Income, Average Spending
* **Slicers**: Education Level, Age Group, Income Level, Marital Status
* **Charts**:

  1. Customer Distribution by Age Group (Pie Chart)
  2. Average Spending by Cluster & Income Level (Stacked Bar Chart)
  3. Campaign Acceptance by Education & Cluster (Clustered Column Chart)
  4. Customer Loyalty by Income Level (Stacked Bar Chart)
  5. Marital Status Distribution by Cluster (Column Chart)
  6. Complaint Status by Marital Status
  7. Spending by Marital Status and Education Level

---

## 📤 Output

* Final dataset with enriched features and cluster labels: `segmented_ifood.csv`
* Can be used directly in Power BI for reporting and advanced visualization.

---

## 🎯 Business Impact

This segmentation model allows the company to:

* Design **tailored marketing campaigns**.
* Understand **high-value customer segments**.
* Optimize **product targeting** and **retention strategies**.
* Track customer **loyalty and satisfaction trends** across various demographics.

---

## 📈 Conclusion

By combining robust data preprocessing, statistical analysis, machine learning clustering, and visualization tools, this project delivers **actionable customer segments** that support **data-driven decision-making** for e-commerce growth.

---
