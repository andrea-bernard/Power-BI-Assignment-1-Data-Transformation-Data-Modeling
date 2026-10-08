# Power-BI-Assignment-1-Data-Transformation-Data-Modeling
# E-Commerce Sales Analysis – Power BI

## Overview
Data transformation and modeling of e-commerce orders using Power BI.

## Files
- PowerBI_Assignment1.pbix – the report/model
- data/ – List of Orders, Order Details, Sales target CSVs

## Transformations done
- Kept first 500 rows of List of Orders (removed 60 blank rows)
- Converted Order Date to Date; Amount, Profit, Target to Fixed Decimal
- Trimmed text, proper-cased CustomerName, created Location, Profit Margin, Profit Status
- Merged List of Orders + Order Details into Orders Data (1,500 rows)

## Missing and duplicate data
- Missing: 60 fully blank rows, removed. No other nulls.
- Duplicates: none found; removal step kept as a safeguard.

## Data model
- List of Orders (1) → (*) Order Details on Order ID
- Order Details (*) ↔ (*) Sales Target on Category
