# Customer Segmentation Project
This project performs **customer segmentation** for a mall using the **Mall Customer Dataset**. The goal is to group customers based on **annual income** and **spending score** to help marketing teams target different customer segments effectively.

We use **unsupervised learning** (K-Means clustering) to find natural groups in the data.

---

## **Project Structure**

```
customer_segmentation/
│
├── segmentation_eda.ipynb          # Exploratory Data Analysis & finding best number of clusters
├── segmentation_model_training.ipynb  # K-Means clustering and cluster visualization
├── segmentation_report.docx        # 2-page report explaining clusters and insights
├── Mall_Customers.csv              # Dataset
└── README.md                       # Project overview
```

---

## **Key Features**

* **Exploratory Data Analysis (EDA):** Visualize income and spending patterns.
* **K-Means Clustering:** Segment customers into meaningful groups.
* **Cluster Insights:** Identify high spenders, cautious spenders, and target customers.
* **Visualization:** Scatter plots showing clusters with distinct colors.

---

## **Customer Segments**

| Cluster | Name               | Description                                                  |
| ------- | ------------------ | ------------------------------------------------------------ |
| 0       | Target Customers   | Medium income, medium spending. Regular shoppers.            |
| 1       | Careful Customers  | High income, high spending. Premium buyers.                  |
| 2       | Big Spenders       | Low income, high spending. Budget-conscious but like to buy. |
| 3       | Spenders on Budget | High income, low spending. Cautious shoppers.                |

---

## **Usage**

1. Clone the repository:

```bash
git clone 
```

2. Open the notebooks in **Jupyter Notebook** or **Jupyter Lab**.

3. Run `segmentation_eda.ipynb` first to explore data and determine the best number of clusters.

4. Run `segmentation_model_training.ipynb` to train K-Means and visualize clusters.

---

## **Insights**

* High-spending and target customer groups can be prioritized for marketing campaigns.
* Low-spending customers indicate opportunities for discounts and promotions.
* Unsupervised learning like K-Means helps **find patterns without labels**.

---

## **Tools & Libraries**

* Python 3
* Pandas, NumPy
* Matplotlib, Seaborn
* scikit-learn (K-Means)
