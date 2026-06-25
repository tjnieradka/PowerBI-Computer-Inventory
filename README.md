# PowerBI-Computer-Inventory

Power BI dashboards built from a SQL Server inventory database demonstrating data modeling, data transformation, reporting, and visualization for asset and operational analysis.

---

## Overview

This project demonstrates how raw relational data from a SQL Server database can be transformed into meaningful insights using Power BI.

It builds on the companion project:

[SQL-Computer-Inventory](https://github.com/tjnieradka/SQL-Computer-Inventory)

### Key Goals

- Connect Power BI to a SQL Server database  
- Transform and model data for reporting  
- Create interactive dashboards  
- Demonstrate practical data analysis scenarios  

---

## Technology Stack

- Power BI Desktop  
- Microsoft SQL Server Express 2022  
- SQL Server Management Studio (SSMS)  
- T-SQL  
- Windows 11  
- GitHub (documentation)  

---
## Planned Repository Structure (To be refined)
<PRE>
PowerBI-Computer-Inventory/
│
├── README.md
│
├── data-source/
│   └── connection-details-and data-setup.md   
├── docs/
│   ├── powerbi-fundamentals.md
│   ├── data-modeling.md
│   ├── report-design.md
│   └── step-by-step-guide.md (TBA)
│
├── pbix/
│   └── computer-inventory.pbix
│
├── queries/
│   └── data-extraction.sql (TBA)
│
└── output/
    ├── dashboard-screenshots/
    │   └── 00-dashboard-overview.png
    │   └── 01a-computer-inventory-overview.png
    │   └── ...(additional screenshots)
    └── setup-screenshots/
        └── connection-setup.png
        └── navigator-setup.png
        └── query-editor.png    
        └── ...(additional screenshots)    
</PRE>

## Data Source

The dataset comes from a locally hosted SQL Server database:

- Database: `ComputerInventory`  
- Source: SQL Server Express  
- Connection: Import

### Tables Used 

- Computer
- CompStatus
- CompType
- Computer_Software  
- Employee  
- EmpOffice
- EmpPosition
- EmpStatus
- Vendor 
- Software  
- SwStatus
- SwLibcns
- SwLanguage 

---

## Connecting Power BI to SQL Server

### Steps

1. Open Power BI Desktop  
2. Click **Get Data → SQL Server**  
3. Enter:
   - Server: `localhost`  
   - Database: `ComputerInventory`  
4. Choose:
   - Import 
5. Select relevant tables or views  
6. Load data into Power BI  

---

## Data Modeling

### Key Relationships

- Computer → Employee  
- Computer → Computer_Software → Software  

### Concepts Demonstrated

- Fact vs Dimension tables  
- One-to-many relationships  
- Star schema (simplified)  

---

## Dashboard Features

### Example Reports

- Computer Inventory Overview
- Computer Inventory Overview by Office
- Overview of Employees by Office
- Software Inventory Overview
- Employee Device and Software Assignment 

---

## Sample Insights

- Identify computers not assigned to any user  
- Track software installations across devices  
- Analyze distribution of assets by type or office 
- Detect outdated or inactive systems  

---

## Step-by-Step Report Creation (TBA)

See: `docs/step-by-step-guide.md`

### Includes

- Creating visuals  
- Using slicers and filters  
- Building charts and tables  
- Basic DAX measures  

---

## Power BI Fundamentals (Quick Reference)

See: `docs/powerbi-fundamentals.md`

### Covers

- Data model concepts  
- Measures vs calculated columns  
- Import vs DirectQuery  
- Visual design best practices  
---

## Output

Screenshots available in:  
`output/dashboard-screenshots/`

---

## Future Enhancements

- Add DAX measures (e.g., device utilization)  
- Add time-based analysis  
- Improve dashboard design and UX  

---

## About This Project

This project demonstrates practical Power BI skills applied to a realistic IT asset management scenario, building on prior experience with SQL reporting, SAP analytics tools, and data analysis workflows.
