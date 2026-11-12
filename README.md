# 🏙️ NYC Airbnb Market Analysis — Power BI Dashboard

An end-to-end 4-page interactive Power BI dashboard analyzing 48.9K+ NYC Airbnb listings across all five boroughs—covering market pricing, geographic distribution, host supply concentration, and historical review demand.

## 📊 Dashboard Pages
1. **Executive Market Overview:** High-level KPIs (Total Listings, Average/Median Price, Total Reviews, Total Hosts), borough-by-room-type distribution, and interactive synced slicers.
2. **Geographic & Pricing Deep Dive:** Custom County-level filled map, top neighborhoods by average price, and a Price vs. Availability correlation scatter plot.
3. **Host Performance & Supply Analysis:** Segmentation of Single-Listing vs. Multi-Listing hosts (`Multi-Listing Share %`), minimum-stay supply breakdown, and a Top Hosts Leaderboard.
4. **Demand & Review Activity Trends:** Historical review volume timeline, active listings over the last 12 months (`Active Listings (Last 12M)`), and zero-review inventory tracking.

## 🛠️ Technical Highlights & Problem Solving
* **Data Modeling & DAX:** Built custom measures for `Multi-Listing Share %`, `Avg Listings per Host`, `Active Listings (Last 12M)` (anchored dynamically via `EDATE` and `MAX`), and `Zero-Review Listings %`.
* **Geospatial Mapping Workaround:** Resolved organization-level Bing/Azure Map restrictions by engineering a `County_Map` calculated column mapped to NYC borough counties inside Power BI's Filled Map visual.
* **UI/UX Design System:** Designed a 1280×720 canvas with a reusable grouped header banner, brand-aligned color palette (`#FF5A5F`, `#00A699`, `#767676`), and synced cross-page slicers.

## 📁 Repository Files
* `NYC_Airbnb_Market_Analysis.pbix` — Interactive Power BI Desktop report
* `NYC_Airbnb_Dashboard_Report.pdf` — 4-page static export
* `/screenshots` — High-resolution previews of all four dashboard pages
