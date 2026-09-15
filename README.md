

<h1 align="center">✨ Aura — E-Commerce Analytics & Business Intelligence Dashboard</h1>

<p align="center">
  <strong>An end-to-end Power BI solution transforming raw e-commerce data into actionable strategic intelligence.</strong>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/222f43f6-66d8-485a-b687-ef849fc00522" alt="Aura - E-Commerce Analytics & Business Intelligence Dashboard Banner" width="100%">
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Tool-Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/ETL-Power%20Query-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Power Query">
  <img src="https://img.shields.io/badge/Language-DAX-orange?style=for-the-badge" alt="DAX">
  <img src="https://img.shields.io/badge/Modeling-Star%20Schema-blue?style=for-the-badge" alt="Star Schema">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status">
</p>

---

## 📌 Table of Contents

1. [Project Overview](#-project-overview)
2. [Key Business KPIs](#-key-business-kpis)
3. [Detailed Dashboard Breakdown](#-detailed-dashboard-breakdown)
   - [Page 1: Executive Summary & Financial Overview](#page-1-executive-summary--financial-overview)
   - [Page 2: Customer Analytics & Web Behavior](#page-2-customer-analytics--web-behavior)
   - [Page 3: Cohort & RFM Analytics](#page-3-cohort--rfm-analytics)
   - [Page 4: Logistics, Shipping & Fulfillment](#page-4-logistics-shipping--fulfillment)
   - [Page 5: Product Performance & Inventory Aging](#page-5-product-performance--inventory-aging)
4. [Data Modeling & Tech Stack](#-data-modeling--tech-stack)
5. [Strategic Business Recommendations](#-strategic-business-recommendations)
6. [How to Run / Clone the Project](#-how-to-run--clone-the-project)
7. [Repository Structure](#-repository-structure)
8. [Contact](#-contact)

---

## 🧭 Project Overview

**Aura** is a full-scale, 5-page **E-Commerce Analytics & Business Intelligence dashboard** built entirely in **Power BI**. The project simulates a real-world enterprise reporting environment for an e-commerce retailer, translating raw transactional, web behavior, logistics, and inventory data into a single source of truth for leadership decision-making.

The objective of Aura was to design a solution that allows stakeholders — from the CFO to the Supply Chain Manager — to answer critical business questions in seconds:

- *Where is our revenue actually coming from, and is it sustainable?*
- *Why are customers abandoning their carts at nearly a 58% rate?*
- *Which customers are our most valuable, and which are at risk of churning?*
- *How efficient is our fulfillment pipeline, and where are the bottlenecks?*
- *Which products are profitable "stars," and which are dead inventory tying up capital?*

To achieve this, the project follows industry best practices across the full BI lifecycle: **data extraction and cleaning (Power Query)** → **dimensional data modeling (Star Schema)** → **business logic layer (DAX measures)** → **interactive visualization and UX design (Power BI Report Canvas)**.

> 💡 **Portfolio Note:** This project demonstrates proficiency in ETL design, relational data modeling, advanced DAX (time intelligence, RFM logic, cohort analysis), and translating analytical findings into strategic business recommendations — core competencies for a Data Analyst / BI Developer role.

---

## 📊 Key Business KPIs

The table below summarizes the headline metrics surfaced across the Aura dashboard suite.

| Category | Metric | Value |
|---|---|---|
| **Financial** | Total Revenue | **$9.22M** |
| **Financial** | Total Profit | **$4.79M** |
| **Financial** | Profit Margin | **51.90%** |
| **Financial** | Total Active Orders | **107K** |
| **Financial** | Average Order Value (AOV) | **$86.52** |
| **Customer** | Total Customers | **100K** |
| **Customer** | Active Customers | **72K** |
| **Customer** | Conversion Rate | **10.58%** |
| **Customer** | Cart Abandonment Rate | **57.94%** |
| **Customer** | Repeat Customer Rate | **37.74%** |
| **Customer** | Customer Lifetime Value (CLV) | **$326.57** |
| **Customer** | VIP Customer Count | **2K** |
| **Logistics** | Return Rate | **11.79%** |
| **Logistics** | Cancellation Rate | **14.86%** |
| **Logistics** | Avg. Delivery Days | **2.51 days** |
| **Logistics** | Avg. Shipping Days | **0.46 days** |
| **Inventory** | Avg. Discount % | **23.01%** |
| **Inventory** | Avg. Days to Sell | **30.01 days** |
| **Inventory** | Unsold Items | **309K** |
| **Inventory** | Sold Items | **182K** |

### Core Calculation Logic

The headline profitability metric follows the standard margin formula, implemented as a DAX measure:

$$\text{Profit Margin \%} = \frac{\text{Total Profit}}{\text{Total Revenue}} \times 100 = \frac{\$4.79M}{\$9.22M} \times 100 = 51.90\%$$

Similarly, Average Order Value (AOV) is derived as:

$$\text{AOV} = \frac{\text{Total Revenue}}{\text{Total Active Orders}} = \frac{\$9,220,000}{107,000} \approx \$86.52$$

---

## 🖥️ Detailed Dashboard Breakdown

### Page 1: Executive Summary & Financial Overview

![Executive Summary Dashboard]<img width="1350" height="760" alt="Executive Summary   Financial Overview" src="https://github.com/user-attachments/assets/97586703-4c65-40e1-a08d-71a17b8cb3ce" />


The landing page of Aura is designed for **C-suite consumption** — a high-density, at-a-glance financial command center.

**Contents:**
- **Headline KPI Cards:** Total Revenue ($9.22M), Total Profit ($4.79M), Profit Margin (51.90%), Total Active Orders (107K), and AOV ($86.52).
- **Revenue by Category/Department:** A breakdown identifying top-performing product departments driving the top line.
- **Monthly Revenue Seasonality Trend:** A time-series line chart exposing seasonal peaks and troughs to support demand planning.
- **Traffic Source Revenue Share:** A donut/bar visual showing **Search as the dominant acquisition channel, contributing 70.01%** of total revenue — a critical insight for marketing budget allocation.
- **Interactive Revenue Decomposition Tree:** A drill-down AI visual allowing users to decompose total revenue dynamically across **Department → Category → Traffic Source → Country**, enabling root-cause analysis of revenue fluctuations without leaving the page.

**Business Value:** Executives can identify, within seconds, whether revenue softness is a category problem, a geography problem, or a channel problem.

---

### Page 2: Customer Analytics & Web Behavior

![Customer Analytics & Web Behavior Dashboard]<img width="1340" height="745" alt="Customer Analytics   Web Behavior" src="https://github.com/user-attachments/assets/d29aeaee-f977-4e80-92b2-e42eb5975063" />


This page shifts focus from *what* is happening financially to *why*, by examining the digital customer journey.

**Contents:**
- **Web Engagement KPI Strip:** Total Customers (100K), Active Customers (72K), Conversion Rate (10.58%), Cart Abandonment Rate (57.94%), and Repeat Customer Rate (37.74%).
- **E-Commerce Conversion Funnel:** A visual funnel tracking the customer journey from:

| Funnel Stage | Volume | Drop-off vs. Previous Stage |
|---|---|---|
| Total Sessions | 682K | — |
| Cart Additions | 596K | −12.6% |
| Orders Placed | 125K | −79.0% |
| Orders Delivered | 31K | −75.2% |

- **Geographic Sales Distribution Map:** A filled/bubble map visualizing sales concentration by country/region.
- **Abandonment vs. Conversion by Traffic Source:** A comparative chart cross-referencing which channels drive high-intent traffic versus high-abandonment traffic.

**Business Value:** Surfaces the single biggest leak in the revenue pipeline — the **79% drop-off between Cart Addition and Order Placement** — pinpointing exactly where UX/checkout optimization efforts should be focused.

---

### Page 3: Cohort & RFM Analytics

![Cohort & RFM Analytics Dashboard]<img width="1342" height="750" alt="Cohort   RFM Analytics" src="https://github.com/user-attachments/assets/e5adc5c8-92b5-495c-b04a-58582dfb61f7" />


A deep dive into customer retention behavior and value-based segmentation, powered by custom DAX logic.

**Contents:**
- **Customer Value KPIs:** Customer Lifetime Value — CLV ($326.57) and VIP Customer Count (2K).
- **Monthly Cohort Retention Matrix:** A heatmap-style matrix grouping customers by their acquisition month and tracking what percentage of each cohort remains active in subsequent months — the gold standard for measuring retention health over time.
- **RFM Customer Segmentation:** Customers scored and clustered on **Recency, Frequency, and Monetary** value into actionable segments:
  - 🟢 **Loyal** — Recent, frequent, high-spend customers (retention priority).
  - 🟡 **At-Risk** — Previously active customers showing declining engagement (win-back priority).
  - 🔴 **Lost** — Long-dormant customers with minimal recent activity (low-cost reactivation or deprioritize).
- **Return Rate by Category:** A ranked bar chart identifying **Jumpsuits & Suits** as the category with the highest return rate — a quality/sizing red flag.

**Business Value:** Moves the business from reactive, aggregate reporting to **proactive, segment-specific CRM strategy** (e.g., targeted retention campaigns for "At-Risk" customers before they churn).

---

### Page 4: Logistics, Shipping & Fulfillment

![Logistics & Fulfillment Dashboard]<img width="1342" height="741" alt="Logistics Shipping   Fulfillment" src="https://github.com/user-attachments/assets/7cdcc38f-bf93-43eb-b3f6-2f0c076e41b1" />


An operational lens on order fulfillment efficiency and supply chain health.

**Contents:**
- **Logistics KPI Cards:** Return Rate (11.79%), Cancellation Rate (14.86%), Avg. Delivery Days (2.51), Avg. Shipping Days (0.46).
- **Order Status Breakdown:** A pie/donut chart of the full order lifecycle distribution:

| Order Status | Share of Orders |
|---|---|
| Shipped | 30.01% |
| Complete | 25.04% |
| Processing | 20.09% |
| Cancelled | 14.86% |
| Returned | 10.01% |

- **Historical Order Trends:** A time-series visual tracking order volume and status mix over time to detect operational degradation or seasonal strain.

**Business Value:** With **~25% of all orders** currently in a non-completed state (Cancelled + Returned), this page directly quantifies the operational cost of fulfillment inefficiency and flags it for supply chain intervention.

---

### Page 5: Product Performance & Inventory Aging

![Product Performance & Inventory Aging Dashboard]<img width="1347" height="752" alt="Product Performance   Inventory Aging" src="https://github.com/user-attachments/assets/85489e6e-0a80-4c88-892b-fed038838800" />


The final page connects merchandising and warehouse operations, identifying capital efficiency issues.

**Contents:**
- **Inventory KPI Cards:** Avg. Discount % (23.01%), Avg. Days to Sell (30.01 days), Unsold Items (309K), Sold Items (182K).
- **Sold vs. Unsold Items by Distribution Center:** A comparative bar chart across fulfillment hubs (e.g., **Memphis, TN** and **Chicago, IL**), exposing which warehouses are carrying excess dead stock.
- **Top Categories by Profit Margin:** Ranked bar chart led by **Blazers & Jackets at 62.14% margin** — the business's most capital-efficient category.
- **Top & Bottom Products by Profit:** A paired ranking table/chart identifying hero SKUs to double down on, and loss-leading SKUs to re-price or discontinue.

**Business Value:** With **309K unsold units against only 182K sold** (a ~63% unsold rate), this page makes a direct, quantified case for inventory rationalization and smarter discount strategy.

---

## 🏗️ Data Modeling & Tech Stack

### Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| **Data Ingestion & Cleaning (ETL)** | Power Query (M Language) | Source connection, data type correction, deduplication, column splitting, and merge/append transformations |
| **Data Modeling** | Power BI Desktop | Relationship management, cardinality configuration, hierarchy creation |
| **Business Logic** | DAX (Data Analysis Expressions) | Calculated columns, measures, time intelligence, RFM scoring, cohort logic |
| **Visualization & UX** | Power BI Report Canvas | Custom theming, bookmarks, tooltips, drill-through, decomposition tree |
| **Version Control** | Git & GitHub | Project documentation and portfolio hosting |

### 🏗️ Data Modeling Approach: Galaxy Schema

Aura is built on a robust **Constellation / Galaxy Schema** architecture in Power BI to ensure optimal performance, proper data granularity, and seamless analytical reporting across Sales, Web Events, and Inventory.

```text
                  ┌──────────────┐
                  │   Dim_Date   │
                  └──────┬───────┘
                         │
      ┌──────────────────┼──────────────────┐
      │                  │                  │
      ▼                  ▼                  ▼
┌───────────┐  ┌──────────────────┐  ┌──────────────┐
│Fact_Orders│  │ Fact_Order_Items │  │ Fact_Events  │
└─────▲─────┘  └────────▲─────────┘  └──────▲───────┘
      │                 │                   │
      ├─────────────────┼───────────────────┤
      │                 │                   │
┌─────┴─────┐    ┌──────┴──────┐      ┌─────┴─────┐
│ Dim_Users │    │Dim_Products │      │Dim_Users  │
└───────────┘    └──────▲──────┘      └───────────┘
                        │
                ┌───────┴──────┐
                │ Dim_Inventory│
                └───────▲──────┘
                        │
              ┌─────────┴────────┐
              │ Dim_Distribution │
              └──────────────────┘
```

Core Tables Breakdown:
Fact Tables:

Fact_Orders: Captures high-level order transactions, overall order status, and total items count.

Fact_Order_Items: Granular line-item details linking individual purchased products, sale prices, and shipping timestamps.

Fact_Events: Captures web user behavior, browser sessions, IP addresses, and user interactions.

Dimension Tables:

Dim_Users: Master customer table containing demographic data, geography, RFM segmentation, and cohort tracking.

Dim_Products: Product catalog details including department, category, brand, and retail pricing.

Dim_Date: Dedicated date dimension table enabling advanced Time Intelligence functions (SAMEPERIODLASTYEAR, DATEADD, etc.).

Dim_Inventory & Dim_Distribution: Warehouse and supply chain metrics tracking product stock availability and fulfillment distribution centers

### Representative DAX Measures

```dax
Total Revenue = CALCULATE( SUM('Fact_Order_Items'[sale_price]),'Fact_Order_Items'[status] <> "Cancelled")

Total Profit = [Total Revenue] - [Total Cost]

Profit Margin % =
DIVIDE([Total Profit], [Total Revenue], 0)

Average Order Value =
DIVIDE([Total Revenue], [Total Active Orders], 0)

Cart Abandonment Rate =
VAR CartSessions = 
    CALCULATE(
        DISTINCTCOUNT('Fact_Events'[session_id]),
        'Fact_Events'[event_type] = "cart"
    )
VAR PurchaseSessions =  CALCULATE(
        DISTINCTCOUNT('Fact_Events'[session_id]),
        'Fact_Events'[event_type] = "purchase"
    )
VAR AbandonedSessions = CartSessions - PurchaseSessions
RETURN
DIVIDE(AbandonedSessions, CartSessions, 0)

Repeat Customer Rate =
VAR CustomerOrders = 
    ADDCOLUMNS(
        VALUES('Fact_Orders'[user_id]),
        "@OrderCount", CALCULATE(DISTINCTCOUNT('Fact_Orders'[order_id]))
    )

RFM Score =
VAR RecencyScore = [Recency Rank]
VAR FrequencyScore = [Frequency Rank]
VAR MonetaryScore = [Monetary Rank]
RETURN
    RecencyScore & FrequencyScore & MonetaryScore

Customer Lifetime Value (CLV) =
[AOV] * [Repeat Customer Rate %] * 10
```

---

## 🎯 Strategic Business Recommendations

Based on the insights surfaced by the Aura dashboard, the following data-driven recommendations are proposed:

1. **Diversify Traffic Acquisition Channels**
   With Search contributing **70.01%** of revenue, the business carries significant channel-concentration risk. Recommend a phased investment in Social and Email channels to reduce dependency and hedge against rising paid-search costs or algorithm changes.

2. **Prioritize Checkout Funnel Optimization**
   The steepest drop-off in the customer journey occurs between **Cart Additions (596K) and Orders Placed (125K)** — a ~79% loss. Recommend a UX audit of the checkout flow (guest checkout, payment options, shipping cost transparency) paired with A/B testing to recover a portion of the **57.94% cart abandonment rate**.

3. **Launch Targeted Retention Campaigns for "At-Risk" RFM Segment**
   Rather than broad-based marketing spend, allocate retention budget specifically toward the **At-Risk segment** identified in the RFM model — this is the highest-ROI intervention point before a customer becomes "Lost."

4. **Investigate Sizing/Quality Issues in Jumpsuits & Suits**
   This category shows the **highest return rate** in the portfolio. Recommend a size-chart audit, updated product imagery, and customer review sentiment analysis to isolate the root cause and reduce reverse-logistics costs.

5. **Rationalize Inventory in Underperforming Distribution Centers**
   With **309K unsold units** against 182K sold, recommend a SKU-level aging analysis by distribution center (starting with Memphis, TN and Chicago, IL) to identify candidates for markdown, redistribution, or discontinuation — freeing up working capital.

6. **Double Down on High-Margin Categories**
   **Blazers & Jackets (62.14% margin)** significantly outperform the portfolio average. Recommend increased marketing spend and shelf/homepage placement for high-margin categories to improve blended profitability without needing to grow topline revenue.

7. **Reduce the Cancellation Rate Through Root-Cause Analysis**
   At **14.86%**, cancellations represent a meaningful revenue leak. Recommend cross-referencing cancellation reasons (stock-outs vs. customer-initiated vs. payment failure) to target the specific operational fix required.

---

 
 
---

## 📬 Contact

**[Mariam Mahmoud Moursi]**
Data Analyst | Business Intelligence Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/maryam-allam-003b00415/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mariammahmoudmorsi-ui)


---

<p align="center"><em>⭐ If you found this project insightful, consider giving the repository a star!</em></p>
