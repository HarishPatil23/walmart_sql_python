
# Walmart Sales Data Analysis  
### End-to-End SQL + Python Project

---

## Project Overview
This is a complete **end-to-end data analysis project** that extracts powerful business insights from Walmart sales data using **Python** for data processing & cleaning and **MySQL** for advanced querying and analytics.

Perfect for data analysts, data enthusiasts, and anyone preparing for interviews — this project covers real-world skills:  
- Kaggle API automation  
- Data cleaning & feature engineering  
- Loading data into MySQL using Python  
- Writing complex, business-oriented SQL queries  

---

## Project Pipeline
**Environment Setup → Data Download (Kaggle API) → Exploration & Cleaning → Feature Engineering → Load to MySQL → Advanced SQL Analysis → Documentation**

---

## Project Steps

### 1. Set Up the Environment  
**Tools Used**: Visual Studio Code, Python, MySQL  
**Goal**: Create a clean, organized workspace and folder structure.

### 2. Set Up Kaggle API  
- Go to your Kaggle profile → Settings → Create New Token → Download `kaggle.json`  
- Place `kaggle.json` in `C:\Users\<YourUser>\.kaggle\` (Windows) or `~/.kaggle/` (Mac/Linux)  
- Download dataset using:  
```bash

kaggle datasets download -d najir0123/walmart-10k-sales-datasets

3. Download Walmart Sales Data
Dataset: Walmart Sales Dataset (10K+ rows)
Storage: All raw & cleaned files are saved in the data/ folder.
4. Install Required Libraries
Bashpip install pandas numpy sqlalchemy mysql-connector-python
5. Data Exploration

Understand structure using .head(), .info(), .describe()
Identify missing values, duplicates, and incorrect data types

6. Data Cleaning (Critical Step)
Tasks Performed:

Removed duplicates
Handled missing values
Fixed data types (especially Date → datetime, Price → float)
Cleaned currency symbols and formatting
Final validation of cleaned dataset

7. Feature Engineering
New Column Added:

Total_Amount = Unit_Price × Quantity
This enables faster aggregations in SQL later.

8. Load Cleaned Data into MySQL

Automated connection & table creation using SQLAlchemy + pandas
Data successfully loaded into MySQL database
Verified with sample SQL queries

9. Advanced SQL Analysis (The Core!)
Wrote complex, production-level SQL queries to answer real business questions such as:

Total revenue by branch, city, and product category
Best-selling & most profitable product categories
Peak sales hours and days
Payment method preferences
Highest-rated branches and customer behavior trends
Gross margin analysis

All queries are saved in the sql_queries/ folder with clear comments.
10. Documentation & Publishing

Full project pushed to GitHub
Clean folder structure
Professional README (this file)
Easy to run and reproduce


Requirements

Python 3.8+
MySQL (Local or cloud instance)
Python Libraries (listed in requirements.txt)
Kaggle Account (for API key)


Getting Started (Quick Start)
Bashgit clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
Then follow the steps in main.py or the Jupyter notebook to:

Download data
Clean & engineer features
Load into MySQL
Run powerful SQL analysis


Project Structure
text├── data/                  # Raw & cleaned CSV files
├── sql_queries/           # All SQL scripts (well-commented)
├── notebooks/             # Optional Jupyter notebook (if used)
├── main.py                # Main Python script
├── requirements.txt       # Python dependencies
├── README.md              # You are here
└── walmart_sales_clean.csv (generated after cleaning)

Key Results & Business Insights (Sample)
