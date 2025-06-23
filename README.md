# B2B Courier Charges Accuracy Analysis 🚚📦

This project analyzes discrepancies between expected and invoiced courier charges in B2B ecommerce logistics. The analysis uses real-world datasets including order reports, SKU master data, and courier invoices to identify overcharges based on weight slabs and delivery zones.

## 🔍 Problem Statement

Courier companies often bill based on **weight slabs** and **delivery zones**, which can lead to discrepancies between the expected shipping cost and the amount actually invoiced. This project aims to detect those inconsistencies, flag overcharges, and improve visibility into cost accuracy.

## 📁 Dataset Overview

- `Order Report.csv` — Order-level data including weights and pincodes.
- `Courier Company - Rates.csv` — Rate card per zone and weight slab.
- `Invoice.csv` — Actual charges billed by the courier.
- `SKU Master.csv` — Product details and unit weights.

## 🛠️ Tools & Techniques

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Jupyter Notebook** in VS Code
- **Git & GitHub** for version control

## 📊 Core Analysis Steps

1. **Data Cleaning & Formatting**
   - Standardized columns, handled missing data
2. **Merged Datasets**
   - Joined SKUs, orders, pincodes, and courier invoices
3. **Calculated Weight Slabs**
   - Rounded weights based on slab rules (e.g., 1.3 kg → 1.5 kg)
4. **Mapped Zones**
   - Based on origin and destination pincodes
5. **Expected vs Actual Charges**
   - Compared calculated vs billed charges per order

## 🔎 Sample Insights

- Orders to Zone B were overcharged 8% more often than Zone A
- Over 35% of shipments were bumped to a higher weight slab unnecessarily
- SKU X consistently had billing inconsistencies, possibly due to weight misclassification

## 🧠 Bonus Ideas for Expansion

- Build a Streamlit dashboard for invoice audit reports
- Forecast expected shipping costs for upcoming orders
- Train a regression model to detect likely billing errors

## 👤 Author

Paulo Chernicharo  
📍 Lagoa Santa, MG, Brazil  
🔗 [GitHub Profile](https://github.com/pchernic)

## 📚 References

This analysis is based on the project walkthrough by [Aman Kharwal](https://amanxai.com/2023/05/22/b2b-courier-charges-accuracy-analysis-using-python/), adapted and extended with additional insights and tooling.


---

*Feel free to fork this repo or reach out with ideas or collabs!*
