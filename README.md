# 🛒 Amazon Product Data Analysis using PySpark

## 📌 Project Overview

This project demonstrates data cleaning and feature engineering using **PySpark** on an Amazon product dataset. The objective is to prepare raw data for analysis by handling missing values, cleaning text, converting data types, and creating meaningful derived columns.

This project is ideal for beginners preparing for **PySpark** and **Data Engineering** interviews.

---

## 🛠️ Technologies Used

- Python
- PySpark
- Google Colab
- Apache Spark

---

## 📂 Dataset

The dataset contains Amazon product information, including:

- Product ID
- Product Name
- Category
- Actual Price
- Discounted Price
- Discount Percentage
- Rating
- Rating Count
- Product Description
- User Reviews

---

## 🔧 Data Cleaning & Transformation Tasks

The following preprocessing steps were performed:

### Data Cleaning

- ✅ Removed duplicate rows
- ✅ Handled null values
- ✅ Removed unwanted columns (`img_link`, `product_link`)
- ✅ Trimmed extra spaces from all string columns
- ✅ Renamed columns for better readability

### Data Type Conversion

- ✅ Removed `₹` symbol from `discounted_price` and `actual_price`
- ✅ Converted `discounted_price` to `Double`
- ✅ Converted `actual_price` to `Double`
- ✅ Removed `%` symbol from `discount_percentage`
- ✅ Converted `discount_percentage` to `Double`
- ✅ Removed commas from `rating_count`
- ✅ Converted `rating_count` to `Integer`
- ✅ Converted `rating` to `Double`

### Feature Engineering

- ✅ Extracted `main_category` from `category`
- ✅ Extracted `sub_category` from `category`
- ✅ Calculated `savings_amount`
- ✅ Calculated `saving_percentage`
- ✅ Created `rating_category`
- ✅ Created `discount_category`
- ✅ Created `price_category`

---

## 📊 New Columns Created

| Column | Description |
|---------|-------------|
| main_category | First category extracted from category column |
| sub_category | Remaining category hierarchy |
| savings_amount | Actual Price - Discounted Price |
| saving_percentage | Percentage saved on each product |
| rating_category | Excellent / Good / Average / Poor |
| discount_category | High / Medium / Low / No Discount |
| price_category | High / Medium / Low |

---

## 🚀 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Feature Engineering
- String Functions
- Conditional Columns
- Data Type Conversion
- PySpark DataFrame API

---

## 📚 PySpark Functions Used

- `withColumn()`
- `withColumnRenamed()`
- `dropDuplicates()`
- `drop()`
- `filter()`
- `select()`
- `split()`
- `slice()`
- `concat_ws()`
- `trim()`
- `regexp_replace()`
- `when()`
- `otherwise()`
- `cast()`
- `col()`
- `round()`

---

## 🎯 Learning Outcome

This project helped me practice real-world data preprocessing techniques commonly used in Data Engineering and Data Analytics projects using PySpark.

---

## 👨‍💻 Author


**Amit Gupta**

Learning PySpark | Data Engineering | Apache Spark
