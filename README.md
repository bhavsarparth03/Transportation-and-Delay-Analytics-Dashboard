# Transportation & Delay Analytics Dashboard

This repository documents my **Transportation & Delay Analytics** Tableau dashboard built on the **DataCo Smart Supply Chain** dataset. The viz helps operations teams diagnose **delays, SLA performance, and ticket backlog** across markets, regions, and service types.

**🟢 Live Dashboard:** https://public.tableau.com/app/profile/parth.bhavsar8858/viz/TransportationDelayAnalyticsDashboard/Dashboard1  
**🗂 Dataset (Kaggle):** https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis

---

## 🎯 Objectives
- Provide a single view of **KPIs**: total shipments, average delay, delay rate, SLA compliance
- Pinpoint **where** and **why** delays happen (geo heatmap + service-type comparison)
- **Prioritize** actions using an SLA bubble chart and ticket-resolution view
- Enable drill-downs with filter-aware insights for markets, regions, and segments

---

## 🧰 Tech Stack
- **Tableau Public / Desktop** – modeling, calculations, dashboarding
- **CSV/Excel (Kaggle)** – source data
- **SQL** – light cleanup before Tableau

---

## 📊 What’s in the Dashboard
1. **KPI Header** – Total Shipments, Avg Delay (days), Delay Rate (%), SLA Compliance  
   > Example snapshot: **180,516 shipments**, **3 days** avg delay, **45.30%** SLA compliance (filter-aware)
2. **Delay Heatmap** – geographic clusters of late deliveries (country/state/city)
3. **Delay Trend Over Time** – % delayed shipments by month to see seasonality/shift
4. **SLA Prioritization (Bubble)** – % Delayed (y) vs SLA Compliance (x) with guides  
   - Vertical **85% SLA threshold** and horizontal **90% delay-risk** line
5. **Service Type Comparison** – First/Same Day/Second/Standard (avg delay, delay rate, volume)  
   - Snapshot insight: **Same Day ≈ 0.5 days** avg delay; **Second Class ≈ 4.0 days**
6. **Ticket Resolution** – open vs resolved cases; filter by **SLA Breached** and **Customer Segment**

---

## 🧮 Metric Definitions
- **Average Delay (days):** Actual delivery − Promised delivery (0 if on time)
- **% Delayed Shipments:** Delayed ÷ Total in the current filter context
- **SLA Compliance:** Delivered within SLA ÷ Total
- **Open/Resolved Tickets:** Delivery-related support tickets by status

---

## 🔎 Key Insights (examples)
- **SLA compliance ~45%** (snapshot) ⇒ high improvement potential vs an 85% target
- **Same Day** consistently lowest average delay; **Second Class** highest ⇒ review routing/capacity
- Geo heatmap surfaces **regional hot spots** for targeted fixes
- Large **open-ticket** load; triage **SLA-breached** orders first to reduce churn

---

## 🚀 How to Use
1. Choose **Order Date** range and filters on the right (Market, Region/Country/State/City, Shipping Mode, SLA Breached, Customer Segment).  
2. Scan **KPIs** → open **SLA Prioritization** to rank problem areas.  
3. Use the **Heatmap** to drill into local bottlenecks.  
4. Compare **Service Types** to align promises with performance.  
5. Check **Ticket Resolution** to focus on SLA-related backlog.

---

## 👋 About Me
**Parth Bhavsar** — Business & Data Analyst (Toronto)  
- Tableau Public: https://public.tableau.com/app/profile/parth.bhavsar8858  
- LinkedIn: https://www.linkedin.com/in/parthbhavsar
- bhavsarparth03@gmail.com
