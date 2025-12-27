# uber-freight-reliability-analysis
#  Logistics Reliability & Carrier Performance Scorecard

###  Executive Summary
**Goal:** Reduce "Value at Risk" and improve On-Time Performance (OTP) for a global logistics network.
**Role:** Data Analyst (Simulation)
**Tools:** Python (Pandas/NumPy), SQL (SQLite), Power BI.

###  Key Insights
* **Operational Bottleneck:** Identified **98,977** late shipments (54.83% failure rate), indicating systemic network issues.
* **Financial Impact:** The total "Value at Risk" (inventory delayed in transit) is **$18.08 Million**.
* **Carrier Performance:** Reliability is consistently low across 5 major carriers, with "Speedy Logistics" and "Yellow Freight" leading in delayed inventory value.
* **Geo-Spatial Discovery:** The dashboard revealed a critical failure node in **Caguas, Puerto Rico**, identifying a hub-level processing issue.

###  Dashboard Preview
![Dashboard](dashboard_screenshot.png)

###  How to Reproduce This Project
Since this project simulates a real-world pipeline, the database is generated locally.

1.  **Get the Data:** Download the [DataCo Smart Supply Chain Dataset](https://www.kaggle.com/datasets/shashwatwork/dataco-smart-supply-chain-for-big-data-analysis) from Kaggle.
2.  **Run the ETL Script:** Open `Data_Cleaning.ipynb` and run all cells. This will:
    * Ingest the raw CSV.
    * Clean column names and engineer features.
    * Generate the `supply_chain.db` SQL file locally.
3.  **Explore:** Connect the generated `.db` file to Power BI (or use the provided Python script for further analysis).

---
### ⚠️ Disclaimer
**Project Type:** Personal Portfolio / Simulation
**Note:** Carrier names were **synthetically generated** using Python to demonstrate domain-specific analysis. This dashboard does **not** represent actual internal data of Uber Freight.
