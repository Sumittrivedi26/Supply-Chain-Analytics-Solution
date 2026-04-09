# 📊 Revenue Analysis using SQL

## 🚀 Project Overview

This project focuses on **end-to-end data analysis using SQL**, starting from database creation to data cleaning and finally deriving meaningful business insights.

The dataset simulates a **retail sales environment**, including:

* Products
* Stores
* Sales transactions
* Date dimension

The goal is to transform raw, inconsistent data into a **clean, analysis-ready dataset** and answer key business questions related to revenue.

---

## 🗂️ Database Schema

The project consists of four main tables:

### 1. **Products**

* ProductID (Primary Key)
* ProductName
* Category

### 2. **Store**

* StoreID (Primary Key)
* StoreName
* Region

### 3. **Sales**

* TransactionID (Primary Key)
* Date (Foreign Key)
* StoreID (Foreign Key)
* ProductID (Foreign Key)
* UnitsSold
* UnitPrice

### 4. **DateDim**

* Date (Primary Key)
* Year, Month, MonthName
* Quarter
* IsCurrentQuarter

---

## 🛠️ Key Steps Performed

### 🔹 1. Database & Table Creation

* Created relational schema with **primary and foreign key constraints**
* Generated a **Date Dimension table** dynamically
* Inserted sample data with intentional inconsistencies

---

### 🔹 2. Data Cleaning & Preprocessing

#### ✅ Handling Null Values

* Replaced categorical nulls with `'UNKNOWN'`
* Imputed numerical nulls using **average values**

#### ✅ Standardization

* Converted text columns to **UPPERCASE**
* Removed leading/trailing spaces using `TRIM()` and `LTRIM()`

#### ✅ Duplicate Removal

* Identified duplicates using `ROW_NUMBER()`
* Removed redundant records safely

#### ✅ Data Validation

* Checked:

  * Null values
  * Duplicate records
  * Invalid entries (e.g., negative UnitsSold)

#### ✅ Data Correction

* Converted negative values using `ABS()`
* Ensured consistency across categorical fields

---

## 📈 Business Insights

### 🏪 1. Total Revenue per Store (Last Quarter)

* Identified highest performing stores based on recent sales

---

### 🛍️ 2. Top 5 Products by Revenue

* Ranked products using:

  * `SUM()`
  * `DENSE_RANK()` / `TOP`

---

### 📅 3. Monthly Sales Trend

* Analyzed revenue trends over time
* Example: Sales performance of **Baseball Cap**

---

### 🥇 4. Best-Selling Product by Category

* Used window functions to identify:

  * Top product in each category

---

### ⚙️ 5. Parameterized Queries

* Enabled dynamic filtering using variables:

  * Example: Filter by category (`APPAREL`, `ELECTRONICS`, etc.)

---

## 🧠 SQL Concepts Used

* Joins (`INNER`, `LEFT`)
* Aggregations (`SUM`, `AVG`, `COUNT`)
* Window Functions (`ROW_NUMBER`, `DENSE_RANK`)
* Subqueries & CTEs
* Data Cleaning Functions (`TRIM`, `UPPER`, `ABS`)
* Date Functions (`YEAR`, `MONTH`, `QUARTER`)
* Conditional Logic (`CASE WHEN`)

---

## 💡 Key Learnings

* Importance of **data cleaning before analysis**
* Handling real-world issues like:

  * Missing values
  * Duplicates
  * Inconsistent formatting
* Writing **optimized and scalable SQL queries**
* Using **analytical functions** for ranking and trends

---

## ⚡ Tools & Technologies

* SQL (Snowflake & SQL Server compatible)
* Relational Database Concepts

---

## 📌 How to Run

1. Create the database:

   ```sql
   CREATE DATABASE Sales_Analysis;
   ```

2. Run table creation scripts

3. Insert the data

4. Execute:

   * Data Cleaning Queries
   * Business Analysis Queries

---

## 📊 Future Enhancements

* Connect with **Power BI / Tableau** for visualization
* Add more advanced KPIs (YoY growth, MoM trends)
* Implement **stored procedures** for automation
* Extend dataset for predictive analytics

---

## 🤝 Contributing

Feel free to fork this repository and enhance the analysis with more insights or visualizations.

---

## 📬 Contact

If you have any questions or suggestions, feel free to reach out!

---

