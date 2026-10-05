# 📊 Sales Performance Analysis

### Power BI dashboard to diagnose a revenue decline in a multi-country B2B market

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power_Query-217346?style=for-the-badge)
![Data Modeling](https://img.shields.io/badge/Data_Modeling-5C2D91?style=for-the-badge)

---

## 🎯 Business Questions

| # | Question | Focus |

| 1 | **Who is the most profitable customer?** | Age group and market segmentation (Europe vs. North America) using sales, average ticket, order frequency and CLV 

| 2 | **How do sales behave over time?** | Yearly trend, monthly seasonality and revenue concentration by country and company 

| 3 | **Why did sales decline in 2023–2024?** | Patterns, anomalies and root causes 

---

## 🔍 Key Findings

> **Revenue fell 2.3% from 2022 to 2023**, mainly due to the disappearance of the sales peaks that drove previous years.

- 🇩🇪 **The decline is concentrated in Germany:** a single company (Ac Fermentum Inc.) accounted for 30%+ of global revenue and dropped 68%.
  
- 📈 **Sweden leads in total revenue, but Germany has the highest average sales per company**, the market with the most potential and the biggest dependency risk.
  
- 📅 **Seasonality:** September and December are the strongest months; summer and November are consistently weak.
  
- 👤 **Most profitable profile (CLV):** 25–35 in the UK and 36–45 in the USA.

---

## 💡 Recommendations

1. **Reduce dependency** on a single key account in Germany by diversifying the customer portfolio.
2. **Concentrate campaigns** before the September and December peaks.
3. **Replicate the acquisition strategy** of the top CLV segments in similar markets.

---

## 🖥️ Dashboard

### 1️⃣ Top User Profile
Who buys more, who spends more and who is worth more in the long term (CLV), by market and age group.

### 2️⃣ Global Trend & Seasonality
Five-year revenue evolution, monthly seasonality and revenue concentration by country and company.

### 3️⃣ 2023–2024 Decline Diagnosis
Month-over-month variation, country and company breakdown, and CLV evolution to explain the drop.

---

## 🗂️ Data Model

Star schema with `transactions` as the fact table and `users`, `company`, `products` and a calendar table as dimensions. All measures are stored in a dedicated measures table.

### Key DAX Measures

| Measure | Description |

| `CLV` | Customer Lifetime Value: average spend × annual purchase frequency |
| `%VarSalesYear` / `%VarSalesMonth` | Year-over-year and month-over-month sales variation |
| `AvgSalesDay` | Average daily sales, used to compare months fairly |
| `CR` | Conversion rate by country |

## 📁 Data

Synthetic dataset provided as part of IT Academy Data Analytics course. It contains no real personal data.

---

## ▶️ How to Open

> [!NOTE]
> The report uses the **PBIR format**.

1. Install the latest version of [Power BI Desktop](https://www.microsoft.com/power-bi/desktop).
2. If the file does not open, go to **File → Options → Preview features**, enable **"Store reports using enhanced metadata format (PBIR)"** and restart Power BI.

