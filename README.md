# Samsung Supply Chain & Logistics Dashboard

## 📌 Project Overview
This project is an end-to-end **Supply Chain and Logistics Analytics Dashboard** built in Power BI, designed to monitor and optimize operations for a global electronics manufacturer (Samsung). 

The goal of this project was to transform raw operational data into a scalable, enterprise-grade data model and layer it with a highly interactive, "website-style" user interface. The dashboard allows stakeholders to seamlessly navigate through high-level overviews down to granular metrics across suppliers, inventory, shipments, and customers.

## 🗄️ Data Architecture & Modeling
A major focus of this project was establishing a robust relational data model capable of handling complex supply chain metrics without compromising report performance. 

![Data Model](Image/DataModeling%20Image.png)

The backend utilizes a comprehensive **Star/Snowflake Schema** consisting of:
* **Fact Tables:** `fact_sales`, `fact_inventory`, `fact_production`, `fact_procurement`, and `fact_shipment` to track transactional events.
* **Dimension Tables:** `dim_product`, `dim_customer`, `dim_date`, `dim_supplier`, and `dim_facility` for filtering and cross-analysis.
* **DAX:** Custom measures were developed to calculate advanced metrics like `Discount %`, perfect order percentages, and dynamic inventory turnover.

## 🌐 Website-Style Navigation
To enhance the user experience, the report eschews standard Power BI tabs in favor of a sleek, built-in navigation bar. Using buttons and page navigation actions, users can easily jump between different functional areas of the business, starting from a clean, branded Home Page.

![Home Page](Image/Home%20Dashboard%20Image.png)

## 📊 Dashboard Pages & Features

### 1. Overview
Acts as the executive summary, providing macro-level financial KPIs ($186.86M Gross Revenue, $48.56M Profit) and snapshot indicators for supply chain health. It includes mini-visuals tracking order quantities, inventory stock, shipment delays by carrier, and revenue by platform.
![Overview Page](Image/Overview%20Dashboard%20Image.png)

### 2. Supplier Performance
Tracks vendor efficiency and cost. Key features include monitoring Total Unit Cost ($78.13M), Average Lead Times (11.53 Days), and Average Quality Scores. The charts identify top-performing suppliers (e.g., Taiwan Semiconductor, Sony) vs. those with longer lead times.
![Supplier Page](Image/Supplier%20Dashboard%20Image.png)

### 3. Inventory & Production
Monitors stock levels against safety thresholds. Highlights include tracking 160K in Inventory Value, Defective Units, and Turnover Rates. A standout visual is the combined chart tracking Current Stock vs. Safety Stock vs. Reorder Points for specific flagship products (e.g., Galaxy S24 Ultra).
![Inventory Page](Image/Inventory%20Dashboard%20Image.png)

### 4. Shipment & Logistics
Focuses on outbound logistics, tracking $19.42M in shipment costs and carrier delays. It breaks down the 573 total delays by carrier (Maersk Line leading with 87 delays) and isolates root causes (Carrier Delays, Customs, Documentation). 
![Shipment Page](Image/Shipment%20Dashboard%20Image.png)

### 5. Customer & Sales
Analyzes the end point of the supply chain. Tracks profitability across different sales channels (Retailer, Online, Direct). Features a scatter plot analyzing the correlation between Discount %, Quantity Sold, and Total Revenue across product categories (Smartphones vs. Wearables).
![Customer Page](Image/Customer%20Dashboard%20Image.png)

## 💡 Key Business Insights
1. **Logistics Bottlenecks:** Maersk Line and DHL Express account for the highest total shipment delays. Furthermore, the primary reason for delivery failures stems from "Carrier Delays" and "Documentation," highlighting a need for better paperwork compliance and carrier renegotiations.
2. **Inventory Optimization:** Flagship products like the *Galaxy S24 Ultra* and *Galaxy Buds2 Pro* are maintaining healthy buffers above their safety stock levels, but defect rates for the S24 Ultra peak at 4.3K units, requiring a review of the production line.
3. **Supplier Quality:** Taiwan Semiconductor and Sony Semiconductor are delivering the highest Average Quality Scores (98) while maintaining consistent lead times, making them the most reliable vendors in the network.
4. **Sales Channels:** Retailers drive the largest portion of revenue (41.39%), but Online channels (18.2%) represent a high-margin growth area. 

## 🛠️ Files Included
*  [Download the Power BI File (Supply Chain Dashboard.pbix)](Supply%20Chain%20Dashboard.pbix): The complete Power BI project file, including the data model, DAX calculations, and interactive report pages.

## 🎓 Credits & Learning Resources
This dashboard was developed to advance my skills in complex data modeling and UI/UX design in Power BI. 

A special thanks to the YouTube channel **"The Developer BI"** for the foundational concepts and design inspiration. You can view the tutorials that guided this build here:
* [Part 1 Tutorial](https://www.youtube.com/watch?v=UqrsTIiOnO4)
* [Part 2 Tutorial](https://www.youtube.com/watch?v=y_CR3EQLrpA&t=1721s)
* [The Developer BI Channel](https://www.youtube.com/@The-Developer-BI/videos)
