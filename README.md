# Sales Performance Analysis Dashboard

**SQL Server · Power BI · Excel · Business Intelligence**

A sales analytics project built around the **AdventureWorks data warehouse**. It uses SQL to prepare sales-related tables, combines sales and budget data in Power BI, and presents interactive reporting to support sales performance analysis.

## Project Overview

The project follows a business-intelligence workflow: understand the business request, prepare dimension and fact data in SQL Server, export cleaned tables, build a Power BI data model, and design a sales dashboard.

**Key analysis areas**
- Sales trends over time
- Customer and product performance
- Sales versus budget
- Geographic sales patterns
- Top-performing products and customers

These describe the dashboard's intended analytical scope; no unverified revenue or performance improvement claims are made.

## Dashboard

- **[View dashboard preview (PDF)](Sales%20Report.pdf)**
- **[Download Power BI report (.pbix)](Sales%20Report.pbix)** — open in Power BI Desktop for interactive exploration.

> GitHub cannot display a Power BI `.pbix` dashboard interactively. The PDF provides a static report preview.

## Technology Stack

| Tool | Role |
| --- | --- |
| SQL Server / T-SQL | Clean and transform AdventureWorks warehouse tables |
| Power BI | Data modeling, calculations and dashboard visualizations |
| Excel | Sales budget input |
| CSV | Cleaned data exports used for analysis |
| Word | Business request, demand overview and user stories |

## Repository Contents

| File | Purpose |
| --- | --- |
| `DIM_Calendar_Clean.sql` | Prepare the calendar dimension |
| `DIM_Customer_Clean.sql` | Prepare customer attributes |
| `DIM_Product_Clean.sql` | Prepare product attributes |
| `FACT_InternetSales_Clean.sql` | Prepare internet sales facts |
| `DIM_Calendar_Export.csv` | Exported calendar data |
| `DIM_Customer_Export.csv` | Exported customer data |
| `DIM_Product_Export.csv` | Exported product data |
| `FACT_InternetSales_Export.csv` | Exported internet sales data |
| `Sent Over Data - SalesBudget.xlsx` | Sales budget spreadsheet |
| `Sales Report.pbix` | Power BI report |
| `Sales Report.pdf` | Static dashboard preview |
| `Example Business Request.docx` | Example stakeholder request |
| `Business Demand Overview & User Stories.docx` | Requirements and user stories |

## Workflow

1. **Define the business problem:** Review the business request and user stories to identify reporting needs.
2. **Prepare data in SQL Server:** Use the four `*_Clean.sql` scripts to select and transform calendar, customer, product and internet sales data from the AdventureWorks warehouse.
3. **Export the cleaned tables:** Use the four included `*_Export.csv` datasets as the prepared reporting inputs.
4. **Build the data model:** Load the sales tables and the Excel budget into Power BI, connect relevant fact and dimension tables, and create calculations.
5. **Design the dashboard:** Explore trends and breakdowns with charts, maps, tables and customer/product-level views.

## Getting Started

### View the finished dashboard
Open [Sales Report.pdf](Sales%20Report.pdf) for a quick preview, or download [Sales Report.pbix](Sales%20Report.pbix) and open it in **Power BI Desktop**.

### Recreate the data preparation
1. Install **SQL Server** and **SQL Server Management Studio**.
2. Download and restore a compatible **AdventureWorksDW** sample database using the [Microsoft AdventureWorks installation guide](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure).
3. Review the four SQL scripts and adjust database names or schema references if needed before executing them.
4. Export the prepared results, or use the included CSV exports.
5. Open the Power BI report and update any local file paths or data-source settings as required.

The source project's setup instructions also reference an [AdventureWorksDW data-update script](https://github.com/techtalkcorner/SampleDemoFiles/blob/master/Database/AdventureWorks/Update_AdventureWorksDW_Data.sql). Review scripts before running them on your database.

## Business Value

The dashboard provides a consolidated view for exploring sales results against budget and drilling into customers, products and time periods. It is a demonstration analytics project, not evidence of an actual business deployment or measured commercial impact.

## Attribution

This repository is based on an existing Sales Analysis SQL/Power BI project. The supplied original README linked to [Mahijain1201/SalesAnalysis](https://github.com/Mahijain1201/SalesAnalysis). That reference is retained here to acknowledge the source; any independent modifications or contributions should be documented separately.
