## Demand & Supply KPI Analysis Dashboard
 Power BI | MS SQL Server | MySQL

### Demand & Supply KPI Analysis: Performance, Profit & Loss Dashboard

An interactive Power BI dashboard developed to analyze demand, availability, supply shortages, profit, and loss using relational databases (Microsoft SQL Server and MySQL) as data sources, with dynamic KPI tracking and environment migration handling.

### Purpose

This project focuses on analyzing demand and supply data to monitor operational performance and financial impact. The dashboard enables users to track daily demand and availability, identify supply shortages, and evaluate profit and loss metrics through KPIs and filters.

The project also demonstrates real-world scenarios such as:

Switching between test and production environments

Migrating data sources from SQL Server to MySQL without rebuilding reports

### Tech Stack

The dashboard was built using the following tools and technologies:

• Power BI Desktop – Dashboard creation, KPI visualization, and reporting

• Microsoft SQL Server – Primary data source (test & production environments)

• MySQL – Secondary data source for data source migration

• SQL – Data validation, joins, and transformation logic

• DAX (Data Analysis Expressions) – KPI and calculated measures

• Power Query – Data cleaning, source switching, and transformation

• File Format – .pbix

### Data Source

Source: Demand & Supply transactional dataset

Initial data loaded into SQL Server (Test Environment – ~99 records)

Updated data loaded into SQL Server (Production Environment – ~1,043 records)

Same dataset later migrated into MySQL database

The project demonstrates how real-world data volume and values can differ between environments.

### Features / Highlights
#### • Business Problem

Operations teams need to continuously monitor:

Daily demand vs availability

Supply shortages

Profit and loss impact

Additionally, real-world projects often require:

Environment changes (test → production)

Data source migrations (SQL Server → MySQL)

Rebuilding dashboards every time is inefficient.

#### • Goal of the Dashboard

Track demand and supply KPIs in real time

Analyze profit and loss trends

Enable filtering by date and product

Demonstrate seamless report migration across environments and databases

#### • Data Preparation & Transformation

Loaded data into SQL Server

Performed data checks:

Distinct value validation for all columns

Null value checks and cleaning

Applied LEFT JOIN to combine demand and availability tables

Imported cleaned data into Power BI

Created a separate measures table using Enter Data

Built all KPIs using DAX measures

#### • KPI Pages Overview
#### Page 1: Demand & Supply KPIs

Average Demand per Day

Average Availability per Day

Total Supply Shortage

#### Page 2: Financial KPIs

Total Profit

Total Loss

Average Daily Loss

#### • Filters & Interactivity

Date filter

Product filter

Interactive visuals for dynamic analysis

#### • Environment Switching (Test → Production)

Initial report connected to Test Environment (99 records)

Production data loaded into a new SQL Server database (1,043 records)

Data source updated in Power BI using:

Data Source Settings

Power Query Editor

Report updated automatically without recreating visuals or measures

#### • Data Source Migration (SQL Server → MySQL)

A real-world scenario where the client changed the database:

Installed MySQL Connector/NET

Imported production data into MySQL using MySQL Workbench

Connected Power BI to MySQL database

Updated Power Query source code to replace SQL Server connection

Dashboard updated successfully without rebuilding KPIs or visuals

#### • Business Impact & Insights

Enables monitoring of operational demand and shortages

Highlights profit and loss trends for decision-making

Demonstrates scalable BI solutions adaptable to data source changes

Reflects real-world enterprise reporting workflows

### 6. Screenshots

#### Page 1: Demand & Supply KPIs

![Page 1 – Demand & Supply KPIs](https://github.com/DDakave/Demand-Supply-KPI-Dashboard/blob/main/Demand%20%26%20Supply%20KPI.png)

#### Page 2: Financial KPIs

![Page 2 – Profit & Loss KPIs](https://github.com/DDakave/Demand-Supply-KPI-Dashboard/blob/main/Financial%20KPIs.png)
