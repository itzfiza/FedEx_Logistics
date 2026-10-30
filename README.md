# FedEx_Logistics
Exploratory Data Analysis (EDA) on FedEx Logistics shipment history to discover cost drivers and operational bottlenecks delaying global deliveries.

# FedEx Logistics: Shipment Delivery & Cost Analysis (EDA)

An Exploratory Data Analysis (EDA) project evaluating FedEx Logistics shipment records to uncover factors driving delivery delays and high logistics spend.

## 📋 Project Summary
This project analyzes **10,324 shipment records** containing 33 original attributes representing purchase order (PO) flows, carrier configurations, destination lanes, and financial structures. Through automated pipelines, feature engineering, and statistical testing, we isolate critical bottlenecks in global delivery performance and estimate freight-to-insurance dynamics.

## 🚀 Key Findings
- **Baseline Performance:** **88.5%** of shipments are delivered On Time; **11.5%** face delivery delays.
- **Bottlenecks:** **Mozambique** experiences the lowest on-time performance among major lanes (**81.6%**). 
- **Shipping Terms:** Shipments managed under EXW are **95.0%** on time, while 'N/A - From RDC' terms lag at **82.8%**.
- **Cost Drivers:** Air transportation is the most expensive carrier option (median **$10.02/kg**), while Ocean is highly cost-effective (median **$1.68/kg**).
- **Lead Time Myth:** A Mann-Whitney U test disproves any significant link between standard scheduled lead times and actual transit delay outcomes ($p = 0.4122$).
- **Insurance Dynamics:** Insurance rates correlate almost perfectly with cargo valuation structures (nearly **99%** match) rather than package physical weights.

## 🛠️ Tech Stack & Methodology
- **Data Cleaning:** Regex stripping, datatype coercions, explicit NaT/NaN tracking (scything text placeholders).
- **Visualizations:** 22 bivariate, univariate, and multivariate charts built using Matplotlib, Seaborn, and Plotly.
- **Statistical Testing:** SciPy `Chi-Square` contingency, `Mann-Whitney U` test, and `Spearman Rank` correlation.

## 📂 File Structure
- `SCMS_Delivery_History_Dataset.csv` - FedEx logistics history raw dataset
- `FedEx_Logistics_EDA.ipynb` - Structured Jupyter notebook containing step-by-step cleaning, visualizations, and tests
- `README.md` - Repository overview
