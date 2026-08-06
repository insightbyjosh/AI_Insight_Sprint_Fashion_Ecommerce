# Data Dictionary

## Overview

This document describes the datasets used in the **AI Insight Sprint™ Case Study #1 – Fashion E-commerce Executive Business Intelligence Dashboard**.

The project integrates four datasets to support revenue analysis, customer intelligence, product performance and marketing campaign evaluation.

---

# 1. Sales Dataset

| Column | Data Type | Description |
|----------|-----------|-------------|
| sale_id | Integer | Unique identifier for each sales transaction. |
| customer_id | Integer | Unique identifier linking each transaction to a customer. |
| product_id | Integer | Unique identifier linking each transaction to a product. |
| sale_date | Date | Date the transaction occurred. |
| channel | Text | Sales channel through which the purchase was made (e.g., E-commerce or App Mobile). |
| discounted | Integer/Boolean | Indicates whether a discount was applied (0 = No Discount, 1 = Discount Applied). |
| total_amount | Decimal | Total monetary value of the transaction. |

---

# 2. Customers Dataset

| Column | Data Type | Description |
|----------|-----------|-------------|
| customer_id | Integer | Unique customer identifier. |
| country | Text | Country where the customer is located. |
| age_range | Text | Customer age group used for segmentation. |
| signup_date | Date | Date the customer registered. |

---

# 3. Products Dataset

| Column | Data Type | Description |
|----------|-----------|-------------|
| product_id | Integer | Unique product identifier. |
| product_name | Text | Product name. |
| category | Text | Product category. |
| brand | Text | Product brand. |
| color | Text | Product colour. |
| size | Text | Product size. |
| catalog_price | Decimal | Standard selling price. |
| cost_price | Decimal | Product cost price. |
| gender | Text | Target customer gender. |

---

# 4. Campaign Dataset

| Column | Data Type | Description |
|----------|-----------|-------------|
| campaign_id | Integer | Unique campaign identifier. |
| campaign_name | Text | Marketing campaign name. |
| start_date | Date | Campaign start date. |
| end_date | Date | Campaign end date. |
| channel | Text | Marketing channel used. |
| discount_type | Text | Promotional discount category. |
| discount_value | Decimal | Discount amount or percentage offered. |

---

# Data Model Relationships

The datasets were integrated using Power BI relationships to create a unified analytical model.

| From | To | Relationship |
|------|----|--------------|
| Sales | Customers | customer_id |
| Sales | Products | product_id |
| Sales | Date Table | sale_date |
| Campaign | Sales | Business analysis where applicable |

---

# Purpose

The integrated data model supports:

- Revenue Intelligence
- Customer Intelligence
- Marketing Intelligence
- Executive Insights
- KPI Development
- Interactive Business Reporting

---

**Prepared by:**

Joshua Odekina

AI Insight Sprint™ Framework

August 2026