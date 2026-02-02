# Blinkit Revenue and Inventory insights - Power BI Dashboard

## Project Overview
This project involves a comprehensive analysis of Blinkit's sales performance, customer satisfaction, and inventory distribution. Using Power BI, I transformed raw data into an interactive dashboard to identify key insights into sales trends based on outlet location, item type, and outlet size.

The goal was to provide a 360-degree view of the business to support data-driven decision-making for inventory management and sales strategies.

## Key Performance Indicators (KPIs)
The dashboard tracks the following core metrics to assess overall performance:
* **Total Sales:** $1.20M (Revenue generated)
* **Average Sales:** $141 (Average revenue per transaction)
* **Number of Items:** 9K (Total unique items/SKUs sold)
* **Average Rating:** 3.9 (Customer satisfaction score)

## Charts & Visualizations Created
1.  **Total Sales by Fat Content (Donut Chart):**
    * Analyzed the impact of fat content on sales, revealing the revenue distribution between "Low Fat" and "Regular" items.
2.  **Total Sales by Item Type (Bar Chart):**
    * Identified top-performing categories (e.g., Fruits & Vegetables, Snack Foods) to assist in inventory planning.
3.  **Outlet Establishment Trend (Line Chart):**
    * Visualized the growth of outlet establishment and sales trends over the years to assess business expansion.
4.  **Sales by Outlet Size (Donut Chart):**
    * Segmented sales by High, Medium, and Small outlet sizes to understand the correlation between store size and revenue.
5.  **Sales by Outlet Location (Funnel/Bar Chart):**
    * Compared performance across Tier 1, Tier 2, and Tier 3 cities to pinpoint regional market leaders.
6.  **Outlet Type Metrics (Matrix Table):**
    * A detailed breakdown of sales, number of items, and ratings for different store types (Grocery Store vs. Supermarket Types).

## Process & Workflow
### 1. Data Cleaning & ETL (Extract, Transform, Load)
* Imported raw data (Excel/CSV) into Power BI.
* Handling missing values in columns like `Item Weight` and `Outlet Size`.
* Standardized categorical values (e.g., merging "LF", "low fat" -> "Low Fat").

### 2. Data Modeling & Analysis
* Established relationships between tables (if applicable).
* Created calculated columns for customized segmentation.

### 3. DAX (Data Analysis Expressions) Implementation
* Used DAX functions to calculate custom measures:
    * `Total Sales = SUM(Blinkit_Data[Sales])`
    * `Avg Sales = AVERAGE(Blinkit_Data[Sales])`
    * `No of Items = COUNTROWS(Blinkit_Data)`
    * `Avg Rating = AVERAGE(Blinkit_Data[Rating])`

### 4. Dashboard Design
* Implemented a user-friendly interface with dynamic slicers for **Outlet Location Type**, **Outlet Size**, and **Item Type**.
* Used a consistent color theme (Blinkit Yellow) for brand alignment.
* Added navigation buttons and clear metric cards for high-level visibility.

## Key Business Insights
* **Tier 3 locations** show strong potential in total sales, suggesting a high demand in emerging markets.
* **"Regular" fat content** items generate higher revenue compared to low-fat options.
* **Supermarket Type 1** outlets are the dominant revenue drivers compared to grocery stores.
* Sales performance is relatively consistent across **High** and **Medium** sized outlets, but optimization is needed for smaller outlets.

## Tech Stack
* **Tool:** Microsoft Power BI Desktop
* **Language:** DAX (Data Analysis Expressions)
* **Data Source:** Excel File
