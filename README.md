# pyspark-amazon-prime-analysis-databricks
End-to-end Data Analysis project using PySpark on Databricks. Analyzes the Amazon Prime Movies &amp; TV Shows dataset to derive business insights through data cleaning, transformation, EDA, and advanced Window Functions. Includes data export to Delta and CSV formats.

# Amazon Prime Movies & TV Shows Analysis: PySpark on Databricks

## 📌 Overview

I have created this project from scratch & published it on my YouTube Channel : www.youtube.com/@DataToCrunch .

<img width="1627" height="918" alt="image" src="https://github.com/user-attachments/assets/298f811a-85a4-4741-a96e-eaaa7818c640" />

This project demonstrates a comprehensive data analysis workflow using **PySpark** and **Databricks**. It follows a structured approach to transform raw Amazon Prime video data into actionable business insights, covering everything from environment setup to advanced analytical rankings and data export.

The analysis provides key metrics on content distribution, genre popularity, and ratings trends to support strategic decision-making.

---

## 🏗️ Workflow
The project is divided into seven major phases:
**Environment Setup** → **Data Ingestion** → **Cleaning** → **Transformation** → **EDA** → **Business Insights** → **Data Export**



---

## ⚙️ Tech Stack
- **Platform:** Databricks
- **Engine:** PySpark
- **Language:** Python
- **Storage:** DBFS (Databricks File System) & Delta Lake
- **Visualization:** Databricks Native Charts

---

## 🔄 Project Implementation

### 🔹 Part 1: Dataset Overview & Ingestion
- **Source:** Amazon Prime Movies and TV Shows dataset.
- **Reading Data:** Ingesting `.csv` files into PySpark DataFrames with defined schemas to ensure data consistency.

### 🔹 Part 2: Data Cleaning
- **Null Handling:** Replacing missing values with business-defined defaults or removing incomplete rows.
- **Deduplication:** Dropping duplicate records to ensure unique content entries.
- **Schema Refinement:** Renaming columns for better readability and alignment with data standards.

### 🔹 Part 3: Data Transformation
- **Feature Engineering:** Creating new derived columns from existing data.
- **Advanced Parsing:** Splitting complex string columns (like `genres` or `cast`) and counting occurrences to understand content variety.

### 🔹 Part 4: Exploratory Data Analysis (EDA)
- **Content Distribution:** Analyzing the ratio between Movies and TV Shows using `groupBy` and `orderBy`.
- **Production Trends:** Tracking content volume produced per year to identify growth patterns.

### 🔹 Part 5: Business Insights
- **Top Rated Content:** Filtering and sorting by ratings to identify high-performing assets.
- **Global Availability:** Aggregating content by country to analyze geographic market reach.

### 🔹 Part 6: Advanced Analytics (Window Functions)
- **Content Ranking:** Using **PySpark Window Functions** to rank content based on ratings within specific years.
- **Logic:** Implementing `partitionBy(year)` and `orderBy(rating.desc())` to find the best content for every production cycle.

---

## 🚀 Key Features
- **Scalable Processing:** Built on PySpark to handle large datasets efficiently.
- **Advanced SQL Logic:** Implementation of complex transformations and analytical functions.
- **Multi-Format Export:** Processed data is exported to **Delta format** (for Lakehouse integration) and **CSV** (for easy sharing).
- **Strategic Recommendations:** Final output includes data-driven advice for content acquisition and marketing strategies.

---

## ▶️ How to Run

1.  **Setup Compute:** Create a Cluster in your Databricks workspace using a standard runtime.
2.  **Import Data:** Upload the dataset to **DBFS** or a **Databricks Volume** to make it accessible to the Spark session.
3.  **Import Notebook:** Upload the provided `.ipynb` file into your Databricks workspace.
4.  **Execute:** Open the notebook and run the cells sequentially to observe the end-to-end cleaning, transformation, and analytical steps.
5.  **Export:** Check your **FileStore** or designated output path for the final generated Delta and CSV files.

---

## 🎥 YouTube Walkthrough

https://youtu.be/7aZGAf8Luys?si=k29Hu7J2brKlnNgQ

---

## 📊 Strategic Recommendations

Based on the data-driven analysis, the project concludes with the following business recommendations:

* **Genre Investment:** Prioritize the acquisition and production of content in high-performing categories identified during the EDA phase.
* **Global Expansion:** Implement targeted marketing campaigns in countries currently showing low content availability but high potential engagement.
* **Rating Optimization:** Use identified patterns from top-rated content (directors, cast, or release timing) to guide future content production and licensing decisions.

---

## 📌 Dataset

**Amazon Prime Movies and TV Shows:** The analysis is based on the comprehensive Kaggle dataset containing metadata for movies and shows available on the platform.

https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows

