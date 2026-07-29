# Nigeria Foreign Trade — Agricultural Exports Dashboard (Excel)

An Excel dashboard analyzing Nigeria's agricultural export performance using official NBS (National Bureau of Statistics) Foreign Trade in Goods data, covering Q1 2023 through Q1 2026.

![Dashboard Overview](screenshot_01_dashboard_overview.png)

## Business Question

How is Nigeria's agricultural export sector performing relative to total exports, and where is that value concentrated — by commodity, destination region, and export sector?

## Data Source

National Bureau of Statistics (NBS) Nigeria, Foreign Trade in Goods Statistics, Q1 2023–Q1 2026 (13 quarters).

## Structure

The workbook is built in three layers:

- **`Raw Data`** — source figures as published by NBS: quarterly total and agricultural export values, top commodities, sector breakdown, and destination region breakdown for the latest quarter
- **`Model`** — 6 PivotTables built directly from the Raw Data, feeding every chart on the dashboard. Nothing on the Dashboard sheet is a static, pasted-in number — it's all live off the pivot cache
- **`Dashboard`** — the presentation layer: 3 KPI cards, a trend line chart, and 3 supporting charts (bar, bar, pie), styled and laid out as a single-page report

## What's on the Dashboard

- **KPI cards:** Q1 2026 agricultural export value, year-over-year change, and agricultural share of total exports
- **Trend line:** agricultural export value by quarter, 2023–Q1 2026
- **Top commodities bar chart:** Q1 2026, by value
- **Destination region bar chart:** Q1 2026, by value
- **Sector share pie chart:** agriculture vs. crude oil, other oil products, raw materials, and other sectors, Q1 2026

## Key Findings

*(verified directly against the Raw Data sheet — reproducible by anyone who opens the file and checks the PivotTables)*

- **Agricultural exports fell 31.2% year-over-year in Q1 2026**, dropping to ₦1,172,373m from ₦1,704,145m in Q1 2025 — the strongest quarter in the entire series.
- **Agriculture's share of total exports has been volatile, not steadily growing.** It rose from 4.3% in Q1 2023 to a high of 8.3% in Q1 2025, then fell back to 5.5% by Q1 2026 — meaning both the sector's absolute value and its share of the export mix pulled back in the most recent quarter.
- **Export value is heavily concentrated in a single commodity.** Cocoa beans alone accounted for ₦596,896m in Q1 2026 — more than the next three commodities (sesame seeds, soya beans, cashew nuts in shell) combined.
- **Asia and Europe together absorb the vast majority of agricultural export value** (₦529,450m and ₦500,343m respectively in Q1 2026), while Africa (₦21,121m) and Oceania (₦261m) are marginal by comparison — despite Nigeria's regional trade ambitions under AfCFTA.
- **Agriculture remains a small fraction of Nigeria's total export economy.** At 5.5% of total exports in Q1 2026, it's dwarfed by crude oil (53%) and other oil products (32%) — the two together account for 85% of total export value.

## Techniques Used

- PivotTables and PivotCharts (6 pivot tables across 4 pivot caches) built from raw NBS source data
- KPI card design with conditional formatting for YoY change
- Multi-chart dashboard layout: line, bar, and pie charts on a single presentation sheet
- Three-layer workbook architecture (source → model → presentation) to separate raw data from calculation logic from the visual layer

## Files

- `nbs_foreign_trade_dashboard.xlsx` — the full workbook (Raw Data, Model, Dashboard)
- `screenshot_01_dashboard_overview.png` — dashboard screenshot, since GitHub cannot render Excel charts inline

## Author

Promise Odufuwa (Ascend)
Data Analyst
