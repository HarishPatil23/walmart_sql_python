
# Walmart Sales Data Analysis  
### End-to-End SQL + Python Project (MySQL)

---

## Project Overview
This project is an **end-to-end data analysis solution** designed to extract critical business insights from Walmart sales data.  

We utilize:
- **Python** for data processing, cleaning, and automation  
- **MySQL** for advanced querying and analytics  
- Structured problem-solving to answer real-world business questions  

Ideal for data analysts, job seekers, and portfolio building — this project demonstrates full-cycle skills: **data ingestion → cleaning → feature engineering → database loading → complex SQL analysis**.

---

## Project Steps

### 1. Set Up the Environment
**Tools Used**: Visual Studio Code (VS Code), Python, MySQL  
**Goal**: Create a structured workspace and organize project folders for smooth development and data handling.

### 2. Set Up Kaggle API
**API Setup**:  
- Go to [Kaggle → Account → Settings → Create New Token](https://www.kaggle.com/settings)  
- Download `kaggle.json`  
**Configure Kaggle**:  
- Place `kaggle.json` in `C:\Users\<YourUser>\.kaggle\` (Windows) or `~/.kaggle/` (Mac/Linux)  
- Use the command `kaggle datasets download -d <dataset-path>` to pull datasets directly into your project.

### 3. Download Walmart Sales Data
- **Data Source:** Use the Kaggle API to download the Walmart sales datasets from Kaggle.
- **Dataset Link:** [Walmart Sales Dataset](https://www.kaggle.com/datasets/najir0123/walmart-10k-sales-datasets)
- **Storage:** Save the data in the `data/` folder for easy reference and access.

### 4. Install Required Libraries and Load Data
- **Libraries:** Install necessary Python libraries using:
```bash
pip install pandas numpy sqlalchemy mysql-connector-python
```
- **Loading Data:** Read the data into a Pandas DataFrame for initial analysis and transformations.

### 5. Explore the Data
- Goal: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
- Analysis: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 6. Data Cleaning
- **Remove Duplicates:** Identify and remove duplicate entries to avoid skewed results.
- **Handle Missing Values:** Drop rows or columns with missing values if they are insignificant; fill values where essential.
- **Fix Data Types:** Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
- **Currency Formatting:** Use `.replace()` to handle and format currency values for analysis.
- **Validation:** Check for any remaining inconsistencies and verify the cleaned data.

### 7. Feature Engineering
**Create New Columns:** Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
**Enhance Dataset:** Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 8. Load Data into MySQL 
- **Set Up Connections:** Connect to MySQL using `sqlalchemy` and load the cleaned data into each database.
- **Table Creation:** Set up tables in MySQL using Python SQLAlchemy to automate table creation and data insertion.
- **Verification:** Run initial SQL queries to confirm that the data has been loaded accurately.

### 9. SQL Analysis: Complex Queries and Business Problem Solving
- Business Problem-Solving: Write and execute complex SQL queries to answer critical business questions, such as:
### Category A — Sales & Revenue Analysis
| # | Business Question | Purpose |
|---|-------------------|--------|
| **Q1** | Analyze Payment Methods and Sales | Understand customer payment preferences |
| **Q2** | Total Quantity Sold by Payment Method | Identify sales volume per payment channel |
| **Q3** | Best-Selling Category per Branch | Optimize product placement & inventory |
| **Q4** | Revenue Contribution by Category (%) | Focus on high-revenue drivers |
| **Q5** | Average Basket Size (Items per Invoice) | Measure cross-selling effectiveness |
| **Q6** | Highest Revenue Day per Month | Detect seasonal & monthly peaks |
| **Q7** | Total Profit by Category | Identify most profitable product lines |

### Category B — Ratings, Profit & Quality Insights
| # | Business Question | Purpose |
|---|-------------------|--------|
| **Q8** | Highest-Rated Category in Each Branch | Promote customer-favorite categories |
| **Q9** | Category Ratings by City (Avg, Min, Max) | Improve city-level customer experience |
| **Q10** | Rating vs Sales Analysis (High Sales, Low Rating) | Flag categories needing quality improvement |
| **Q11** | Profit by Branch | Evaluate branch-level financial performance |

### Category C — Branch & Time-Based Operational Insights
| # | Business Question | Purpose |
|---|-------------------|--------|
| **Q12** | Busiest Day for Each Branch | Optimize staffing & inventory planning |
| **Q13** | Most Common Payment Method per Branch | Improve checkout efficiency |
| **Q14** | Sales by Shift (Morning/Afternoon/Evening/Night) | Better shift management & replenishment |
| **Q15** | Branch Revenue Decline YoY | Early detection of underperforming branches |

---

10. Project Publishing and Documentation
Documentation: Maintain well-structured documentation of the entire process in Markdown or a Jupyter Notebook.
Project Publishing: Publish the completed project on GitHub or any other version control platform, including:
The README.md file (this document).
Jupyter Notebooks (if applicable).
SQL query scripts.
Data files (if possible) or steps to access them.
Requirements
Python 3.8+
SQL Databases: MySQL, PostgreSQL
Python Libraries:
pandas, numpy, sqlalchemy, mysql-connector-python, psycopg2
Kaggle API Key (for data downloading)
Getting Started
Clone the repository:
git clone <repo-url>
Install Python libraries:
pip install -r requirements.txt
Set up your Kaggle API, download the data, and follow the steps to load and analyze.
Project Structure
|-- data/                     # Raw data and transformed data
|-- sql_queries/              # SQL scripts for analysis and queries
|-- notebooks/                # Jupyter notebooks for Python analysis
|-- README.md                 # Project documentation
|-- requirements.txt          # List of required Python libraries
|-- main.py                   # Main script for loading, cleaning, and processing data
Results and Insights
This section will include your analysis findings:

Sales Insights: Key categories, branches with highest sales, and preferred payment methods.
Profitability: Insights into the most profitable product categories and locations.
Customer Behavior: Trends in ratings, payment preferences, and peak shopping hours.
Future Enhancements
Possible extensions to this project:

Integration with a dashboard tool (e.g., Power BI or Tableau) for interactive visualization.
Additional data sources to enhance analysis depth.
Automation of the data pipeline for real-time data ingestion and analysis.
License
This project is licensed under the MIT License.

Acknowledgments
Data Source: Kaggle’s Walmart Sales Dataset
Inspiration: Walmart’s business case studies on sales and supply chain optimization.
