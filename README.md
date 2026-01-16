# powerbi-sales-kpi-dashboard
Power BI practice dashboard with KPIs and slicers
# Power BI Sales KPI Dashboard (Practice Project)

This is a simple Power BI dashboard built as a practice project to demonstrate core BI skills: loading structured data from Excel, building a basic model, creating KPI measures, and presenting results in an interactive dashboard.

## What this dashboard shows
- **Total Sales**
- **Products Sold**
- **Customer Count**
- Products sold split by **Gender**
- Products sold by **Country**
- A slicer to filter by **Product Color**

## Dashboard preview
[![Dashboard Preview](images/dashboard-preview.png)
](https://github.com/shehabseif/powerbi-sales-kpi-dashboard/blob/main/Task%20Visual.JPG)

## Data source
The project uses an Excel file that contains one fact table and multiple dimension tables:

**Fact table**
- `fact_InternetSales`

**Dimension tables**
- `dim_Product`
- `dim_Customer`
- `dim_SalesTerritory`
- `dim_Currency`

## Data model (high-level)
The model follows a standard star-style structure:
- `fact_InternetSales` links to dimensions using keys like `ProductKey`, `CustomerKey`, `SalesTerritoryKey`, and `CurrencyKey`.

## Measures (KPIs)
This report includes KPI measures used in the card visuals:
- `TotalSales`
- `ProductsSold`
- `Customers`

## Main visuals and interactions
- **KPI Cards**: Total Sales / Products Sold / Customers
- **Donut chart**: Products Sold by Gender
- **Bar chart**: Products Sold by SalesTerritoryCountry
- **Slicer**: Product Color

## Tools used
- Power BI (PBIX)
- DAX measures (basic KPI measures)
- Excel (source dataset)

## How to open the project
1. Download or clone the repository.
2. Open the PBIX file: `dashboard/Task_5_Submission.pbix`
3. If Power BI asks for the data source, point it to:
   `data/8_1_section-five-data-extract.xlsx`

## Notes (for recruiters)
This is a practice project designed to demonstrate dashboard building fundamentals:
- data loading + basic modeling
- KPI creation
- clean, readable dashboard layout
- slicers and interactive visuals
