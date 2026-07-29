# Amazon-FMCG-Excel-project
## Amazon FMCG Supply Chain & Warehouse Data Analytics Dashboard
Executive Summary
This project presents a comprehensive end-to-end data analysis and interactive dashboard solution built for Amazon FMCG (Fast-Moving Consumer Goods) Warehouse Operations. The analysis covers a dataset of 25,000 operational warehouses, evaluating supply chain bottlenecks, storage efficiency, flood resilience, regulatory compliance, and regional capacity distribution.

Through multi-level analytical tiers (Basic Data Exploration, Medium Operational Insights, and Advanced Statistical & Regression Modeling), this repository provides actionable intelligence to optimize inventory refill throughput, reduce storage defects, and streamline warehouse network expansion.

## Business Problem & Objectives
Managing large-scale FMCG fulfillment operations requires continuous monitoring of physical infrastructure, logistics network proximity, and operational reliability. Key strategic goals addressed in this analysis include:

Capacity & Distribution Optimization: Evaluating how warehouse sizes (Large, Mid, Small) and ownership models (Company-Owned vs. Rented) affect throughput.

Risk Management & Infrastructure Assessment: Quantifying the operational impact of flood-prone locations, electric supply stability, and temperature-controlled machinery.

Root Cause Analysis of Storage Bottlenecks: Identifying key drivers behind storage issue reports and warehouse breakdowns.

Regulatory Compliance: Tracking government certifications, inspection frequencies, and structural safety standards.

## Data Dictionary
The underlying dataset contains 25,000 warehouse records across 32 operational attributes:

# Attribute      - Field	Data Type	Description
# Warehouse ID-   String	Unique identifier for each warehouse (WH_100000 to WH_124999)
# WH Manager ID	String- 	Unique employee ID of the warehouse manager
# Location type	- Categorical	Operating environment: Urban or Rural
# WH capacity size	-   Categorical	Capacity categorization: Large, Mid, Small
# zone	-  Categorical	Macro geographic zone (North, South, West, East)
# WH regional zone	-  Categorical	Granular operational zone (Zone 1 through Zone 6)
# num_refill_req_l3m	-Numeric	Count of inventory refill requests in the last 3 months
# transport_issue_l1y-	Numeric	Total transport/logistics disruptions reported in the last 1 year
# Competitor in mkt	-Numeric	Number of competing FMCG distribution centers in immediate market
# retail shop num	-  Numeric	Total retail outlets served by the warehouse
# distributor num	-   Numeric	Number of registered regional distributors associated
# flood impacted	-   Binary	Binary flag (1 = Previously flood-affected, 0 = No history)
# flood proof	Binary	-   Binary flag (1 = Certified flood-proof facility, 0 = Standard)
# electric supply	Binary-    	Availability of uninterrupted power grid / back-up
# distance from hub-   	Numeric	Distance in kilometers from the central distribution hub
# workers num	-  Numeric	Total workforce / employee headcount at the facility
#   storage_issue_reported_l3m-	Numeric	Count of storage-related incidents reported in the last 3 months
#  temp reg match	-Binary	Presence of functional temperature-regulation machinery (1/0)
# approved wh govt certificate	-   Categorical	Government certification status (A, B, C, or pending)
#   wh_breakdown_l3m-	Numeric	Operational breakdown instances over the past 3 months
#   govt_check_l3m	-Numeric	Frequency of government authority inspections in last 3 months
#   product wg ton-	Numeric	Total weight of stored/processed products (in Metric Tons)

## Key Analytical Insights & Findings
# Capacity & Warehouse Distribution

Dominant Sizes: Large warehouses account for 40.68% of total facilities, closely followed by Mid-sized facilities at 40.08%, while Small facilities represent 19.24%.

Refill Volumes: Large and Mid-sized facilities handle over 80% of total refill requests across the network, emphasizing their role as core bulk hubs.

## Operational Correlation Analysis
Warehouse Age vs. Storage Issues: A strong negative correlation (r≈−0.629) was identified between facility establishment year  and reported storage issues (storage_issue_reported_l3m). Modern/newer facilities feature significantly fewer storage failures, pointing to infrastructure aging in legacy units.

## Workforce Scale vs. Storage Issues: The correlation between workers num and storage issues is near zero (r≈−0.0087), showing that headcount alone does not mitigate operational storage errors; process efficiency and facility quality are primary drivers.

## Statistical & Regression Modeling
Linear Regression Assessment: Multiple regression models were fitted to evaluate product volume (product wg ton) and operational breakdowns. The weak overall explanatory power (R 2≈0.00028) indicates that tonnage is driven primarily by external order demand rather than internal physical facility age or worker count alone.

## Dashboard Layout & Interactive Features
The Excel Dashboard (dashboard for amazon FMCG sheet) integrates dynamic Pivot Tables, Slicers, and Visualizations allowing operational managers to perform cross-filtering across multiple dimensions:

## Summary Key Metrics
Total Warehouse Count (25,000 facilities)

Total Workforce Headcount & Average Workforce per Facility

Network Flood-Proofing Coverage Ratio

Government Compliance Grade Distribution

## Analysis Views
Zone-wise Warehouse Breakdown: Visualizing distribution across macro zones (North, South, East, West).

Capacity vs. Ownership Model: Comparing company-owned vs. rented facilities grouped by capacity size.

Storage Issues & Breakdown Heatmap: Identifying high-risk regional zones requiring structural upgrades.

## Interactive Slicers
Filter by WH_regional_zone
Filter by Location_type (Urban / Rural)
Filter by wh_owner_type (Company Owned / Rented)

## Strategic Recommendations
Legacy Warehouse Modernization: Prioritize capital expenditure updates on facilities built before 2010, as the data demonstrates an inverse relationship between facility age and storage issues (r=−0.629).

## AUTHOR
## AARZU BHARTI
