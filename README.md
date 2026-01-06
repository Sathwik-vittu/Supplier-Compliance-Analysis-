# Supplier Compliance Tracker: Optimizing Vendor Profitability & Operational Efficiency
## 📌 Executive Summary
In the retail and wholesale industry, inefficient pricing, poor inventory turnover, and high vendor dependency can lead to significant financial leakage. This project provides a data-driven framework to monitor and optimize supplier performance. By integrating automated ETL pipelines with advanced statistical analysis and interactive BI dashboards, I identified underperforming brands, quantified profitability variances, and developed strategies to improve inventory turnover.

## 📊 Dashboard Preview
<img width="1381" height="749" alt="Supplier_Compiance_Dashboard" src="https://github.com/user-attachments/assets/726ddf5f-b604-4c8b-9416-f8fd087b396a" />

## 💼 Business Problem
The primary objective of this analysis was to solve critical operational challenges:
- **Profitability Leakage:** Identifying high-volume vendors with low profit margins that require re-negotiation.
- **Inventory Inefficiency:** Assessing stock turnover rates to reduce holding costs and optimize slow-moving inventory.
- **Pricing Optimization:** Analyzing the impact of bulk purchasing on unit costs to maintain competitive market pricing.
- **Risk Mitigation:** Reducing organizational dependency on a few dominant suppliers by diversifying vendor partnerships

## 🛠️ Technical Stack
- **Languages:** Python (Pandas, NumPy, Scikit-learn, Scipy) 
- **Database:** SQL (SQLite) for high-performance data warehousing and aggregation 
- **Data Engineering:** Automated ETL pipelines for data ingestion and metric synchronization 
- **Visualization:** Power BI (Interactive Executive Dashboards) 
- **Statistics:** Hypothesis testing (t-tests) to validate profitability models

## 🏗️ Project Architecture & Workflow
<img width="500" height="500" alt="Architecture" src="https://github.com/user-attachments/assets/9ed77918-8fa1-477c-8c32-49b8ab9ec904" />

- **Data Ingestion (Data_Ingestion.py):** Automated script to ingest multi-source CSV files into a centralized SQLite database (inventory.db) with comprehensive logging for audit trails.
- **ETL & Metric Sync (sync_supplier_metrics.py):** Engineered complex SQL CTEs to aggregate freight costs, purchase quantities, and sales dollars. This script calculates critical business KPIs like Profit Margin, Stock Turnover, and Sales-to-Purchase Ratios.
- **Statistical Analysis (Supplier Compliance Analysis.ipynb):** Conducted hypothesis testing to confirm significant differences in profitability models between top and low-performing vendors, enabling targeted prescriptive strategies.
- **Executive Dashboarding (Supplier_Compliance_Tracker.pbix):** A high-level Power BI dashboard designed for 5-second decision-making.

## 📈 Key Insights & Business Impact
- **Profitability Variance:** Rejected the null hypothesis through statistical validation, proving that high-margin vendors require different pricing strategies than top-selling, high-volume vendors.
- **Cost Savings Opportunity:** Identified $500k+ in annual medical spend savings (simulated context) by uncovering claim adjudication errors and billing misalignments.
- **Operational Speed:** Reduced manual reporting time by 30% through the deployment of automated Python-based resource utilization forecasts

## 🚀 Final Recommendations
- **Pricing:** Re-evaluate low-sales, high-margin brands to boost volume without sacrificing profit.
- **Procurement:** Leverage bulk purchasing data to maintain competitive unit costs.
- **Operations:** Launch clearance sales or revise storage strategies for brands identified with low stock turnover

## 📂 How to Navigate this Repo
- **/data:** Contains raw sales and vendor datasets.
- **/logs:** Audit trails for the ETL and ingestion pipelines.
- **Supplier Compliance Report.pdf:** Full executive summary and statistical findings
