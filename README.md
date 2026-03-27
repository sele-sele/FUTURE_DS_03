# E-Commerce Conversion Performance Analysis (Python)

## Overview
This project analyzes e-commerce funnel data using **Python** to understand how users move through the customer journey from **Visitors → Leads → Customers**.

The analysis focuses on:
- cleaning and structuring funnel data
- measuring conversion performance
- identifying drop-off points
- comparing category performance
- analyzing trends over time
- providing actionable recommendations

The final output is a dashboard-style visualization built with Python

## Objectives
The project was designed to answer the following questions:

- How many users move from Visitors to Leads to Customers?
- What is the **Traffic-to-Lead conversion rate**?
- What is the **Lead-to-Customer conversion rate**?
- Where do the biggest **drop-off points** occur?
- Which product categories contribute most to conversions?
- How does conversion activity change over time?
- What recommendations can improve conversions?

## Dataset Description
The dataset contains e-commerce event-level data with the following fields:

- `event_time` — timestamp of user activity
- `event_type` — interaction type (`view`, `cart`, `purchase`)
- `product_id` — product identifier
- `category_id` — category identifier
- `category_code` — product category path
- `brand` — product brand
- `price` — product price
- `user_id` — unique user identifier
- `user_session` — session identifier


## Funnel Definition
The funnel was defined as:

- **Visitors** = unique users who performed a `view`
- **Leads** = unique users who performed `cart` or `purchase`
- **Customers** = unique users who performed a `purchase`

This approach was used to keep the funnel logically consistent in cases where some users had purchase events without a separately recorded cart event.


## Data Cleaning and Preparation
The following preprocessing steps were performed:

- Converted `event_time` into datetime format
- Created a `Date` column for time-based analysis
- Handled missing values in `category_code`
- Extracted simplified category labels from `category_code`
- Removed `"unknown"` categories from category-level visuals
- Used **unique users** for funnel KPIs
- Used **rolling averages** for trend visualization

---

## Tools and Libraries
- **Python**
- **Pandas**
- **Matplotlib**
- **NumPy**


## Key Metrics
The analysis includes the following KPI metrics:

- Visitors
- Leads
- Customers
- Traffic-to-Lead Conversion Rate
- Lead-to-Customer Conversion Rate
- Drop-off from Visitors to Leads
- Drop-off from Leads to Customers

## Dashboard Components
The final dashboard includes:

### 1. KPI Metrics
- Visitors
- Leads
- Customers

### 2. Conversion Funnel
- Visual representation of the user journey

### 3. Conversion Metrics
- Traffic-to-Lead %
- Lead-to-Customer %

### 4. Top Product Categories
- Categories generating the most purchase events

### 5. Lead Sources Performance
- Comparison of Leads vs Customers by category

### 6. Conversion Trend Over Time
- Trend of cart and purchase behavior over time

### 7. Insights and Recommendations
- Key findings
- Drop-off analysis
- Business recommendations

## Key Insights
Some of the main findings include:

- There is a **significant drop-off from Visitors to Leads**, indicating that initial engagement is weak.
- The **Lead-to-Customer conversion rate is relatively strong**, showing that users with purchase intent are more likely to convert.
- A few categories dominate conversions, with **smartphone-related products** performing best.
- Conversion activity changes over time, revealing useful behavioral trends.


## Recommendations
recommendations include:

- Improve landing page experience and calls-to-action to increase visitor-to-lead conversion
- Retarget users who browse but do not show purchase intent
- Prioritize high-performing categories in campaigns and merchandising
- Optimize low-performing categories for better engagement
- Track time-based conversion trends to improve strategy decisions


## Project Author
**Sereya Nchoe**
