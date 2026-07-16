# CRM-Sales-Performance-Analysis-with-Power-BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)([view](https://app.powerbi.com/view?r=eyJrIjoiMGIxY2ExMzEtYTM4ZS00NzBiLWE5ZDQtNGM5MzM2MGI2MDI1IiwidCI6ImI2NDU3ZDY4LTQzODgtNGMzYS04MjIyLTc0ZGU0NDU5ZDFlZiJ9&pageName=9f9f3953b30e7aef0e41))

![Medium](https://img.shields.io/badge/Medium-Case%20Study-000000?logo=medium)([view](https://medium.com/@ajagunalliyu/from-raw-crm-data-to-business-decisions-building-a-sales-performance-dashboard-for-brainards-group-335d53110168?sharedUserId=ajagunalliyu))

![Excel](https://img.shields.io/badge/Excel-Data%20Preparation-217346?logo=microsoft-excel)

![DAX](https://img.shields.io/badge/DAX-Measures-0066CC)

![License](https://img.shields.io/badge/License-MIT-blue)

An end-to-end interactive CRM sales performance dashboard built with Excel, Power Query, DAX, and Power BI to uncover actionable business insights from over 8,800 sales opportunities.

![](images/dashboard_page1.png)

## Dashboard

> Experience the dashboard online or explore the project below.

![Executive Dashboard](images/dashboard_page1.png)

## 🔗 Quick Links

🌐 **Live Dashboard**

> [POWER BI LINK](https://app.powerbi.com/view?r=eyJrIjoiMGIxY2ExMzEtYTM4ZS00NzBiLWE5ZDQtNGM5MzM2MGI2MDI1IiwidCI6ImI2NDU3ZDY4LTQzODgtNGMzYS04MjIyLTc0ZGU0NDU5ZDFlZiJ9&pageName=9f9f3953b30e7aef0e41)

📖 **Medium Case Study**

> [MEDIUM LINK](https://medium.com/@ajagunalliyu/from-raw-crm-data-to-business-decisions-building-a-sales-performance-dashboard-for-brainards-group-335d53110168?sharedUserId=ajagunalliyu)

📄 **Project Report (PDF)**

> reports/CRM Sales Dashboard Report.pdf

📂 **Dataset**

[Dataset Link](https://www.kaggle.com/datasets/innocentmfa/crm-sales-opportunities)


## 📖 Project Overview

Organizations generate large volumes of sales data every day, but raw data alone does not drive better decisions. This project demonstrates how Business Intelligence can be used to transform CRM sales records into meaningful insights that support strategic decision-making.

Using a publicly available CRM Sales Opportunities dataset from Kaggle, I developed an interactive Power BI dashboard that analyzes sales performance across consultants, products, customer sectors, and regional offices.

The project follows a complete analytics workflow—from data preparation and modeling to dashboard development and business recommendations, showcasing both technical implementation and business problem-solving.


## 📌 Project at a Glance

| Item | Details |
|------|---------|
| **Project Type** | Business Intelligence / Sales Analytics |
| **Industry** | Business Consulting & Professional Services |
| **Dataset** | CRM Sales Opportunities (Kaggle) |
| **Sales Opportunities** | 8,800 |
| **Client Accounts** | 85 |
| **Sales Consultants** | 35 |
| **Regional Offices** | 3 |
| **Products** | 7 |
| **Tools Used** | Excel, Power Query, DAX, Power BI |
| **Dashboard Pages** | 2 |
| **Outcome** | Interactive Executive Dashboard with actionable business insights |

---

# 📊 Dashboard Preview

### Executive Dashboard


![Executive Dashboard](images/dashboard_page1.png)


### Detailed Performance Dashboard


![Detailed Dashboard](images/dashboard_page2.png)

The dashboard was designed for interactive exploration.

Users can filter results by:

- Sales Consultant
- Manager
- Product
- Region
- Time Period


# 🎯 Business Problem

Brainards Group needed a clearer understanding of its sales performance.

Management wanted answers to questions such as:

- Which industry sectors generate the most revenue?
- Which consultants perform best?
- Which products contribute the most to sales?
- Which regional office performs best?
- How efficient is the sales pipeline?
- What actions can improve business performance?

Rather than relying on fragmented reports, this project provides a centralized dashboard that supports data-driven decision-making.


# ❓ Business Questions

The analysis was guided by six key business questions:

1. Which sectors generate the most revenue, and are we spending our energy in the right places?

2. What actually separates a won deal from a lost one—agent, sector, product, or something else?

3. How long does it really take to close business, and what does that tell us about how we sell?

4. Who are our strongest performers, and how does each consultant compare to the team?

5. Which products generate the most revenue, and how do they contribute to overall sales performance?

6. Which regions contribute the most revenue, and how does performance vary across regions?


# 📂 Dataset

This project uses the **CRM Sales Opportunities** dataset available on Kaggle [here](https://www.kaggle.com/datasets/innocentmfa/crm-sales-opportunities).

The dataset contains four related tables.

| Table | Description |
|---------|------------|
| Accounts | Company information |
| Products | Product catalogue |
| Sales Teams | Sales consultants and managers |
| Sales Pipeline | Sales opportunities |


# 🛠 Tools & Technologies

- Microsoft Excel
- Power Query
- Power BI Desktop
- DAX


# 🔄 Project Workflow

The project followed a complete analytics lifecycle.

Business Understanding
        ↓
Data Collection
        ↓
Excel Data Cleaning
        ↓
Power Query Transformation
        ↓
Data Modeling
        ↓
DAX Measures
        ↓
Dashboard Design
        ↓
Business Insights
        ↓
Recommendations
```

---

# 🧹 Data Preparation

The raw dataset was provided as four CSV files.

The preparation process included:

- Importing all CSV files into Microsoft Excel
- Consolidating the files into a single workbook
- Reviewing data quality
- Validating dates
- Checking for duplicates
- Standardizing categorical values
- Preserving active sales opportunities with blank close dates
- Importing the cleaned workbook into Power BI


# 📅 Date Table

A dedicated Date Table was created using DAX.

```DAX
Date Table = CALENDARAUTO()
```

Additional columns were created to support time intelligence:

- Year
- Quarter
- Month Name
- Month Number

This enabled accurate time-based analysis and chronological reporting throughout the dashboard.


# 🧩 Data Modeling

The model follows a **star-schema design**, with the **Sales Pipeline** table serving as the central fact table.

Dimension tables include:

- Accounts
- Products
- Sales Teams
- Date Table

Relationships were created to enable interactive filtering across the report.


## Data Model

![Data Model](images/data_model.png)


# 📈 Key DAX Measures

Examples of measures created include:

- Total Revenue
- Total Opportunities
- Won Deals
- Lost Deals
- Open Opportunities
- Win Rate
- Average Deal Size
- Average Sales Cycle

These measures dynamically respond to user selections, ensuring every visual updates automatically when filters or slicers are applied.


# 📊 Dashboard Features

### Executive Dashboard

The first dashboard provides a high-level overview of business performance.

It includes:

- KPI Cards
- Revenue by Sector
- Revenue Trend
- Product Performance
- Sales Outcome Distribution
- Interactive Filters


### Detailed Dashboard

The second dashboard provides operational insights into:

- Consultant Performance
- Product Analysis
- Regional Analysis
- Sales Pipeline
- Win Rate
- Opportunity Analysis


# 🔍 Key Insights

Some of the major findings include:

- Retail, Technology, and Medical sectors generated the highest revenue.
- Revenue differences across sectors were driven primarily by opportunity volume rather than higher win rates.
- Consultant performance varied significantly, with a small group generating a disproportionate share of total revenue.
- Regional win rates were remarkably similar, suggesting that lower-performing regions require more opportunities rather than additional sales coaching.
- GTK 500 recorded the highest average deal value, while also having the longest sales cycle.
- Revenue was broadly distributed across customer accounts, reducing dependency on a small number of clients.
- Monthly sales followed a noticeable quarter-end pattern.


# 💡 Recommendations

The analysis resulted in several business recommendations.

- Increase opportunity generation within the East region.
- Capture and replicate the practices of top-performing consultants.
- Prioritize high-value product strategies.
- Review products with unusually low deal values.
- Monitor long-running sales opportunities.
- Continue embedding data into strategic decision-making.


# 📁 Repository Structure

```
crm-sales-performance-analysis
│
├── dashboard
│   ├── CRM Sales Dashboard.pbix
│   ├── dashboard_page1.png
│   └── dashboard_page2.png
│
├── data
│   ├── accounts.csv
│   ├── products.csv
│   ├── sales_pipeline.csv
│   ├── sales_teams.csv
│   └── data_dictionary.csv
│
├── images
│   ├── data_model.png
│   ├── workflow.png
│   └── dashboard_images...
│
├── reports
│   └── CRM Sales Dashboard Report.pdf
│
└── README.md
```

---

# Explore the Project

## 🌐 View the Interactive Dashboard

Experience the dashboard online.

> [POWER BI LINK](https://app.powerbi.com/view?r=eyJrIjoiMGIxY2ExMzEtYTM4ZS00NzBiLWE5ZDQtNGM5MzM2MGI2MDI1IiwidCI6ImI2NDU3ZDY4LTQzODgtNGMzYS04MjIyLTc0ZGU0NDU5ZDFlZiJ9&pageName=9f9f3953b30e7aef0e41)


## 📖 Read the Medium Case Study

A detailed walkthrough of the project.

> [MEDIUM LINK](https://medium.com/@ajagunalliyu/from-raw-crm-data-to-business-decisions-building-a-sales-performance-dashboard-for-brainards-group-335d53110168?sharedUserId=ajagunalliyu)


## 📄 Read the Full Report

Open the PDF report included in this repository.


## 💻 Run the Project Locally

Clone the repository.

git clone ...

Open the PBIX.

Refresh.

Explore.


# 👨‍💻 About Me

Hi, I'm **Alliyu Ajagun**.

I'm a Data Analyst with a background in Applied Mathematics and a passion for transforming raw data into actionable business insights using Excel, SQL, Python, and Power BI.

I enjoy solving business problems through data visualization, dashboard development, and analytical storytelling.


## Let's Connect
 
> Feel free to reach out: [ajagunalliyu@gmail.com](mailto:ajagunalliyu@gmail.com)  
> Connect with me on [LinkedIn](https://www.linkedin.com/in/alliyuajagun)  
> Follow on [Twitter/X](https://x.com/Sayyid_Alliyu)  
> Read more on [Medium](https://medium.com/@ajagunalliyu)  
> 💻 Explore more projects on [GitHub](https://github.com/ajagunalliyu)
> View [Portfolio website](https://sites.google.com/view/alliyutheanalyst/portfolio?authuser=0)


## ⭐ Support

If you found this project helpful or interesting, consider giving the repository a **star**. Your support helps increase the visibility of my work and encourages me to continue building and sharing data analytics projects.

Thank you for visiting!
