# Superstore Sales Analytics | Power BI

A three-page Power BI report for exploring sales performance, product trends, customer segments, and shipping results. The project is stored in the **Power BI Project (PBIP)** format, with the report definition authored using **PBIR** and the semantic model defined in **TMDL**.

## Report preview

### Executive Overview

![Executive Overview report page](Screenshots/Exec%20Overview.png)

### Product Performance

![Product Performance report page](Screenshots/Product%20Performance.png)

### Customer & Shipping Analysis

![Customer and Shipping Analysis report page](Screenshots/Customer%20Analysis.png)

## What’s inside

- **Executive Overview:** sales, profit, margin, order and customer KPIs, with monthly and regional trends.
- **Product Performance:** sub-category rankings, product-level sales and profit comparison, category trends, and product tables.
- **Customer & Shipping Analysis:** customer segment performance, shipping mode results, order value, and shipping time.
- **Semantic model:** a star schema with `FactSales` and date, customer, product, geography, and shipping dimensions.
- **Measures:** sales, profit, margin, order value, customer growth, time intelligence, and shipping measures.
- **Interactive filtering:** slicers vary by report page, including year, region, segment, category, sub-category, and ship mode.

## Project structure

```text
Superstore-PowerBI/
├── Data/
│   └── Superstore.csv
├── Screenshots/
├── Superstore.Report/          # PBIR report definition and theme resources
├── Superstore.SemanticModel/   # TMDL semantic model
└── Superstore.pbip             # Open this file in Power BI Desktop
```

## Open the project

1. Clone or download this repository.
2. Open `Superstore.pbip` in Power BI Desktop.
3. Before refreshing, update the `SourceFilePath` parameter in `Superstore.SemanticModel/definition/expressions.tmdl` to the full path of `Data/Superstore.csv` on your computer.
4. Refresh the model when prompted.

The source path is currently configured for the original development machine, so updating it is required on another computer.

## Tools and formats

- Microsoft Power BI Desktop
- PBIP project format
- PBIR report definition
- TMDL semantic model
- Power Query (M) and DAX

## Data

The report uses the Superstore sample sales dataset included at `Data/Superstore.csv`.
