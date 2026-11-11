# Olist E-Commerce Supply Chain & Sales Performance Dashboard

[![Tableau](https://img.shields.io/badge/Tableau-View_Live_Dashboard-E97627?style=for-the-badge&logo=Tableau&logoColor=white)](https://public.tableau.com/app/profile/amey.yadav/viz/OlistE-CommerceSupplyChainCommercialDashboard/OlistE-CommerceSupplyChainCommercialDashboard)

## 🔗 Quick Links
* **Live Dashboard:** [Tableau Public Live View](https://public.tableau.com/app/profile/amey.yadav/viz/OlistE-CommerceSupplyChainCommercialDashboard/OlistE-CommerceSupplyChainCommercialDashboard)

## 📊 Live Interactive Preview
[![Olist Dashboard Preview](./assets/dashboard_preview.png)](https://public.tableau.com/app/profile/amey.yadav/viz/OlistE-CommerceSupplyChainCommercialDashboard/OlistE-CommerceSupplyChainCommercialDashboard)
*Click the preview image above to interact with filters and state mappings.*

# End-to-End-E-Commerce-Supply-Chain-Sales-Performance-Dashboard
I built this interactive dashboard using 99k+ real-world transactions from Olist to help executive leadership pinpoint fulfillment bottlenecks and profit leaks across Brazil's e-commerce network.
1. Business Problem
Logistics Bottlenecks: Customer order delivery times in the Northeast region of Brazil (e.g., Bahia, Maranhão, Pernambuco) were significantly higher than central hubs like São Paulo, driving down customer satisfaction and retention.
Margin Compression: High freight costs relative to product prices on oversized/heavy product categories were severely eroding net profitability across regional fulfillment lanes.
2. Data Architecture & Engineering
Relational Data Modeling: Architected a multi-table star schema connecting 5 core datasets: olist_orders_dataset, olist_order_items_dataset, olist_customers_dataset, olist_products_dataset, and product_category_name_translation.
Feature Engineering: Calculated dynamic fulfillment duration metrics using Tableau Calculated Fields (DATEDIFF('day', [order_purchase_timestamp], [order_delivered_customer_date])) to track fulfillment delay across 99,000+ orders.
Data Cleaning & Standardization: Resolved cross-regional timestamp mismatches, handled missing geographic coordinates, and mapped Portuguese category names into English for executive reporting.
3. Strategic Recommendations
Fulfillment Center Optimization: Decentralize warehousing from the Southeast and establish regional micro-fulfillment centers closer to high-volume demand hubs in the Northeast (specifically Bahia and Pernambuco) to reduce last-mile delivery times by an estimated 30–40%.
Shipping Fee & Category Restructuring: Re-evaluate shipping tariff rules and introduce minimum cart-value thresholds or weight-adjusted freight surcharges for high-freight, low-margin product categories to safeguard bottom-line margins.
