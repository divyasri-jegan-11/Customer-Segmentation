# Customer-Segmentation
Customer Segmentation using K-Means Clustering

## 📌 Project Overview
In this project, we aim to transform transactional data into a customer-centric dataset by creating new features that will facilitate the segmentation of customers into distinct groups using the K-means clustering algorithm. This segmentation will allow us to understand the unique profiles and preferences of various customer groups, thus amplifying the efficiency of marketing strategies and fostering increased sales. Subsequently, we intend to develop a recommendation system that suggests top-selling products to customers within each segment who haven't purchased those items yet, enhancing marketing efficacy and fostering increased sales.

## 📊 Dataset Information
The dataset consists of online retail transactions with the following columns:

| Column       | Description                                      |
|-------------|--------------------------------------------------|
| InvoiceNo   | Unique identifier for each transaction          |
| StockCode   | Product code                                    |
| Description | Product name (some missing values)             |
| Quantity    | Number of items purchased                      |
| InvoiceDate | Date and time of the transaction               |
| UnitPrice   | Price per unit of the product                  |
| CustomerID  | Unique customer identifier (some missing values) |
| Country     | Country where the transaction took place       |

## 🔧 Preprocessing Steps
1. **Handle Missing Values**: Dropped rows where `CustomerID` is missing.
2. **Convert Data Types**: Changed `InvoiceDate` to datetime format.
3. **Feature Engineering**:
   - Created a `TotalPrice` column (`Quantity * UnitPrice`).
   - Computed RFM metrics: `Recency`, `Frequency`, and `Monetary`.

## 🚀 Customer Segmentation Approach
### 1️⃣ **RFM Analysis**
- **Recency**: Number of days since the customer's last purchase.
- **Frequency**: Total number of transactions per customer.
- **Monetary**: Total amount spent by each customer.

### 2️⃣ **K-Means Clustering**
- Standardized the RFM values for better clustering.
- Used the **Elbow Method** to determine the optimal number of clusters.
- Applied K-Means to segment customers into groups.

## 📈 Key Findings
1. **High-Value Customers**: Recently purchased, high spending, frequent buyers.
2. **Frequent Shoppers**: Regular buyers but moderate spending.
3. **Inactive Customers**: Haven't purchased in a long time, low spending.
4. **New Customers**: Recent buyers with lower frequency.
5. **Recommendation System** : For better market increase of products.

## 🔥 How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/divyasri-jegan-11/customer-segmentation.git
   ```
2. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

## 📌 Next Steps
✅ Add machine learning predictions in Power BI using Python.

✅ Perform advanced clustering techniques (Hierarchical, DBSCAN).

✅ Expand analysis with **geographic segmentation**.

## 📈 What was the learning??

-- got insights about handling data and how customers data help in handling the sales.



