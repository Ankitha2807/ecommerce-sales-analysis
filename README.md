# E-Commerce Sales & Customer Analytics

## Project Overview

An exploratory data analysis project using Python to investigate online retail transactions, sales trends, product performance, and geographical revenue distribution.

The project demonstrates data cleaning, exploratory data analysis (EDA), aggregation, and visualization using real-world retail data.

## Objectives

- Analyze monthly revenue trends.
- Identify top-performing products by revenue and quantity.
- Compare sales performance across countries.
- Investigate missing values, duplicate records, returns, and unusual prices.
- Communicate findings through visualizations and business insights.

## Dataset

**Source:** [UCI Machine Learning Repository — Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail)

The dataset contains transaction-level records from a UK-based online retailer covering December 2010 to December 2011.

The original dataset contains 541,909 rows and includes invoice numbers, product codes, descriptions, quantities, invoice dates, unit prices, customer IDs, and countries.

Download the dataset from the official source and place `Online Retail.xlsx` inside the `data/` directory.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Git and GitHub

## Project Structure

```text
ecommerce-sales-analysis/
├── data/
│   └── Online Retail.xlsx
├── notebooks/
│   └── 01_sales_analysis.ipynb
├── visualization/
├── README.md
└── requirements.txt
```

## Analysis Performed

### Data Quality Assessment
- Identified missing product descriptions and customer IDs.
- Detected exact duplicate rows.
- Investigated negative quantities and unusual unit prices.
- Examined the implications of incomplete customer information.

### Sales Analysis
- Aggregated transaction revenue by month.
- Compared products by recorded revenue and net quantity.
- Analyzed revenue, quantity, and identifiable customer counts by country.
- Created visualizations to communicate findings.

## Preliminary Findings

- November 2011 recorded the highest monthly revenue in the current analysis.
- The United Kingdom is the leading country by recorded revenue.
- Product rankings differ depending on whether revenue or quantity is used.
- Missing customer IDs do not necessarily make a transaction unusable for overall sales analysis.

These findings are preliminary and will be refined after final validation of returns, cancellations, and unusual transactions.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from the official UCI source.
4. Place `Online Retail.xlsx` in the `data/` directory.
5. Open `notebooks/01_sales_analysis.ipynb` in VS Code or Jupyter.
6. Run the notebook cells in order.

## Future Improvements

- Refine the definition of revenue and validate return/cancellation handling.
- Investigate customer purchasing patterns.
- Add further visualizations and business recommendations.
- Improve the notebook's reproducibility and presentation.

## Author

Ankitha K N