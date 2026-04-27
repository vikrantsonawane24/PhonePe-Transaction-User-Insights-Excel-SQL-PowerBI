# 📱 PhonePe Transaction & User Insights Dashboard

An interactive **Power BI dashboard** analyzing PhonePe's digital payment transactions, user registrations, device brand distribution, and regional growth trends across India from **2018 to 2022**.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [Dataset Description](#dataset-description)
- [Dashboard Pages](#dashboard-pages)
- [Key Insights](#key-insights)
- [Setup & Usage](#setup--usage)
- [Folder Structure](#folder-structure)
- [Future Improvements](#future-improvements)

---

## Project Overview

This project explores PhonePe's transaction ecosystem across Indian states and districts. It combines **transaction-level data** with **user registration and device brand data** to answer:

- Which states and districts drive the highest transaction value?
- How has digital payment growth trended over the years?
- Which device brands dominate the PhonePe user base?
- How do transaction counts and values vary by quarter and transaction type?

The final output is a **2-page interactive Power BI dashboard** with dynamic slicers for Year, Quarter, State, District, Brand, Transaction Type, and more.

---

## Tech Stack

| Layer | Tool |
|---|---|
| Data Source | PhonePe Engagement (kaggle) |
| Visualization | Power BI Desktop |
| Map Visual | Bing Maps (built-in Power BI) |
| File Format | `.pbix` |

---

## Dataset Description

Data sourced from the **PhonePe engagement** from Kaggle

### Key Data Fields

| Field | Description |
|---|---|
| `state` | Indian state name |
| `district` | District within the state |
| `year` | Year of transaction (2018–2022) |
| `quarter` | Quarter (Q1–Q4) |
| `transaction_type` | Type of UPI transaction |
| `transaction_count` | Number of transactions |
| `transaction_amount` | Total value of transactions |
| `registered_users` | Number of registered PhonePe users |
| `brand` | Device brand used (Xiaomi, Samsung, Vivo, etc.) |
| `user_count` | Number of users per brand |

---

## Dashboard Pages

### Page 1 — Transaction & User Insights Dashboard

**KPI Cards:**
- Total Transaction Value: **₹121.39 Trillion**
- Total Transaction Count: **72 Billion**
- Total Registered Users: **3.5 Billion**

**Visuals:**
- 🗺️ **State-wise Transaction Analysis** — Bubble map showing transaction distribution across all Indian states
- 🥧 **User Brand Distribution** — Pie chart showing device brand share (Xiaomi 36.25%, Samsung 28%, Vivo 26.07%, Realme 9.17%, Tecno)
- 📊 **Top Districts by Transaction Value** — Bengaluru Urban, Hyderabad, Pune, Jaipur, Rangareddy
- 📈 **Transaction Growth Over Years** — Quarter-wise line chart from 2018 to 2022

**Slicers / Filters:**
- Year, Quarter, State, District, Brand, Transaction Type, User Count, Transaction Count, Amount, Percentage

---

### Page 2 — PhonePe Transaction Insights (Summary)

A curated insights page highlighting the most important findings from the data:

- Southern states like **Karnataka and Telangana** contribute the highest transaction value
- **Digital payments show strong growth** trend after 2020
- **Xiaomi and Samsung** dominate the PhonePe user base
- **Major urban districts** generate significantly higher transaction volume compared to rural regions

---

## Key Insights

- 💰 PhonePe processed over **₹121 Trillion** in total transactions between 2018–2022
- 📍 **Bengaluru Urban** is the single highest transaction value district in India
- 📱 **Xiaomi (36.25%)** leads device brand share, followed by **Samsung (28%)** and **Vivo (26.07%)**
- 📈 Transaction growth accelerated sharply **post-2020**, likely driven by the COVID-19 digital payment boom
- 🏙️ Urban districts far outperform rural regions in both transaction count and value
- 🌏 **Southern India** (Karnataka, Telangana) leads in transaction contribution compared to other regions

---

## Setup & Usage

### Prerequisites
- Power BI Desktop (free) — [Download here](https://powerbi.microsoft.com/desktop)

### Steps

1. **Clone this repository**
```bash
git clone https://github.com/your-username/phonepe-dashboard.git
cd phonepe-dashboard
```

2. **Open the dashboard**
   - Launch **Power BI Desktop**
   - Open `PHONEPAY.pbix`

3. **Interact with the dashboard**
   - Use the slicers on the left panel to filter by Year, Quarter, State, District, Brand, and Transaction Type
   - Toggle between **Page 1** and **Page 2** using the page buttons on the dashboard

> **Note:** The dashboard uses Bing Maps for the state-wise bubble map. An active internet connection is required for the map visual to render properly.

---

## Folder Structure

```
phonepe-dashboard/
│
├── PHONEPAY.pbix                  
│   ├── page1_dashboard.pbix
│   └── page2_insights.pbix        
└── README.md
```

---

## Future Improvements

- [ ] Add district-level drill-down map for deeper geographic analysis
- [ ] Include **year-over-year growth %** KPI cards
- [ ] Compare PhonePe trends with broader **UPI ecosystem data** (NPCI)
- [ ] Add **transaction type breakdown** (Merchant payments, P2P, Recharge, etc.)
- [ ] Publish to **Power BI Service** for online sharing

---

## Data Source

- 📦 **PhonePe Pulse** — Official open dataset by Kaggle


## 👤 Author

**Vikrant**
- 📍 Kalyan, Maharashtra, India
- 📧 vikrantsonawane24@gmail.com
- 🔗 www.linkedin.com/in/vikrantsonawane24/

---

> *This project was built as part of a data analytics learning journey to explore real-world fintech data using Power BI.*
