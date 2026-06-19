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

## Configuration

In Power BI Desktop, select `Import Data from SQL`.




