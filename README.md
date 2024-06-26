# Business Insights 360

Welcome to the **Business Insights 360** project repository. This project demonstrates comprehensive data analysis and visualization using Power BI. It covers various aspects of data handling, from extraction and transformation to visualization and reporting, leveraging the robust capabilities of Power BI.

## Project Overview

AtliQ Hardware is growing rapidly in recent years and has decided to implement data analytics using Power BI for the first time to surpass their competitors in the market and make data-driven decisions. This project aims to provide answers to stakeholders' questions in terms of all aspects like finance, sales, marketing, and supply chain.

I worked on this project by following the Codebasics Power BI Course. [Link to the course](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiZTI2Nzk4M2ItOWMyNC00MmVjLTk4MjYtMjI3YmVjMjMxNzRhIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=1520a3d763bc46ea945e) 

## Tech Stacks

- **Power BI Desktop**
- **Excel**
- **DAX language**
- **Power Query**
- **SQL**
- **DAX Studio** (for optimizing the report)
- **Project Charter**

## Project Charter File

### Power BI Techniques Learned

- What questions should be asked before starting the project.
- Creating calculated columns
- Creating measures using DAX language
- Data modeling
- Star & Snowflake Schema
- Using Field Parameters
- Using bookmarks to switch between two visuals
- Dynamic page navigation with buttons
- Dashboard designing
- Using the divide function to prevent zero division errors
- Creating a date table using M language
- Dynamic titles based on the applied filters
- Tooltips
- Toggle Button
- Dynamic Slicers
- Using KPI indicators
- Conditional formatting of values in visuals using icons or background color
- Data Validation techniques
- Report Optimization

### Power BI Services

- Publishing reports to Power BI services
- Setting up a personal gateway to set up the auto-refresh of data
- Power BI App creation
- Collaboration, workspace, access permissions in Power BI services

### Quality Assurance & Review

- User Acceptance Testing (UAT)
- Stakeholder Review & Feedback implementation

## GitHub

- Uploading large-size files using GitHub LFS
- Tracking specific types of file extensions for LFS

## Business-Related Terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales (Revenue)
- Net profit
- COGS - Cost of Goods Sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer
- Customer
- Benchmark

## Company’s Background

AtliQ Hardware is a company that has grown vastly in recent years and opened businesses all over the globe. It sells computers and computer accessories through three mediums/channels:

- Retailers
- Direct
- Distributors

While they grew substantially in the last few years, they also had some bitter experiences in Latin America. They tried establishing their presence there but faced huge losses because all decisions were based on some surveys, intuitions, and some basic Excel based Data Analysis.
They were using Excel for analysis but now the company got big so they switched over to PowerBI and wanted to bring lot of transparency in the data and make accurate decisions. Their competitors are growing and making use of data analysis on a large scale and they too want to leverage the power of data analysis. Therefore, AtliQ Hardware had no other option but to build its analytics team for data-driven insights and decisions in the future to survive better in the industry.

## Project Kick-Off Session

During the project kick-off session, clarify the following:

- What is the objective of building this Power BI dashboard?
- What are the different data sources?
- What are the critical KPIs for assessing success and platform performance?
- What is the project deadline?
- Do the stakeholders expect a preview before the actual release?
- What are the stakeholders' hopes for this project?
- What are the stakeholders' fears regarding building this dashboard?
- Who will be using this dashboard and for what purpose?
- What are the stakeholders' expectations for the project's completion?
- Are there any risks that could derail the project or the timeline?
- What resources/data are needed to build this dashboard?
- Are there any inputs from stakeholders in terms of design and views of the dashboard?
- How frequently does the dashboard need to be updated?

After the project kick-off meetings, the data engineering team provided the data as requested by the data analytics team. Let’s explore them.

## Dataset Understanding

Understanding available data is crucial before performing analysis. Ensure a good understanding of the available data before jumping into the analysis.

### Dimension Table

Contains static data like details of customers and products:

- **dim_customer**: 27 distinct markets (e.g., India, USA, Spain), 75 distinct customers throughout the market, 2 types of platforms (Brick & Mortar - Physical/offline store, E-commerce - Online Store), and three channels (Retailer, Direct, Distributors).
- **dim_market**: 27 distinct markets, 7 sub-zones, 4 regions (APAC, EU, NA, LATAM).
- **dim_product**: Divisions (P & A, Peripherals, Accessories, PC, Notebook, Desktop, N & S, Networking, Storage), 14 different categories, and different variants available for the same product.

### Fact Table

Contains data about transactions:

- **fact_forecast_monthly**: Used to forecast customer needs in advance, aiming for higher customer satisfaction and reduced storage costs. The table is denormalized by the data engineering team for analytical work, with all dates of the month replaced by the start date of the month.
- **fact_sales_monthly**: Similar to the fact_forecast_monthly table but with sold quantity instead of forecast value.

### Other Tables

- **freight_cost**: Details of travel and other costs for each market with the fiscal year.
- **gross_price**: Details of gross prices with product code.
- **manufacturing_cost**: Details of manufacturing costs with product code and year.
- **pre_invoice_deductions**: Details of pre-invoice deductions percentage for each customer with year.
- **post_invoice_deductions**: Post-invoice deductions and other deductions details.

## Importing Data into Power BI

Since the database is **MySQL** in this project, we need to import the datasets from the MySQL database to Power BI by providing the database access credentials.

## Data Model

Data modeling plays a vital role and is considered the foundation of the report. All visuals will be built upon the data model. Poor data modeling affects the overall performance of the report. Following good data modeling practices is essential. Refer to this [blog](https://addendanalytics.com/blog/data-modelling-best-practices) to understand good practices.

In this project, we followed the Snowflake data modeling method.

![Data Modeling](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/data%20model.png)

## Dashboard Design

Based on the mock ups received as per the requirements, visual designing and measures will be created as and when required.

## Home View

In Home View, all the view buttons are available. Users will land on a specific page depending on which button they click on. 

- Finance View
- Sales View
- Marketing View
- Supply Chain View
- Executive View
- Info
- Support

## Report Overview

![]()

## Home Page

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/home-page-gif.gif)

## Finance View

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/FinanceView-gif.gif)

## Sales View

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/SalesView-gif.gif)

## Marketing View

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/MarketingView-gif.gif)

## Supply Chain View

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/SupplyChainView-gif.gif)

## Executive View

![](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/Resources/ExecutiveView-gif.gif)

To view the full report 
- ![Report](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/BI360.pbix)
- ![PDF](https://github.com/Avinash-Jha19/Business-Insights-360/blob/main/BI360.pdf)