⭐ **If you like this project, don’t forget to give it a star!**
# 📊 Revenue Analysis using SQL

## 🚀 Project Overview

This project focuses on **end-to-end data analysis using SQL**, starting from database creation to data cleaning and finally deriving meaningful business insights.

The dataset simulates a **retail sales environment**, including:

* Products
* Stores
* Sales transactions
* Date dimension

The goal is to transform raw, inconsistent data into a **clean, analysis-ready dataset** and answer key business questions related to revenue.

---

## 🗂️ Database Schema

The project consists of four main tables:

### 1. **Products**

* ProductID (Primary Key)
* ProductName
* Category

### 2. **Store**

* StoreID (Primary Key)
* StoreName
* Region

### 3. **Sales**

* TransactionID (Primary Key)
* Date (Foreign Key)
* StoreID (Foreign Key)
* ProductID (Foreign Key)
* UnitsSold
* UnitPrice

### 4. **DateDim**

* Date (Primary Key)
* Year, Month, MonthName
* Quarter
* IsCurrentQuarter

---

## 🛠️ Key Steps Performed

### 🔹 1. Database & Table Creation

* Created relational schema with **primary and foreign key constraints**
* Generated a **Date Dimension table** dynamically
* Inserted sample data with intentional inconsistencies

---

### 🔹 2. Data Cleaning & Preprocessing

#### ✅ Handling Null Values

* Replaced categorical nulls with `'UNKNOWN'`
* Imputed numerical nulls using **average values**

#### ✅ Standardization

* Converted text columns to **UPPERCASE**
* Removed leading/trailing spaces using `TRIM()` and `LTRIM()`

#### ✅ Duplicate Removal

* Identified duplicates using `ROW_NUMBER()`
* Removed redundant records safely

#### ✅ Data Validation

* Checked:

  * Null values
  * Duplicate records
  * Invalid entries (e.g., negative UnitsSold)

#### ✅ Data Correction

* Converted negative values using `ABS()`
* Ensured consistency across categorical fields

---

## 📈 Business Insights

### 🏪 1. Total Revenue per Store (Last Quarter)

* Identified highest performing stores based on recent sales

---

### 🛍️ 2. Top 5 Products by Revenue

* Ranked products using:

  * `SUM()`
  * `DENSE_RANK()` / `TOP`

---

### 📅 3. Monthly Sales Trend

* Analyzed revenue trends over time
* Example: Sales performance of **Baseball Cap**

---

### 🥇 4. Best-Selling Product by Category

* Used window functions to identify:

  * Top product in each category

---

### ⚙️ 5. Parameterized Queries

* Enabled dynamic filtering using variables:

  * Example: Filter by category (`APPAREL`, `ELECTRONICS`, etc.)

---

## 🧠 SQL Concepts Used

* Joins (`INNER`, `LEFT`)
* Aggregations (`SUM`, `AVG`, `COUNT`)
* Window Functions (`ROW_NUMBER`, `DENSE_RANK`)
* Subqueries & CTEs
* Data Cleaning Functions (`TRIM`, `UPPER`, `ABS`)
* Date Functions (`YEAR`, `MONTH`, `QUARTER`)
* Conditional Logic (`CASE WHEN`)

---

## 💡 Key Learnings

* Importance of **data cleaning before analysis**
* Handling real-world issues like:

  * Missing values
  * Duplicates
  * Inconsistent formatting
* Writing **optimized and scalable SQL queries**
* Using **analytical functions** for ranking and trends

---

## ⚡ Tools & Technologies

* SQL (Snowflake & SQL Server compatible)
* Relational Database Concepts

---

## 📌 How to Run

1. Create the database:

   ```sql
   CREATE DATABASE Sales_Analysis;
   ```

2. Run table creation scripts

3. Insert the data

4. Execute:

   * Data Cleaning Queries
   * Business Analysis Queries

---

## 📊 Future Enhancements

* Connect with **Power BI / Tableau** for visualization
* Add more advanced KPIs (YoY growth, MoM trends)
* Implement **stored procedures** for automation
* Extend dataset for predictive analytics

---

## 🤝 Contributing

Feel free to fork this repository and enhance the analysis with more insights or visualizations.

---

## 📬 Contact

If you have any questions or suggestions, feel free to reach out!

---

⭐ **If you like this project, don’t forget to give it a star!**
