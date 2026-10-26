# Boston 311 Service Request Analysis

Analysis of 246,271 Boston 311 service requests (2025) to identify
geographic, departmental, and seasonal patterns that can improve
response times and resource allocation across the city.

## Key Findings

- **Geographic clustering:** Dorchester (31,010 requests) and Roxbury
  (22,521 requests, including 3,238 needle pickups) are the two
  highest-demand neighborhoods; the top 10 neighborhoods account for
  69.8% of total volume.
- **Department performance disparity:** PWDx resolves 88.1% of
  requests on time (1.7-day average); BTDT resolves only 32.7%
  on time (9.9-day average) despite comparable scale.
- **Seasonal demand:** Request volume rises 48.8% from January to
  September, with Tuesdays consistently the highest-volume day.
- **Digital adoption:** 85.83% of requests are now submitted
  digitally, versus 12.8% by phone.

## Tech Stack

- **Databricks / PySpark** — data processing, calculated fields,
  aggregation by neighborhood, department, and time period
- **Power BI** — interactive dashboard (KPI cards, trend lines,
  scatter plots, cross-filtering slicers)
- **Python** (Jupyter Notebook) — exploratory analysis

## Repository Structure

- `notebooks/` — full analysis notebook
- `data/` — source dataset from Boston's Open Data Portal
- `outputs/` — generated summary tables, organized by insight area
- `dashboard/` — Power BI dashboard file (.pbix)
- `REPORT.pdf` — full written analysis and recommendations

## Recommendations Summary

1. Deploy specialized cleanup crews to Roxbury for public health response
2. Conduct an immediate BTDT process audit; replicate PWDx's practices
3. Implement dynamic seasonal staffing (+40% June–September)
4. Continue mobile app investment while phasing down phone infrastructure

## Data Source

City of Boston. (2025). *311 Service Requests.* Boston Open Data Portal.
https://data.boston.gov/dataset/311-service-requests
