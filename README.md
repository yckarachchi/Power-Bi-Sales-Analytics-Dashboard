📊 Power BI Sales Analytics Dashboard
Project Overview

A comprehensive business intelligence solution built in Power BI for analyzing sales performance across multiple dimensions including countries, products, sales teams, and time periods. This project demonstrates end-to-end BI development from raw data to interactive dashboards.

📈 Key Measures (DAX)

SumOfSales - Total sales amount

AVG_Sales - Average sale value

AVG_Sale_Per_Order - Revenue per order

SalesCount - Number of orders

NoOfSalesPersons - Distinct salespeople count

MaximumSale - Highest individual sale

Total_Team1_Sales_India - Filtered measure example

🔧 Technical Implementation
Data Transformation (Power Query/M)

Sales.csv: Conditional product categorization, data type conversion

Countries.csv: Header promotion, text formatting

SalesPerson.csv: Multi-column processing, team leader assignment

ProductDetails.csv: Dynamic category mapping, column restructuring

Advanced Features

Dynamic Date Table

Auto-generates calendar based on Sales data range

Complete date hierarchy for time intelligence

Template-based structure for reusability

Conditional Business Logic

dax

TopSales = IF(Sales[Sales] > 500, "Top Sale", "Normal Sale")

IndiaTopSalesColumn = IF(AND(Sales[Sales] > 300, Sales[Country] = "India"), "India Top Sales", "Others")

Relationship Management

4 active relationships between fact and dimension tables

Date relationship with joinOnDateBehavior: datePartOnly

Auto-detected and manual relationship configuration

📊 Business Insights Capabilities

Analytical Dimensions

Geographic Analysis: Country → Continent drill-down

Temporal Analysis: Year → Quarter → Month → Day hierarchy

Product Analysis: Category performance with cost integration

Team Analysis: Salesperson → Team → Team Leader structure

Key Performance Indicators

Regional sales performance

Product profitability (Sales vs. Cost)

Team effectiveness metrics

Time-based trend analysis

High-value transaction identification

🚀 Getting Started

Prerequisites

Power BI Desktop (Version 2.144.1378.0 or compatible)

Sample data files (CSV format)

Basic understanding of DAX and Power Query

Data Files Required

Sales.csv - Transaction data

Countries.csv - Geographic mapping

SalesPerson.csv - Team structure

ProductDetails.csv - Product catalog

Setup Instructions

Clone/download the .pbix file

Update file paths in Power Query editor if needed

Refresh data connections

Explore pre-built dashboards and measures

💡 Learning Outcomes

This project demonstrates proficiency in:

Data Modeling: Star schema design and implementation

DAX: Measure creation, time intelligence, conditional logic

Power Query: ETL processes, data transformation

Visualization: Dashboard design and user experience

BI Best Practices: Performance optimization, data categorization
