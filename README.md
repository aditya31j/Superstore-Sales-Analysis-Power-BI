# Superstore Analytics & Forecasting Dashboard


A comprehensive business intelligence solution for analyzing sales performance and forecasting future trends for the Superstore dataset.

---

##  Live Interactive Dashboard

### [Click Here to Interact with the Live Report](https://github.com/aditya31j/Superstore-Sales-Analysis-Power-BI/blob/main/Superstore%20Dashboard.pbix)


---

## 📖 Table of Contents
* [Dashboard Showcase]
* [Key Performance Indicators (KPIs)]
* [Dashboard Design & Interactivity]
* [In-Depth Analysis & Insights]
* [Sales Forecasting]
* [Technical Details]

---

## 🖼️ Dashboard Showcase

### Sales Overview Dashboard
![Sales Overview](https://github.com/aditya31j/Superstore-Sales-Analysis-Power-BI/blob/main/sales_dashboard.jpg.png)

### 15-Day Sales Forecast
![Sales Forecast](Images/forecast_dashboard.png)

---

##  Key Performance Indicators (KPIs)

The primary KPIs provide an at-a-glance understanding of the business's health. Each KPI is calculated using DAX for precision and context-awareness.

| KPI                  | Precise Value     | Description & Business Importance                                                                               |
| -------------------- | ----------------- | --------------------------------------------------------------------------------------------------------------- |
| **Total Sales**      | **$1,604,800.50** | The primary measure of revenue generation. This KPI tracks the total monetary value of all goods sold. |
| **Total Profit**     | **$175,321.80**   | The ultimate measure of profitability, calculated as `Total Sales - Total Cost`. It indicates the financial health and   efficiency of the business. |
| **Total Quantity**   | **22,450 Units**  | Represents the total number of individual products sold. Essential for inventory management and understanding      Product movement. |
| **Average Ship Days**|    **4 Days**     | The average time taken from order to shipment. A critical metric for operational efficiency and customer           satisfaction. |

---

## ✨ Dashboard Design & Interactivity

This dashboard is designed for intuitive exploration, allowing stakeholders to seamlessly move from a high-level overview to granular details.

* **Aesthetic & Layout:** A clean, minimalist design with a balanced color palette ensures that the data stands out. The layout follows a logical flow, with KPIs at the top, followed by detailed categorical and time-based analyses.
* **Central Filters:** Top-level buttons for **Region** (`Central`, `East`, `South`, `West`) act as master filters, allowing for a focused analysis of specific markets.
* **Cross-Filtering:** The entire dashboard is interactive. Clicking on a segment in any visual (e.g., clicking "Corporate" in the *Sales by Segment* donut chart) will instantly filter all other visuals on the page to reflect that selection.
* **Hierarchical Drill-Down:** Visuals like *Sales by Category* are designed to work in tandem with *Sales by Sub-Category*, providing a natural drill-down path without leaving the main page.

---

## 💡 In-Depth Analysis & Insights

> The dashboard reveals several key business insights that can drive strategic decisions.

#### Regional Performance
The **West** region is the clear revenue leader, contributing **33.37%** of total sales. However, profit analysis shows that some regions with lower sales may have higher profit margins, indicating opportunities for strategic growth.

#### Customer & Product Analysis
- The **Consumer** segment is the largest, accounting for **48.09%** of sales, highlighting the importance of B2C marketing strategies.
- **Office Supplies** is the highest-grossing category overall, but a closer look at sub-categories reveals that **Phones** (Technology) and **Chairs** (Furniture) are the most lucrative individual products.

#### Operational Efficiency
- **Standard Class** shipping is the most used mode (**$0.33M** in sales), yet an analysis of profit margins by ship mode could reveal if promoting faster (and potentially higher-margin) shipping options is viable.
- **COD (Cash on Delivery)** remains a highly popular payment method (**42.62%**), suggesting that digital payment adoption could be a key area for business improvement.

---

## 📈 Sales Forecasting

The second page of the report focuses on predictive analytics to forecast future demand.

* **Model:** Utilizes Power BI's native time-series forecasting algorithm, which analyzes seasonality and trends in the historical data (`Order Date`).
* **Forecast Period:** Projects sales for the next **15 days**.
* **Key Finding:** The forecast for early January 2021 shows an expected dip in sales (e.g., a predicted value of **$3.0K** on a specific day), which is typical after the holiday season rush seen in late December. The confidence interval provides a probable range for these future sales, aiding in inventory and staffing decisions.

---

## 🛠️ Technical Details

* **Data Source:** The public Superstore dataset (CSV/Excel).
* **ETL Process:** Data was loaded into Power BI and transformed using **Power Query** for cleaning (handling nulls, correcting data types) and structuring.
* **Data Modeling:** A star schema was implemented where appropriate to create relationships between the fact table (sales) and dimension tables (products, customers, etc.).
* **Languages:** **DAX (Data Analysis Expressions)** was used extensively to create the KPIs and other complex calculations.
