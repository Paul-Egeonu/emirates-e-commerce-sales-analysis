# 📊 Emirates E-Commerce Sales Analysis | Excel Dashboard & Power Query

![Excel](https://img.shields.io/badge/Tool-Microsoft%20Excel-green)
![Power
Query](https://img.shields.io/badge/Data%20Cleaning-Power%20Query-blue)
![EDA](https://img.shields.io/badge/Analysis-Exploratory%20Data%20Analysis-orange)
![Dashboard](https://img.shields.io/badge/Visualization-Interactive%20Dashboard-purple)
![Status](https://img.shields.io/badge/Project-Completed-success)

------------------------------------------------------------------------

# 📌 Project Overview

This project analyzes sales performance for a multi‑platform e‑commerce
marketplace using **Microsoft Excel, Power Query, Pivot Tables, and
dashboarding techniques**.

The goal of the analysis is to transform raw transactional data into
**actionable business intelligence** that can help decision‑makers
understand:

-   Revenue drivers
-   Product performance
-   Customer satisfaction trends
-   Platform efficiency
-   Market demand by geography
-   Sales growth opportunities

The project demonstrates a **complete end‑to‑end data analytics
workflow**, from business problem definition to strategic
recommendations.

------------------------------------------------------------------------

# 🎯 Business Problem

E‑commerce companies operate across multiple platforms, product
categories, and geographic markets. Without structured analytics, it
becomes difficult to understand:

-   Which products generate the most revenue
-   Which platforms perform best
-   Where demand is strongest
-   Whether customer satisfaction affects performance
-   What growth opportunities exist

This analysis answers those questions using **data‑driven insights**.

------------------------------------------------------------------------

# 🧠 Business Objectives

The analysis was designed to help stakeholders understand:

1.  Which products and categories generate the most revenue
2.  Which platforms perform best
3.  Which cities generate the highest demand
4.  Customer satisfaction trends based on ratings
5.  Which brands dominate the market
6.  Seasonal sales patterns
7.  Future revenue projections

------------------------------------------------------------------------

# 📂 Dataset

**Dataset:** `Emirates_E-commerce.xlsx`

The dataset contains **10,000 e‑commerce transactions** across multiple
products, cities, and platforms.

### Key Fields

-   Order ID
-   Order Date
-   Product
-   Brand
-   Category
-   Platform
-   City
-   Price
-   Quantity Sold
-   Rating
-   Reviews

------------------------------------------------------------------------

# 🛠 Tools & Technologies

  | Tool | Purpose |
|-----|--------|
| Microsoft Excel | Data analysis & dashboard creation |
| Power Query | Data cleaning & transformation |
| Excel Data Analysis ToolPak | Summary statistics |
| Pivot Tables | Data aggregation |
| Pivot Charts | Data visualization |

------------------------------------------------------------------------

# 💼 Resume‑Optimized Project Description

**Emirates E‑Commerce Sales Analytics Project**

Performed an end‑to‑end business analysis of **10,000 e‑commerce
transactions** using Excel and Power Query to identify revenue drivers,
platform performance, customer satisfaction patterns, and growth
opportunities.

Built an **interactive dashboard with dynamic slicers**, developed KPIs,
conducted exploratory data analysis, and generated strategic insights
capable of supporting executive‑level business decisions.

------------------------------------------------------------------------



# 🔄 Data Cleaning & Transformation

Data preprocessing was conducted in **Power Query** to ensure accuracy
and reliability.

### Key Steps

**1. Duplicate Removal**

Removed duplicate records to ensure data integrity.

**2. Revenue Calculation**

A new revenue column was created:

```m
= [Price] * [Quantity Sold]
```

**3. Customer Rating Classification**

Customer satisfaction categories were created:

```m
= if [Rating] <= 1.9 then "Very Poor" 
else if [Rating] <= 2.4 then "Poor" 
else if [Rating] <= 2.9 then "Average" 
else if [Rating] <= 3.9 then "Good" 
else if [Rating] <= 4.4 then "Very Good" 
else "Excellent"
```



**4. Data Type Correction**

Adjusted column types for:

-   Currency
-   Numeric values
-   Dates

**5. Chronological Sorting**

Transactions were sorted by **Order Date (ascending)** to support
time‑series analysis.

------------------------------------------------------------------------

# 📊 Summary Statistics

 | Measure | Price | Quantity | Revenue | Rating | Reviews |
|--------|------|----------|--------|-------|--------|
| Mean | $200.56 | 3.01 | $603.99 | 3.01 | 2520 |
| Median | $201.27 | 3 | $473.43 | 3 | 2537 |
| Mode | $11.65 | 4 | $753.30 | 3.4 | 2432 |
| Std Dev | $114.57 | 1.42 | $477.24 | 1.16 | 1443 |
| Minimum | $2.11 | 1 | $2.27 | 1 | 0 |
| Maximum | $399.99 | 5 | $1999.88 | 5 | 5000 |
| Range | $397.88 | 4 | $1997.61 | 4 | 5000 |
| Count | 10,000 | 10,000 | 10,000 | 10,000 | 10,000 |

Key observations:

-   Average product price ≈ **\$200**
-   Customers buy **\~3 items per order**
-   Average order value ≈ **\$603.99**
-   Revenue distribution shows **positive skewness**, indicating a few
    high‑value orders.

------------------------------------------------------------------------

# 📈 Key Performance Indicators (KPIs)

### Sales KPIs

  | KPI | Value |
|-----|------|
| Total Revenue | $6,039,914 |
| Total Orders | 10,000 |
| Total Quantity Sold | 30,062 |
| Average Order Value | $603.99 |

### Customer KPIs

 | KPI | Value |
|-----|------|
| Average Rating | 3.0 |
| Total Reviews | 25,200,722 |

### Product KPIs

  | KPI | Value |
|-----|------|
| Top Product | Xiaomi Redmi Note 12 |
| Top Category | Electronics |
| Best Brand | Xiaomi |

### Platform KPIs

  | KPI | Value |
|-----|------|
| Top Platform | Souq |
| Revenue | $2,038,419 |

------------------------------------------------------------------------

# 📊 Dashboard

An **interactive Excel dashboard** was created to visualize performance
metrics.

### Dashboard Visualizations

-   Revenue by Category
-   Monthly Sales Trend
-   Revenue by Platform
-   Revenue by City
-   Top Selling Products
-   Top Brands
-   Quantity Sold by Category

### Interactive Filters

Users can filter the dashboard by:

-   Month
-   Category
-   Brand
-   Platform
-   City

<img width="1322" height="536" alt="Emirates_E-commerce_Dashboard" src="https://github.com/user-attachments/assets/c2dc022a-ed84-4545-afaa-7490a962a7da" />


*(Insert GIF showing dashboard interaction here)*

------------------------------------------------------------------------

# 🔍 Key Insights

### 1. Balanced Platform Performance

Revenue distribution:

-   Souq --- 33.75%
-   Jumia --- 33.68%
-   Amazon --- 32.58%

This indicates **low dependency on any single marketplace**.

### 2. Electronics & Fashion Dominate Revenue

Top categories:

-   Electronics --- \$1.85M
-   Fashion --- \$1.83M

Together they generate **over 60% of total revenue**.

### 3. Strong Basket Size

Customers buy **\~3 items per order**, generating a strong **average
order value of \$603.99**.

### 4. Product Revenue Diversification

Top product revenues range between **\$561K -- \$675K**, indicating
**balanced product demand**.

### 5. Stable Monthly Sales

Revenue remains consistent throughout the year, indicating **stable
consumer demand**.

### 6. Customer Satisfaction Opportunity

Nearly **47% of reviews are average or below**, indicating potential
improvements in:

-   delivery
-   product quality
-   product descriptions

------------------------------------------------------------------------

# 📈 Business Recommendations

**1. Expand High‑Demand Categories**

Increase product assortment in **Electronics and Fashion**.

**2. Strengthen Brand Partnerships**

Collaborate with:

-   Xiaomi
-   Nike
-   Adidas
-   Samsung

**3. Improve Customer Experience**

Focus on:

-   delivery speed
-   product quality verification
-   improved customer support

**4. Increase Average Order Value**

Introduce:

-   product bundles
-   accessory upselling
-   cross‑selling promotions

**5. Optimize Platform Marketing**

Allocate advertising budgets based on **platform conversion
performance**.

------------------------------------------------------------------------

# 📈 Sales Projection

Current metrics:

Average Order Value = **\$603.99**

If order volume grows **10%**:

Projected Revenue ≈ **\$6.64M**

If AOV increases **5%**:

Projected Revenue ≈ **\$6.98M**

------------------------------------------------------------------------

# 🧱 Project Architecture

The project follows a structured analytics workflow:

Business Understanding\
→ Data Cleaning (Power Query)\
→ Data Transformation\
→ Exploratory Data Analysis\
→ KPI Development\
→ Pivot Table Analysis\
→ Dashboard Visualization\
→ Business Insights & Recommendations

------------------------------------------------------------------------

# 📁 Project Structure

    Emirates-Ecommerce-Analysis
    │
    ├── data
    │   └── Emirates_E-commerce.xlsx
    │    └── Emirates_E-commerce_Analysis.xlsx
    │
    ├── dashboard
    │   └── Excel Dashboard Screenshot.png
    │
    ├── visuals
    │   └── Dashboard Interaction.gif
    │
    └── README.md

------------------------------------------------------------------------

# 🚀 Project Value

This project demonstrates the ability to:

-   perform structured **business analysis**
-   clean and transform data using **Power Query**
-   conduct **exploratory data analysis**
-   develop **business KPIs**
-   create **interactive dashboards**
-   translate data into **strategic business recommendations**


------------------------------------------------------------------------

# 👤 Author

**Paul Egeonu**  
Data Analyst | Business Intelligence | Financial Analytics  

---

> ⭐ If you found this project insightful, feel free to star the repository.

Designed to demonstrate practical **Excel‑based business analytics
skills** applicable to real‑world e‑commerce decision making.
