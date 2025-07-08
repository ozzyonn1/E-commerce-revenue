# E-commerce Revenue Dashboard – SQL + Power BI

## Project Overview

This project showcases an end-to-end workflow of a data analyst: data transformation in SQL, export of analytical tables, and development of a Power BI dashboard for business reporting. The analysis is based on a synthetic e-commerce dataset and covers metrics related to revenue trends, regional performance, product categories, and campaign ROI.

---

## Files Included

- `synthetic_ecommerce_data.csv` – source data for analysis
- `queries/` – all SQL scripts used for data transformation (cohort, ROI, RFM, etc.)
- `data/` – output CSVs ready for Power BI import
- `e_commerce_project.pbix` – interactive dashboard (Power BI Desktop)
- `ecommerce_project` – optional SQLite database

## Dashboard Export (PDF)

For convenience, a static version of the Power BI dashboard is also available in PDF format.

- `e_commerce_project_pb.pdf` – full dashboard exported from Power BI
---

## SQL Transformation Layer

All data was transformed using SQL queries executed in DBeaver and exported as `.csv` files. Each query targets a specific business need.

### 1. Cohort Analysis
- File: `queries/cohort_analysis.sql`
- Purpose: Groups users into cohorts by first purchase month, calculates active customers and total revenue over time.
- Output used in: `cohort_data.csv`

### 2. Revenue by Region & Category
- File: `queries/revenue_by_region_and_category.sql`
- Purpose: Aggregates revenue by region and product category.

### 3. Category Rank by Region
- File: `queries/category_rank_by_region.sql`
- Purpose: Ranks product categories within each region based on total revenue.

### 4. Campaign ROI
- File: `queries/campaign_roi.sql`
- Purpose: Calculates total ad spend, total revenue, and ROI.

### 5. Discount Impact
- File: `queries/discount_impact.sql`
- Purpose: Measures how discounts influence transaction volume and revenue.

### 6. RFM Segmentation
- File: `queries/rfm_analysis.sql`
- Purpose: Identifies top customers based on Recency, Frequency, and Monetary value.

---

## Power BI Dashboard

The dashboard was developed in Power BI Desktop based on the pre-aggregated CSV files exported from SQL. Its layout and structure are designed to support a high-level overview of the e-commerce business.

### KPIs

The top of the dashboard includes key performance indicators:

- **Active Users** – based on cohort activity
- **Total Ad Spend** – calculated from campaign ROI data
- **Total Revenue** – overall revenue from all transactions
- **Earliest ROI Date** – first campaign month with positive ROI

### Visualizations

The dashboard contains the following visual blocks:
![image](https://github.com/user-attachments/assets/57233a49-4b7a-48d5-b521-1bfa09c1e057)


- **Monthly Revenue Dynamics**  
  A line chart showing revenue trends by cohort month.

- **Revenue by Category**  
  A bar chart comparing total revenue across the top product categories.

- **Revenue by Region**  
  Displayed as both a bar chart and a donut chart for better visual clarity.

### Design and Layout

- Clean grid structure with proper visual spacing
- White background with minimal distractions
- Emphasis on clarity, not decoration

### Export

The dashboard is available both as a `.pbix` file and a static `.pdf` export for quick preview.

---

## Author
Oleh Zemlianyi
oleh.zemlianyi@gmail.com



