# 📊 Olist E-Commerce Intelligence Dashboard

[![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi)](https://klnaclk-my.sharepoint.com/:u:/g/personal/ganegod-cs20045_stu_kln_ac_lk/IQAkv02mLZXnRYwoEpyEv_wgAeqqqM_o2QefPw1iBfLSvg4?e=yQTJEX)
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=for-the-badge&logo=python)](https://python.org)
[![PDF Report](https://img.shields.io/badge/📄_View-PDF_Report-red?style=for-the-badge)](Olist_Dashboard.pdf)

> **An end-to-end business intelligence project analysing 100,000+ real Brazilian e-commerce orders — covering customer segmentation, delivery performance, payment analysis and revenue trends.**

---

## 🌐 View the Dashboard

👉 **[Download Full Dashboard (Power BI)](https://klnaclk-my.sharepoint.com/:u:/g/personal/ganegod-cs20045_stu_kln_ac_lk/IQAkv02mLZXnRYwoEpyEv_wgAeqqqM_o2QefPw1iBfLSvg4?e=yQTJEX)**

👉 **[View PDF Report](Olist_Dashboard.pdf)**

---

## 📌 Project Overview

Olist is a Brazilian e-commerce marketplace connecting small businesses to major retailers. This project analyses **100,000+ real orders from 2016–2018** to answer key business questions:

- 📈 How is revenue trending month over month?
- 👥 Who are our most valuable customers?
- 🚚 Which states have the worst delivery performance?
- 💳 How do customers prefer to pay?
- ⭐ Which product categories get the best reviews?

---

## 📊 Dashboard Pages

### Page 1 — Executive Summary
![Executive Summary](page1_executive_summary.png)

Key metrics at a glance — total revenue, orders, customers, average order value, review score and delivery time. Revenue trend line and top 10 product categories.

---

### Page 2 — Customer Intelligence (RFM Segmentation)
![Customer Intelligence](page2_customer_intelligence.png)

Customers segmented into 5 groups using **RFM Analysis** (Recency, Frequency, Monetary):
| Segment | Description |
|---------|-------------|
| Champions | Bought recently, buy often, spend the most |
| Loyal Customers | Regular buyers with good spend |
| Potential Loyalists | Recent buyers with growth potential |
| At Risk | Haven't purchased recently |
| Lost | Long inactive, low spend |

---

### Page 3 — Operations & Quality
![Operations & Quality](page3_operations_quality.png)

Delivery performance by state, review scores by product category, and order volume patterns by day of week.

---

### Page 4 — Payment Analysis
![Payment Analysis](page4_payment_analysis.png)

Payment method breakdown, average order value by payment type, and relationship between number of items and order value.

---

## 🔍 Key Business Insights

- 💰 **Revenue peaked in November 2017** — Black Friday effect clearly visible
- 🏆 **Health & Beauty** is the top revenue category
- 🚚 **Roraima (RR) and Amapá (AP)** have the longest delivery times — logistics gap
- 💳 **Credit card** is the dominant payment method (73% of orders)
- ⭐ **Average review score: 4.09/5** — strong customer satisfaction overall
- 👥 **Champions segment** drives disproportionate revenue despite being smallest group

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python (Pandas, NumPy) | Data cleaning, merging, RFM calculation |
| Matplotlib, Seaborn | EDA visualisations |
| Power BI Desktop | Dashboard design & DAX measures |
| DAX | Custom KPI measures |
| Google Colab | Python environment |

---

## 📂 Project Structure
olist-ecommerce-dashboard/
├── Olist_Dashboard.pdf          # Full dashboard export
├── page1_executive_summary.png  # Dashboard screenshot
├── page2_customer_intelligence.png
├── page3_operations_quality.png
├── page4_payment_analysis.png
├── monthly_trend.png            # Python EDA chart
├── rfm_segments.png             # RFM analysis chart
└── README.md

---

## 📈 DAX Measures Used

```dax
Total Revenue    = SUM(olist_master[total_payment])
Total Orders     = COUNTROWS(olist_master)
Total Customers  = DISTINCTCOUNT(olist_master[customer_id])
Avg Order Value  = AVERAGE(olist_master[total_payment])
Avg Review Score = AVERAGE(olist_master[review_score])
Avg Delivery Days = AVERAGE(olist_master[delivery_days])
```

---

## 🗂️ Dataset

- **Source:** [Kaggle — Brazilian E-Commerce by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Size:** 100,000+ orders | 8 relational CSV files
- **Period:** September 2016 – October 2018
- **Tables:** Orders, Customers, Products, Sellers, Payments, Reviews, Items

---

## 👩‍💻 Author

**Senuri Ganegoda**
- 🎓 BSc (Hons) Computer Science — Data Science, University of Kelaniya
- 💼 Data & Analytics Intern — Dialog Axiata PLC
- 🔗 [LinkedIn](https://linkedin.com/in/senuri-ganegoda-311227220)
- 🐙 [GitHub](https://github.com/senu045)

---

*⭐ If you found this project useful, please give it a star!*
