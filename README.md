# Sales Performance Analysis Dashboard

**SQL Server · Power BI · Excel · Business Intelligence**

This project is based on the AdventureWorks sales database. I used SQL Server to prepare the sales data, Excel to work with the sales budget, and Power BI to create a dashboard for analysing sales performance.

The dashboard brings together sales and budget information so that different aspects of the business can be viewed in one place.

## Project Overview

The project starts with understanding the sales reporting requirements, preparing the required data in SQL Server and then using Power BI to build the dashboard.

The main areas covered in the project are:

- Sales trends over different time periods
- Sales performance by customer and product
- Actual sales compared with budget
- Sales across different geographical locations
- Top-selling products and customers

## Dashboard

- **[View dashboard preview (PDF)](Sales%20Report.pdf)**
- **[Download Power BI report (.pbix)](Sales%20Report.pbix)** – Open the file in Power BI Desktop to explore the dashboard.

> The PDF contains a static preview of the dashboard. To interact with the report, open the PBIX file in Power BI Desktop.

## Technology Stack

| Tool | Usage |
| --- | --- |
| SQL Server / T-SQL | Preparing and cleaning sales data |
| Power BI | Creating the data model and dashboard |
| Excel | Working with sales budget data |
| CSV | Storing the exported SQL tables |
| Word | Business requirements and user stories |

## Repository Contents

| File | Description |
| --- | --- |
| `DIM_Calendar_Clean.sql` | SQL script for preparing calendar data |
| `DIM_Customer_Clean.sql` | SQL script for preparing customer data |
| `DIM_Product_Clean.sql` | SQL script for preparing product data |
| `FACT_InternetSales_Clean.sql` | SQL script for preparing internet sales data |
| `DIM_Calendar_Export.csv` | Exported calendar data |
| `DIM_Customer_Export.csv` | Exported customer data |
| `DIM_Product_Export.csv` | Exported product data |
| `FACT_InternetSales_Export.csv` | Exported internet sales data |
| `Sent Over Data - SalesBudget.xlsx` | Sales budget data |
| `Sales Report.pbix` | Power BI dashboard |
| `Sales Report.pdf` | Dashboard preview |
| `Example Business Request.docx` | Business request document |
| `Business Demand Overview & User Stories.docx` | Project requirements and user stories |

## Project Workflow

1. **Understanding the requirements:** Went through the business request and user stories to understand what information was needed in the sales report.
2. **Data preparation using SQL:** Used SQL Server to prepare the calendar, customer, product and internet sales tables from the AdventureWorks data warehouse.
3. **Exporting the data:** Exported the cleaned tables into CSV files for use in Power BI.
4. **Working with Power BI:** Imported the CSV files and sales budget Excel file, created relationships between the tables and prepared the data model.
5. **Dashboard creation:** Created charts, tables, maps and other visuals to display sales trends, budget comparisons and product and customer performance.

## Getting Started

### View the Dashboard

Open [Sales Report.pdf](Sales%20Report.pdf) to see the dashboard preview.

To explore the report, download [Sales Report.pbix](Sales%20Report.pbix) and open it using Power BI Desktop.

### Run the SQL Scripts

1. Install SQL Server and SQL Server Management Studio.
2. Download the AdventureWorksDW sample database using the [Microsoft AdventureWorks installation guide](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure).
3. Restore the database in SQL Server.
4. Open the four SQL scripts and run them to prepare the required tables. Change database or schema references if needed.
5. Export the query results into CSV files, or use the CSV files already included in the repository.
6. Open the Power BI file and update the data source paths if required.

The original project setup also refers to an [AdventureWorksDW data update script](https://github.com/techtalkcorner/SampleDemoFiles/blob/master/Database/AdventureWorks/Update_AdventureWorksDW_Data.sql). Review the script before running it.

## Project Outcome

The final output is a Power BI dashboard that brings sales and budget data together. It allows users to compare sales with budget and look at performance across products, customers, locations and different time periods.
