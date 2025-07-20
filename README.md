# ShopLink Africa Delivery & Inventory Analysis
A real-world business dashboard built during my Excel internship at RemilyTIQ, using a multi-table dataset drafted and cleaned by my teammate and me.
📊 Project Overview
This project focuses on uncovering operational issues faced by ShopLink Africa, a retail e-commerce company operating across West Africa. The company was experiencing:

⚠️ Frequent delivery delays

📦 Lost or late packages

💰 Erratic courier pricing

🛒 Popular items going out of stock

📉 Signs of customer churn

Using Excel, we transformed raw data from five different datasets into a unified dashboard that gives clear visibility into delivery performance, inventory health, and customer satisfaction.

🧩 Data Sources
We merged and analyzed the following datasets:

Orders Table: Order details, delivery date, delivery duration

Customers Table: Complaint counts, customer IDs

Couriers Table: Region, average courier cost

Inventory Table: SKU/Product ID, stock levels

Sales History Table: Product sales over a 4-week period

These tables were joined using VLOOKUP on common keys such as Order ID, Customer ID, and Product ID.

✅ Business Problems Solved
1. Where are delivery costs and durations the highest?
We calculated average courier costs and delivery durations, broken down by courier and region, using Pivot Tables and grouped summaries.

2. Which SKUs are at risk of stocking out?
We calculated a Stock Cover metric:

sql
Copy
Edit
Stock Cover = Current Stock / (Orders Per Week × 4)
and applied Conditional Formatting to flag SKUs that may stock out in <1 week.

3. Which regions and couriers are linked to customer churn?
By using the number of complaints as a proxy for churn, we created new labels (“Churned” vs. “Active”) and explored churn patterns by region and courier.

📌 Key Features
🔄 Dynamic Dashboard with slicers and filters

📈 Charts and Pivot Tables for interactive storytelling

🧠 Applied Excel functions: VLOOKUP, TRIM, IF, PivotTables, Conditional Formatting

💡 Business insight generation with clear action steps

📊 Insights & Recommendations
1. 🚚 Courier Performance — Delivery Timeliness & Duration
Insights:

Couriers with high late delivery rates include:

ExpressJet (Ghana)

GoDeliver (Togo)

FastShip (Togo)

RapidDrop (Togo)

Trackit (Benin)

These couriers also show longer average delivery durations (5–6 days).

Couriers with strong on-time performance and short durations (3 days) include:

LocalLink (Benin)

QuickBee (Togo)

ZapXpress (Togo)

Recommendations:

Audit courier operations for ExpressJet, GoDeliver, and Trackit to address late deliveries.

Consider reassigning deliveries in Benin to faster couriers like LocalLink and EcoCourier.

Strengthen partnerships with QuickBee and ZapXpress due to their high efficiency.

2. 💸 Cost vs. Performance — Courier Cost Effectiveness
Insights:

ExpressJet (₦9.02) and GoDeliver (₦8.90) are the most expensive couriers, yet they have the poorest delivery performance.

LocalLink is the most cost-effective courier (₦6.32) with reliable, on-time deliveries in just 3 days.

Recommendations:

Reassess courier contracts with ExpressJet and GoDeliver; their high cost does not translate to quality service.

Prioritize LocalLink for regions like Benin due to its strong performance at lower cost.

3. 📉 Churn Risk by Courier & Region
Insights:

Churn risk is highest in:

Ghana (33%)

Togo (13%)

Benin has no recorded churn cases.

Couriers with the highest churn-linked orders:

ExpressJet (2,914 orders) — Ghana

GoDeliver (2,748 orders) — Togo

Couriers like EcoCourier, QuickBee, and LocalLink are not associated with any churn.

Recommendations:

Investigate and improve customer experience for ExpressJet and GoDeliver.

Launch churn-prevention strategies in Ghana and Togo, including faster delivery, better communication, and post-purchase support.

Monitor high-risk regions with proactive tracking and feedback systems.

🛠 Tools Used
Microsoft Excel (Pivot Tables, Charts,)

Google Sheets (Data merging, conditional formatting)

Collaboration tools (Google meet, Slack)

🤝 Collaborators
Rebecca Emmanuel Bassey and Julius Chukwunaru – Data sourcing, initial cleaning, context building, validation, Data analysis, cleaning, merging, excel dashboard design.

 

📬 Contact
For questions or feedback, feel free to connect with me on LinkedIn https://www.linkedin.com/in/rebecca-emmanuel-bassey-847b80335/ or open an issue on this repository.

