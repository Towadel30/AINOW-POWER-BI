# AINOW-POWER-BI


# Electronic Sales Performance Dashboard (AI NOW Bootcamp)

## Project Overview

This project is a comprehensive Sales and Profitability analysis using an **Electronic Sales Dataset**. The goal was to transform raw data into actionable business insights using **Power BI**, focusing on Time Intelligence and Dimensional Analysis.

## Data Interpretation & Key Insights

Based on the final dashboard visuals, the following business insights were derived:

* 
**Financial Health**: Total Sales reached **$56.24M** with a healthy **Total Profit of $32.44M**.


* 
**Profitability**: The business maintains a strong **Profit Margin of 58%**, indicating efficient cost management relative to sales.


* 
**Channel Performance**: The **Store** channel is the primary driver of revenue, accounting for **57.24%** ($32.19M) of total sales.


* 
**Product Leadership**: The **Computers** and **Cameras/Camcorders** categories dominate the market share, as seen in the treemap analysis.


* 
**Regional Footprint**: Sales are widely distributed across **Nigeria**, with significant clusters in major urban centers.


* 
**Growth Trends**: While the **Sales YOY % is 39.75%** (when viewing all dates), specific monthly analysis shows sales peaking near **$6M** in months like November.



## Technical Implementation

The project was completed in four distinct phases:

### 1. ETL (Extract, Transform, Load)

* Cleaned raw data by removing unnecessary header rows (top 6 rows).
* Corrected data types for `Order Date` (Date) and `Sales` (Fixed Decimal).
* Handled "Unknown" channel values to ensure clean visualization.



### 2. Data Modeling

* Created a dedicated **Date Table** using DAX.
* Established a **1-to-Many relationship** between the `DateTable` and the `Sales` table to enable Time Intelligence.



### 3. DAX Measures

Created a "Key Measures" table including:

* **Sales YTD/QTD**: For tracking year-to-date and quarter-to-date performance.
* **Same Period Last Year (SPLY)**: To compare current performance against historical data.
* 
**Sales YOY %**: Calculated as `DIVIDE([Sales YOY], [Sales SPLY], 0)`.


* 
**Profit Margin**: Calculated as `DIVIDE([Total Profit], [Total Sales])`.



### 4. Visualizations

* 
**KPI Cards**: For immediate oversight of Sales, Profit, and Margin.


* 
**Donut Chart**: Analysis by Channel.


* 
**Treemap**: Analysis by Product Category.


* 
**Map Visual**: Geographic distribution by State/Zone.


* 
**Line & Column Chart**: Monthly trend analysis of Sales vs. Profit Margin.





