# DEX Depot - Power BI Sales Analytics Project

## Project Overview

This project focuses on building a complete sales analytics solution in Power BI using a Star Schema data model. The report was designed to analyze sales performance, customer behavior, product trends, returns, and regional performance through interactive visualizations and DAX calculations.

The project demonstrates data modeling, relationship management, calculated columns, measures, time intelligence functions, and advanced DAX concepts commonly used in real-world business reporting.

---

# Project Objectives

The main objectives of this project were:

- Design a Star Schema data model.
- Create relationships between fact and dimension tables.
- Develop calculated columns and measures.
- Implement business KPIs.
- Perform time-based sales analysis.
- Analyze product, customer, and regional performance.
- Create dynamic categorization using DAX.
- Use iterator functions for advanced calculations.
- Build an interactive dashboard for decision-making.

---

# Dataset Structure

The project contains the following tables:

### Fact Tables

| Table Name | Description |
|------------|-------------|
| Sales_Fact | Stores all sales transactions |
| Returns_Fact | Stores returned order information |

### Dimension Tables

| Table Name | Description |
|------------|-------------|
| Customer_Dim | Customer information |
| Product_Dim | Product information |
| Date_Dim | Calendar and date details |
| Region_Dim | Region information |

---

# Data Modeling

A Star Schema model was implemented to improve performance and simplify reporting.

## Primary Key

A Primary Key uniquely identifies each record within a table.

Examples:

- CustomerID in Customer_Dim
- ProductID in Product_Dim
- RegionID in Region_Dim
- Date in Date_Dim
- SalesID in Sales_Fact

### Characteristics

- Unique for every record
- Cannot contain duplicate values
- Used to identify rows uniquely

---

## Foreign Key

A Foreign Key is a column used to create relationships between tables.

Examples:

- CustomerID in Sales_Fact
- ProductID in Sales_Fact
- RegionID in Sales_Fact
- Date in Sales_Fact
- SalesID in Returns_Fact

### Characteristics

- Can contain duplicate values
- References a Primary Key from another table
- Establishes table relationships

---

# Relationships Implemented

The following relationships were created:

| From Table | To Table |
|------------|----------|
| Sales_Fact → Customer_Dim |
| Sales_Fact → Product_Dim |
| Sales_Fact → Date_Dim |
| Sales_Fact → Region_Dim |
| Returns_Fact → Sales_Fact |

Relationship Type:

```text
One-to-Many (1:*)
```

Cross Filter Direction:

```text
Single Direction
```

---

# Tasks Completed

## Calculated Columns

The following calculated columns were created:

- Full Customer Name
- Return Status
- Customer Age Group

These columns help improve data readability and support business analysis.

---

## Measures

Several measures were created to calculate important business metrics, including:

- Total Sales
- Total Cost
- Total Profit
- Return Rate

These measures are used throughout the report to evaluate business performance.

---

## Quick Measures

Quick Measures were implemented to simplify common calculations such as:

- Sales Count
- Average Sales

---

## Dedicated Measure Table

A dedicated measure table was created to store all DAX measures in a single location.

Benefits:

- Improved organization
- Easier maintenance
- Cleaner data model
- Better development practices

---

## Filter Context and Context Transition

Advanced DAX concepts were implemented to analyze:

- Sales by Region
- Sales by Product Category
- Recent Sales Performance

This enables dynamic filtering and interactive reporting.

---

## Time Intelligence Analysis

Time Intelligence functions were used to perform period-over-period analysis.

Implemented analyses include:

- Year-to-Date (YTD) Sales
- Previous Year Sales Comparison
- Running Total Sales

These calculations help identify trends and growth patterns across months and years.

---

## Additional Business Scenarios

### Sales Categorization

Sales values were categorized into:

- Low
- Medium
- High

This allows easier segmentation of business performance.

# Dashboard Features

The report includes interactive dashboard elements such as:

### KPI Cards

- Total Sales
- Total Cost
- Total Profit
- Return Rate

### Slicers

- Region
- Product Category
- Year

# Business Insights Generated

The dashboard enables users to:

- Monitor sales performance over time.
- Compare current and previous year sales.
- Identify high-performing products.
- Analyze regional sales trends.
- Track returned orders.
- Measure profitability.
- Evaluate customer segments.

---

# Skills Demonstrated

Through this project, the following Power BI skills were applied:

- Data Modeling
- Star Schema Design
- Primary Key & Foreign Key Relationships
- DAX Measures
- Calculated Columns
- Quick Measures
- Context Transition
- Time Intelligence
- Iterator Functions
- Dashboard Development
- Business Intelligence Reporting

---
