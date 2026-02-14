# British Airways Customer Review Analysis

## 📊 Overview
This project showcases an end-to-end data analysis workflow using Tableau. The objective was to analyze British Airways customer reviews to identify trends in satisfaction across different metrics, aircraft types, and geographical locations.

**[View the Live Dashboard on Tableau Public](<div class='tableauPlaceholder' id='viz1771099371830' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BritishAirwaysReviews_17710966859090&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BritishAirwaysReviews_17710966859090&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Br&#47;BritishAirwaysReviews_17710966859090&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1771099371830');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1555px';vizElement.style.height='827px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1555px';vizElement.style.height='827px';} else { vizElement.style.width='100%';vizElement.style.height='1477px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>)**

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
- `Tableau-British-Airways-Customer-Review-Analysis-Dashboard.twb`: Tableau Packaged Workbook containing the dashboard.
