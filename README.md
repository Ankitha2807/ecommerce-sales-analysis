# E-commerce Sales Analysis

**A Python-based exploratory data analysis project to understand retail sales trends, product performance, and geographical sales distribution.**

## Project Overview

This project analyzes a real-world online retail transaction dataset to identify sales patterns, explore product performance, and compare sales across countries.

Using Python, Pandas, and Matplotlib, the project covers data cleaning, data quality investigation, exploratory data analysis (EDA), and visualization of key business metrics.

## Objectives

- Analyze monthly sales trends and identify high-performing periods.
- Identify products with the highest recorded gross sales.
- Compare sales performance across countries.
- Investigate missing values, duplicate records, cancellations, returns, and zero-price transactions.
- Present findings through clear and informative visualizations.

## Dataset

**Dataset:** Online Retail

**Source:** [UCI Machine Learning Repository — Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail)

The dataset contains transactions from a UK-based online retail business between December 2010 and December 2011.

The original dataset contains 541,909 records and eight columns, including:

| Column | Description |
|---|---|
| InvoiceNo | Transaction invoice number |
| StockCode | Product code |
| Description | Product description |
| Quantity | Number of items in the transaction |
| InvoiceDate | Date and time of the transaction |
| UnitPrice | Price per item |
| CustomerID | Customer identifier |
| Country | Customer's country |

### Dataset Setup

The Excel dataset is not included in this repository.

1. Download the dataset from the UCI Machine Learning Repository.
2. Place the downloaded Excel file in the project's `data/` directory.
3. Ensure the filename is `Online Retail.xlsx`.

## Tools and Technologies

- **Python** — Data analysis and processing
- **Pandas** — Data cleaning, grouping, aggregation, and analysis
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Jupyter Notebook** — Interactive analysis
- **Git and GitHub** — Version control and project hosting

## Project Workflow

### 1. Data Exploration
- Inspected dataset dimensions, column names, data types, and summary statistics.
- Examined missing values and duplicate records.
- Investigated unusual quantities and unit prices.

### 2. Data Cleaning
- Removed exact duplicate records from the working dataset.
- Created a revenue column using quantity multiplied by unit price.
- Identified cancellation invoices using invoice numbers beginning with `C`.
- Investigated negative quantities, missing customer identifiers, and zero-price transactions.

### 3. Exploratory Data Analysis
- Analyzed monthly gross sales.
- Ranked product descriptions by gross sales.
- Compared gross sales across countries.
- Examined transaction and customer counts.

### 4. Visualization
Created charts to communicate sales trends, product rankings, and geographical performance.

## Key Findings

- **Monthly trends:** November 2011 recorded the highest monthly value in the initial transaction-level revenue analysis. December 2011 contains incomplete data, ending on December 9.
- **Country performance:** The United Kingdom was the leading country by gross sales in the filtered sales dataset, with approximately £9.00 million recorded.
- **Product performance:** Product descriptions ranked differently depending on their recorded sales value. Postage and manual-charge entries were examined separately from the merchandise-focused ranking.
- **Data quality:** The dataset contains cancellations, negative quantities, zero-price records, missing customer identifiers, and unusual transaction descriptions.
- **Customer analysis:** Missing customer IDs limit the completeness of customer-level comparisons.

## Visualizations

### Monthly Gross Sales

![Monthly Gross Sales](visualization/monthly_gross_sales.png)

### Top 10 Merchandise Descriptions by Gross Sales

![Top 10 Merchandise Descriptions](visualization/top_10_merchandise_by_sales.png)

### Top 10 Countries by Gross Sales

![Top 10 Countries by Gross Sales](visualization/top_10_countries_by_sales.png)

## Project Structure

```text
ecommerce-sales-analysis/
├── data/
│   └── Online Retail.xlsx       # Download separately; not committed
├── notebooks/
│   └── 01_sales_analysis.ipynb
├── visualization/
│   ├── monthly_gross_sales.png
│   ├── top_10_products_by_sales.png
│   ├── top_10_merchandise_by_sales.png
│   └── top_10_countries_by_sales.png
├── .gitignore
├── README.md
└── requirements.txt
```

## How to Run the Project

### Prerequisites

- Python 3.x
- Jupyter Notebook or Visual Studio Code
- The Online Retail Excel dataset

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Ankitha2807/ecommerce-sales-analysis.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ecommerce-sales-analysis
   ```

3. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

4. Download the dataset and place `Online Retail.xlsx` in the `data/` directory.

5. Open `notebooks/01_sales_analysis.ipynb` in Jupyter Notebook or Visual Studio Code and run the cells in order.

## Limitations

- Gross sales are calculated from transactions with positive quantities and positive unit prices, excluding invoices marked as cancellations.
- The gross sales measure is not net revenue or profit. Subsequent returns, refunds, and other adjustments require separate treatment.
- Some non-merchandise charges may remain in the analysis.
- Missing customer IDs limit customer-level analysis.
- December 2011 represents an incomplete month.
- Merchandise filtering excludes selected descriptions, not every possible operational or adjustment entry.

## Future Improvements

- Perform a more detailed analysis of returns, cancellations, and net sales.
- Develop customer segmentation and purchasing-behavior analysis.
- Add an interactive dashboard using Power BI or Plotly.
- Explore sales forecasting using time-series methods.

## Author

**Ankitha K N**

Computer Science and Engineering Graduate

[GitHub Profile](https://github.com/Ankitha2807/)

---

*This project was developed for hands-on practice in Python, data cleaning, exploratory data analysis, and data visualization.*