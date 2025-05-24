# Business Performance Dashboard

Business Performance Dashboard provides a clear, at-a-glance view of key challenges and opportunities for the small e-commerce shop:

* 📍 **Location-based Performance**
  Which regions are underperforming in sales? Identifying low-performing locations helps us target local promotions and adjust inventory.

* 👥 **Customer Tenure**
  Are new customers sticking around? Tracking customer tenure highlights when we risk losing buyers so we can refine our loyalty and re-engagement strategies.

* 💰 **Product Profitability**
  Which products drive our sales—and which drag them down? Spotlighting top and bottom performers informs assortment and pricing decisions.

* 📈 **Trend Detection**
  How is sales trending over time? Early trend signals allow us to optimize stock levels, plan marketing campaigns, and prevent stockouts or overstocks.

## Dashboard Features

* 📂 **Data Source**: [Kaggle](https://www.kaggle.com/datasets/rishikumarrajvansh/marketing-insights-for-e-commerce-company/data)
* 🔧 **Data Model**: Star schema with one fact table *F\_Online Sales* and two dimension tables: *D\_Calendar* and *D\_Customer*
* 🧮 **DAX Calculations**:

  * Dynamic calendar dimension spanning the transaction date range with attributes for calendar year, month name, month number, quarter, week number, and day name
  * **Is Weekday** flag classifying each date as Weekday or Weekend
  * Customer **Tenure Brackets** segmentation into cohorts: up to 6 months; 6–12 months; 1–2 years; 3–5 years
* 🔄 **Synchronized Slicers**: Date period, Is Weekday, Customer Tenure, Location, and Category for interactive filtering.
* 🎨 **Customized Theme**: Light, minimalistic design for a clean and modern look.

## Walk-through

### 1. Business Performance Overview
A concise snapshot of the shop’s overall performance, showcasing total sales, order count, and active customers. Used reference labels for KPIs to limin number of server calls.
<p align="center">
  <img src="https://raw.githubusercontent.com/KalinaKa/portfolio/main/Business%20Performance%20Dashboard/pages/Bussiness_Performance_Overview.png" alt="Dashboard Overview" width="800" />
</p>

---

### 2. Performance by Location
Breaks down sales and orders by region, allowing identification of top-performing areas and underperforming locations.

<p align="center">
  <img src="https://raw.githubusercontent.com/KalinaKa/portfolio/main/Business%20Performance%20Dashboard/pages/PerformanceLocation.png" alt="Location Analysis" width="800" />
</p>

---

### 3. Performance by Customer Tenure
Visualizes customer cohorts based on tenure length, highlighting the revenue contribution of each segment.

<p align="center">
  <img src="https://raw.githubusercontent.com/KalinaKa/portfolio/main/Business%20Performance%20Dashboard/pages/PerformanceTenure.png" alt="Customer Tenure" width="800" />
</p>

---

### 4. Product Performance
Compares products by sales volume and revenue, pinpointing best- and worst-selling items for targeted action.

<p align="center">
  <img src="https://raw.githubusercontent.com/KalinaKa/portfolio/main/Business%20Performance%20Dashboard/pages/ProductPerformance.png" alt="Product Performance" width="800" />
</p>

---


## Improvements

To deepen insights and tackle more complex business questions, the following improvements should be considered:

* **Margin Analysis**: Incorporate product-level cost data (once available) to move beyond revenue and see true profitability.
* **Returns Tracking**: Add a returns module to measure reverse flows, understand return rates by product and identify problem SKUs.
* **Stock Level Monitoring**: Blend in inventory data so you can spot potential stockouts or overstocks by location.
* **Cohort Analysis**: Group customers by signup date or first purchase to track retention curves and lifetime value over time.
* **Customer Segmentation**: Segment audience by behaviour, spend or demographics to tailor marketing and product offers and predict next purchase date to offer replenishment services.
* **Web Analytics Insights**: Integrate Google Analytics metrics to see how on-site behaviour (page views, bounce rate) feeds into sales trends.
* **Basket Analysis**: Discover product pairings and inform cross-sell or upsell promotions.
