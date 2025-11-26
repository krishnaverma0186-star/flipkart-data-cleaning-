# 🛍️ Flipkart Data Cleaning and Exploratory Analysis

This repository contains the data and analysis for cleaning and performing initial exploration on a dataset of Flipkart product listings. The primary goal was to handle missing values and prepare the data for more advanced analysis, followed by basic data exploration.

---

## 📁 Project Contents

* **`flipkart_dataset_dirty.csv`**: The original, raw dataset containing missing values in several columns.
* **`flipkart.ipynb`**: A Jupyter Notebook detailing the step-by-step process of data cleaning, preprocessing, feature engineering (like renaming the price column), and basic exploration.

---

## ✨ Key Analysis & Cleaning Steps

The `flipkart.ipynb` notebook covers the following key stages of the project:

1.  **Environment Setup:** Ensuring necessary libraries (like Pandas) are installed and imported.
2.  **Initial Data Inspection:** Checking data types and identifying missing values across various columns.
3.  **Handling Missing Values:**
    * Missing values in the **`Stock`** column were imputed using the mean stock value.
    * Other missing values (e.g., in `Brand` and `Ratings`) were addressed using appropriate strategies (e.g., mode imputation or removal, detailed in the notebook).
4.  **Data Transformation:** Renaming the `Price` column to `Product_price` for clarity.
5.  **Data Type Correction:** Ensuring all columns (e.g., `Ratings` as a float, `Is_Prime` as boolean) are correctly formatted.

---

## 📊 Data Dictionary

The dataset consists of 1000 records with the following attributes:

| Column Name | Data Type (Cleaned) | Description |
| :--- | :--- | :--- |
| **Product_ID** | `object` | Unique identifier for the product. |
| **Product_Name** | `object` | The general category (e.g., Camera, Shoes). |
| **Brand** | `object` | The product's brand. |
| **Product_price** | `int64` | The product's price in INR (Original: `Price`). |
| **Discount_%** | `int64` | The discount percentage offered. |
| **Ratings** | `float64` | Customer rating of the product. |
| **Stock** | `float64` | Current quantity of the product in stock. |
| **Delivery_Time_days** | `int64` | Estimated delivery time in days. |
| **Return_Policy_Days** | `int64` | The return window offered. |
| **Is_Prime** | `bool` | Eligibility for fast/Prime shipping. |

---

## 💻 How to Run the Project

### Prerequisites

To run the notebook locally, you need a Python environment with **Jupyter** installed, and the following core library:

```bash
pip install pandas
