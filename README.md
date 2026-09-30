# Customer Segmentation Using K-Means Clustering

## 📌 Project Overview

Customer Segmentation is an unsupervised machine learning project that groups customers into different clusters based on their **Annual Income** and **Spending Score**.

This project uses the K-Means Clustering algorithm to identify customer groups with similar spending behavior. Businesses can use these insights to understand their customers and plan targeted marketing strategies.

## 🎯 Objectives

* Analyze customer data to understand customer behavior.
* Perform data cleaning and exploratory data analysis (EDA).
* Visualize customer age, annual income, and spending score distributions.
* Apply feature scaling using StandardScaler.
* Determine the number of clusters using the Elbow Method.
* Group customers using K-Means Clustering.
* Predict the cluster of new customers.

## 📂 Dataset

**Dataset:** Mall Customers Dataset

The dataset contains customer information, including:

* CustomerID
* Gender
* Age
* Annual Income (k$)
* Spending Score (1-100)

The clustering model uses **Annual Income** and **Spending Score (1-100)** as its input features.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## ⚙️ Project Workflow

### 1. Import Libraries

Imported the required Python libraries for data manipulation, visualization, feature scaling, and clustering.

### 2. Load the Dataset

Loaded the Mall Customers dataset using Pandas and examined the first few rows.

### 3. Data Exploration

* Checked the number of rows and columns.
* Examined column names and data types.
* Generated descriptive statistics.
* Checked for missing values.
* Identified and removed duplicate records.

### 4. Exploratory Data Analysis (EDA)

Created histograms to understand the distributions of:

* Customer Age
* Annual Income
* Spending Score

### 5. Feature Selection

Selected two features for clustering:

* Annual Income (k$)
* Spending Score (1-100)

### 6. Feature Scaling

Applied `StandardScaler` to standardize the selected features so that differences in their scales do not disproportionately affect the clustering process.

### 7. Find the Optimal Number of Clusters

Used the **Elbow Method** to calculate Within-Cluster Sum of Squares (WCSS) for different values of K, from 1 to 10.

The WCSS values were plotted to help identify a suitable number of clusters.

### 8. Apply K-Means Clustering

Built the K-Means model using five clusters and assigned each customer to a cluster.

### 9. Visualize Customer Segments

Created a scatter plot to visualize the customer clusters based on annual income and spending score.

### 10. Analyze Customer Segments

Calculated the average age, annual income, and spending score for each cluster using Pandas `groupby()`.

### 11. Predict New Customers

Used the trained model to predict the cluster membership of new customers based on their annual income and spending score.

## 📊 Algorithm Used: K-Means Clustering

K-Means is an **unsupervised machine learning algorithm** that divides data points into K clusters based on their similarity.

The algorithm works by:

1. Selecting the number of clusters, K.
2. Assigning data points to their nearest cluster centroid.
3. Updating the centroids based on the assigned points.
4. Repeating the process until the clusters converge.

The objective is to minimize the distance between data points and their assigned cluster centroids.

## 📈 Results

The project generates:

* Histograms showing customer data distributions.
* An Elbow Method plot for selecting the number of clusters.
* A scatter plot displaying customer segments.
* A summary of average customer characteristics for each cluster.
* Cluster predictions for new customer records.

These outputs help explore patterns in customer income and spending behavior.

## 💡 Business Applications

Customer segmentation can help businesses:

* Understand different customer spending patterns.
* Develop targeted marketing campaigns.
* Personalize offers and promotions.
* Identify customer groups for further analysis.
* Support data-driven business decisions.

## 🚀 How to Run the Project

1. Clone or download this repository.

2. Make sure Python and Jupyter Notebook are installed.

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scikit-learn jupyter
   ```

4. Place `Mall_Customers.csv` in the appropriate project directory.

5. Open `customer_segmentation.ipynb` in Jupyter Notebook.

6. Run the notebook cells in order.

## 📁 Project Structure

```text
Customer-Segmentation/
│
├── customer_segmentation.ipynb
├── Mall_Customers.csv
└── README.md
```

*Note: The dataset file should be included in the repository if you have permission to redistribute it.*

## 👩‍💻 Author

**Vaishnavi Rai**

B.Com Graduate | Aspiring Data Analyst | Data Science Enthusiast

Skills: Python, Pandas, NumPy, Matplotlib, Machine Learning, Data Analysis

---

⭐ If you find this project useful, feel free to explore the notebook and learn more about customer segmentation using machine learning.

