<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/ca/Walmart_logo.svg/1280px-Walmart_logo.svg.png" alt="Walmart Logo" width="200" align="right"/>

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
