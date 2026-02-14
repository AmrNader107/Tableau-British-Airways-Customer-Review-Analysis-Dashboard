# British Airways Customer Review Analysis

## 📊 Overview
This project showcases an end-to-end data analysis workflow using Tableau. The objective was to analyze British Airways customer reviews to identify trends in satisfaction across different metrics, aircraft types, and geographical locations.

**[View the Live Dashboard on Tableau Public](INSERT_YOUR_TABLEAU_PUBLIC_LINK_HERE)**

---

## 🛠️ Skills & Techniques Used

### 1. Data Connection & Modeling
* **Connecting to Data:** Imported multiple CSV files.
* **Data Modeling:** Established relationships between the main review dataset and a country mapping table based on geographical location.
* **Geographic Role Assignment:** Assigned geographical roles (Country/Region) to `place` columns to enable map plotting.

### 2. Advanced Data Transformation (Tableau)
* **Parameters:** Created a `[Pick a Metric]` parameter to allow users to dynamically switch the analysis between:
    * Overall Rating
    * Seat Comfort
    * Cabin Staff Service
    * Food & Beverages
    * Ground Service
    * Value for Money
    * Entertainment
* **Calculated Fields:** Wrote complex `CASE` statements to connect the parameter to the corresponding data fields.
* **Data Grouping:** Created an `[Aircraft Group]` to consolidate rare aircraft models into an "Other" category for cleaner visualization.

### 3. Visualization & Dashboarding
* **Dynamic Mapping:** Built a geographical map visualizing average ratings by country with customized background layers and tooltips.
* **Key Performance Indicators (KPIs):** Designed a summary bar with average scores across all metrics.
* **Interactivity:** Implemented dashboard actions, allowing users to click on visuals (e.g., a specific country or month) to filter the rest of the dashboard automatically.
* **Custom Formatting:** Applied brand-specific colors and tailored number formats for better readability.

---

## 🚀 Features
- **Metric Selection:** Instantly switch between different types of ratings.
- **Geographic Filters:** Analyze specific regions using a map or a dropdown menu.
- **Temporal Analysis:** Understand satisfaction trends over time using the monthly timeline chart.
- **Aircraft Analysis:** Identify which aircraft models receive the highest/lowest reviews.

---

## 📁 Files
- `ba_reviews.csv`: Raw review data.
- `countries.csv`: Geographical mapping data.
- `BA_Analysis.twbx`: Tableau Packaged Workbook containing the dashboard.
