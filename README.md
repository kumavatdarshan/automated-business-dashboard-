# automated-business-dashboard-
Power BI dashboard monitoring e-commerce KPIs with automated DAX alert logic — revenue, churn, orders and customer health tracking
# 📊 Automated Business Health Monitoring Dashboard
### Power BI · E-Commerce Analytics · Real-Time KPI Alerts

A business intelligence dashboard that **automatically monitors e-commerce performance**, detects anomalies, and generates health alerts — eliminating the need for manual daily reporting.

---

## 🖼️ Dashboard Preview

> *Add screenshots of your Power BI dashboard here after building*

| Page | Description |
|---|---|
| Executive Overview | KPI cards, health score, live alert banners |
| Revenue & Trends | Daily/weekly revenue, day-of-week patterns |
| Customer & Category | Retention rate, category breakdown, customer mix |
| Channel & Payments | Acquisition channels, payment methods, city map |

---

## 🎯 Problem Statement

Most e-commerce businesses review performance **weekly or monthly**, missing critical signals like a sudden mid-week revenue drop, order volume declining 3 days in a row, or slowing customer acquisition before it becomes a crisis.

This dashboard solves that by **continuously monitoring health metrics** and flagging issues automatically the moment thresholds are breached.

---

## 🚨 Automated Alert System

Rule-based alert logic built entirely in DAX:

| Alert Level | Trigger Condition | Example |
|---|---|---|
| 🔴 CRITICAL | Revenue WoW drop > 20% | Revenue dropped 22% this week |
| 🟡 WARNING | Orders WoW drop > 8% | Order volume declining |
| 🟢 HEALTHY | All metrics within range | Revenue on track |

The **Overall Health Score** (0–100) aggregates 4 KPI signals into a single composite metric — updated with every slicer selection.

---

## 📐 KPIs & Measures Built

**Core KPIs:** Total Revenue · Total Orders · Average Order Value · New vs Returning Customers · Retention Rate · Return Rate

**Time Intelligence:** Revenue & Orders (Last 7 Days vs Previous 7 Days) · Week-over-Week % Change · Revenue by Day of Week

**Health Alerts (DAX):** Revenue Alert · Orders Alert · Churn Alert · Overall Health Score · Health Status (EXCELLENT / GOOD / FAIR / POOR)

**Category & Channel:** Category Revenue Share % · Revenue per Acquisition Channel · Performance by City

---

## 📁 Repository Contents

```
automated-business-dashboard/
│
├── ecommerce_data.csv             # 2,282 orders · Jan–Mar 2025 · 14 columns
├── BusinessHealthDashboard.pbix   # Power BI dashboard (4 pages)
├── DAX_Measures.txt               # All DAX formulas with comments
├── PowerBI_Build_Guide.txt        # Step-by-step build documentation
├── README.md
└── screenshots/
    ├── page1_overview.png
    ├── page2_trends.png
    ├── page3_customers.png
    └── page4_channels.png
```

---

## 📊 Dataset Overview

| Column | Description |
|---|---|
| order_id | Unique order identifier |
| order_date | Date of order (Jan 1 – Mar 21, 2025) |
| customer_id | Unique customer ID |
| customer_type | New / Returning |
| city | 10 Indian cities |
| category | Electronics, Apparel, Home & Garden, Sports, Beauty |
| product_name | Specific product |
| quantity | Units ordered (1–3) |
| unit_price | Price per unit |
| discount_pct | Discount applied (0–20%) |
| revenue | Final revenue after discount |
| channel | Acquisition channel (6 types) |
| payment_method | Payment method (6 types) |
| order_status | Delivered / Returned / Cancelled |

---

## 💡 Key Insights Discovered

1. **Electronics drives 38% of revenue** — highest AOV category, growing fastest
2. **Mid-week revenue dips 31%** vs weekends — opportunity for Tue–Thu promotions
3. **Returning customers spend 35% more** — loyalty programs have clear ROI
4. **Organic Search is the top channel** — 30% of revenue at lowest acquisition cost
5. **UPI is rising fast** — 25% of payments, preferred by mobile-first customers
6. **Revenue declined in March** — WoW drop triggers automated CRITICAL alert

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard design, visualizations |
| DAX | Calculated measures, alert logic, time intelligence |
| Power Query (M) | Data loading and transformation |

---

## 🚀 How to Use

1. Download `ecommerce_data.csv` and `BusinessHealthDashboard.pbix`
2. Open the `.pbix` file in Power BI Desktop
3. Update the data source path if prompted: Transform Data → Data Source Settings
4. Refresh the data — all measures and alerts recalculate automatically
5. Use the slicers (Date, Category, City, Customer Type) to filter any view

---

*Built to demonstrate automated business monitoring — moving from reactive reporting to proactive health tracking.*
