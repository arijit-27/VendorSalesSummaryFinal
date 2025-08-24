# Vendor Sales Insights Dashboard
# End-to-End Data Analysis Project

## Project Overview

This project is an end-to-end data analysis workflow that involves handling multiple large datasets, building a database, extracting key insights through SQL and Python, and presenting findings through interactive visualization and reports.

## Data Sources

The project starts by working with six major datasets, which are quite large:

- **Begin_inventory**: shape (206,529, 9)  
- **End_inventory**: shape (224,489, 9)  
- **Vendor_invoice**: shape (5,543, 10)  
- **Purchase_prices**: shape (12,261, 9)  
- **Sales**: shape (12,372,474, 16) — this dataset contains over 13 million records and requires special handling due to its size  

## Workflow

1. **Database Creation**  
   Using the Google Colab environment, a SQLite database is created to efficiently store and process the multiple large datasets.

2. **Handling Large Sales Data**  
   Given the massive size of the Sales dataset (over 13 million rows), it is ingested in chunks of 5,000,000 rows to avoid exhausting RAM and to prevent timeout errors during processing.

3. **Data Exploration and SQL Querying**  
   The initial step involves understanding the key parameters in each table relevant to the analysis. Through carefully crafted SQL queries, a desired summary table is created with the following columns:  
   - VendorNumber  
   - VendorName  
   - Brand  
   - Description  
   - PurchasePrice  
   - ActualPrice  
   - Volume  
   - TotalPurchaseQuantity  
   - TotalPurchaseDollars  
   - TotalSalesQuantity  
   - TotalSalesDollars  
   - TotalSalesPrice  
   - TotalExciseTax  
   - FreightCost  

4. **Exploratory Data Analysis (EDA)**  
   Utilizing Python libraries such as Matplotlib, Seaborn, and Pandas, extensive exploratory data analysis is performed on the resulting dataset to uncover patterns, trends, and anomalies.

5. **Statistical Analysis**  
   Hypothesis testing and confidence interval calculations are executed to validate insights and support data-driven conclusions.

6. **Visualization and Reporting**  
   The analysis culminates with the creation of a Power BI dashboard that visualizes key metrics and trends interactively. A comprehensive report summarizes all findings.

## Technologies Used

- SQLite (via Google Colab)  
- Python (Pandas, Matplotlib, Seaborn)  
- Power BI  
- SQL  

## Project Outcome

This project demonstrates the ability to integrate multiple massive data sources, build a relational database, perform complex data manipulations on large datasets with memory-efficient chunk processing, and deliver actionable insights through statistical analysis and interactive visualizations. It provides a full-cycle example of real-world data analysis from raw data to business intelligence reporting.

---

Feel free to explore the notebook and dashboards to understand the detailed steps and insights.

