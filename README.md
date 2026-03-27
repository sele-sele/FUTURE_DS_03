# E-Commerce Conversion Performance Analysis (Power BI)

## Overview
This project focuses on analyzing an e-commerce marketing funnel using **Power BI** to understand user behavior from **Visitors → Leads → Customers**.  

The goal was to identify conversion rates, detect drop-off points, evaluate category performance, and provide actionable recommendations to improve business outcomes.


## Objectives
The analysis aimed to:

- Measure **traffic-to-lead conversion**
- Measure **lead-to-customer conversion**
- Identify **drop-off points** in the funnel
- Compare performance across **product categories**
- Analyze **conversion trends over time**
- Provide **data-driven recommendations**


## Dataset Description
The dataset contains e-commerce user activity including:

- `event_time` — timestamp of activity  
- `event_type` — user action (`view`, `cart`, `purchase`)  
- `product_id` — product identifier  
- `category_code` — product category  
- `brand` — product brand  
- `price` — product price  
- `user_id` — unique user identifier  
- `user_session` — session identifier  


## Data Cleaning (Power BI)
Data was cleaned and prepared using **Power Query Editor**:

- Converted `event_time` to **Date/Time format**
- Removed **null values**
- Extracted simplified categories from `category_code`
- Created new columns for analysis (Date, Category group)
- Ensured correct **data types**
- Combined datasets (October & November) using **Append Queries**


## Data Modeling & Measures (DAX)
Key metrics were created using **DAX**:

### Funnel Metrics
- Visitors = DISTINCTCOUNT of users who viewed products  
- Leads = DISTINCTCOUNT of users who added to cart or purchased  
- Customers = DISTINCTCOUNT of users who purchased  

### Conversion Rates
- Traffic-to-Lead Conversion  
- Lead-to-Customer Conversion  

### Drop-Off Analysis
- Visitors → Leads drop-off  
- Leads → Customers drop-off  


## Dashboard Components

<img width="931" height="503" alt="image" src="https://github.com/user-attachments/assets/4b152097-a094-4416-844e-a596adbdaea1" />

The Power BI dashboard includes:

### 1. KPI Cards
- Visitors  
- Leads  
- Customers  

### 2. Conversion Funnel
- Visual representation of user journey  
- Highlights drop-off between stages  

### 3. Conversion Metrics
- Traffic-to-Lead (%)  
- Lead-to-Customer (%)  

### 4. Top Product Categories
- Categories generating the most conversions  

### 5. Lead Source Performance
- Comparison of Leads vs Customers by category  

### 6. Conversion Trend Over Time
- Time-based trend analysis using Date hierarchy  

### 7. Insights & Recommendations Panel
- Key findings and business recommendations  


## Key Insights
- There is a **significant drop-off from Visitors to Leads**, indicating a need to improve engagement.
- **Lead-to-Customer conversion is relatively strong**, showing effective conversion once interest is established.
- Certain categories ( smartphones) dominate conversions.
- Conversion performance varies over time, highlighting trends in user behavior.


## Recommendations
- Improve landing pages and product descriptions to increase initial conversion  
- Retarget users who do not proceed beyond browsing  
- Focus marketing efforts on high-performing categories  
- Optimize underperforming categories for better engagement  
- Continuously monitor trends to adjust strategies  


## Tools Used
- **Power BI**
  - Power Query (Data Cleaning)
  - DAX (Measures & KPIs)
  - Data Modeling
  - Dashboard Design & Visualization  

## Project Output
The final deliverable is an interactive **Power BI dashboard** showing:

- Funnel performance  
- Conversion rates  
- Category insights  
- Trend analysis  
- Business recommendations  


## Learning Outcomes
Through this project, I developed skills in:

- Power BI data transformation (Power Query)  
- DAX measure creation  
- Funnel and conversion analysis  
- Dashboard design and storytelling  
- Turning raw data into actionable insights  


## Author
**Sereya Nchoe**
