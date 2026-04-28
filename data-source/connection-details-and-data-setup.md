# Connection Details and Data Setup

## Overview

This document describes how data was connected, prepared, and modeled in Power BI using the ComputerInventory SQL Server database.

## Data Connectivity Mode

This project uses **Import mode** in Power BI.

### Rationale

- Provides faster performance for dashboard interaction
- Simplifies data modeling and DAX usage
- Suitable for small-to-medium datasets used in this demo environment

### Alternative Approach

In enterprise environments, **DirectQuery** may be used when:
- Real-time or near real-time data is required
- Large datasets cannot be efficiently imported
- Data governance requires queries to run directly against the source system

## Steps

1. In Power BI Desktop, select `Import Data from SQL`.

<img width="693" height="549" alt="image" src="https://github.com/user-attachments/assets/dd82c408-2a6f-4a15-92a8-1124b52fe536" />


2. Select tables and views. Additional tables may be added later, if needed.  Select `Transform Data`.

<img width="875" height="693" alt="image" src="https://github.com/user-attachments/assets/c0e2abbe-8ddd-42a7-a198-cd25b0eba06e" />


3. Clean up and remove columns that have "Table" or "Value" values in the rows.  Only columns with IDs or descriptive field names are kept.

<img width="854" height="572" alt="image" src="https://github.com/user-attachments/assets/7151530d-6921-4326-a6d0-f6372714011a" />


4. Select `Model view` in Power BI Desktop, and validate or modify relationships.  Remove unnecessary tables.  In the example vW_* were removed since raw tables will be used.  the extra view tables would have created confusing duplicate logic.

<img width="1347" height="848" alt="image" src="https://github.com/user-attachments/assets/667283cc-f3af-422c-8c0a-3c010423f39e" />


5.  At this step, we can start creating reports in `Report View`.
