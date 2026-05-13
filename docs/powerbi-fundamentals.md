# Power BI Fundamentals

This document provides a concise overview of core Power BI concepts relevant to this project. It is intended as a quick reference for understanding data modeling, reporting, and visualization principles used in the Computer Inventory dashboard.

## Core Concepts

| Concept | Description |
|--------|------------|
| Power BI | Data visualization and reporting tool |
| Dataset | Collection of data loaded into Power BI |
| Report | Collection of visuals built from a dataset |
| Dashboard | High-level view combining visuals (Power BI Service) |
| Data Model | Relationships between tables |
| Table | Structured data (rows and columns) |
| Column | Field within a table |
| Measure | Calculation using DAX (e.g., COUNT, SUM) |
| DAX | Expression language used for calculations |
| Import Mode | Data loaded into Power BI memory |
| DirectQuery | Queries data directly from source |
| Relationship | Connection between tables (e.g., foreign key) |

## Calculated Columns vs Measures

| Type | Description | Example Use |
|------|------------|------------|
| Calculated Column | Computed row-by-row and stored in the model | Categorizing data (e.g., device age group) |
| Measure | Calculated dynamically based on filters | Aggregations (e.g., total devices, average RAM) |

## Filter Context

Filter context defines how data is filtered when a visual or measure is calculated.

Examples:
- Selecting a slicer (e.g., Office = Vancouver)
- Filtering a visual (e.g., only laptops)
- Applying report/page filters

Measures are evaluated within the current filter context.

## Common Visual Types

| Visual | Use Case |
|--------|---------|
| Card | Display a single KPI (e.g., total devices) |
| Bar/Column Chart | Compare categories (e.g., devices by type) |
| Table | Detailed records |
| Pie/Donut Chart | Proportions (use sparingly) |
| Slicer | Interactive filtering |

## Data Modeling (Star Schema)

A common modeling approach in Power BI:

- Fact tables store measurable data (e.g., Computer, Computer_Software)
- Dimension tables provide descriptive attributes (e.g., Employee, CompType)

Benefits:
- Simplifies reporting
- Improves performance
- Makes relationships easier to manage

## Best Practices

- Keep data models simple and well-structured  
- Use meaningful column and table names  
- Avoid unnecessary columns in the model  
- Prefer measures over calculated columns for aggregations  
- Use star schema where possible  
- Design visuals for clarity, not complexity

## References
- https://learn.microsoft.com/en-us/power-bi/transform-model/
- https://learn.microsoft.com/power-bi/fundamentals/desktop-getting-started  
- https://learn.microsoft.com/en-us/power-bi/transform-model/desktop-modeling-view
- https://learn.microsoft.com/power-bi/transform-model/desktop-quickstart-learn-dax-basics  
- https://learn.microsoft.com/power-bi/visuals/power-bi-visualization-types-for-reports-and-q-and-a  
