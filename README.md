# 📺 YouTube Trends Dashboard — Global Video Category Analysis

![Tableau](https://img.shields.io/badge/Tableau-Dashboard-orange)
![Data Visualization](https://img.shields.io/badge/Data-Visualization-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Project Overview

This project was developed as part of the **Data Analytics Bootcamp at [TripleTen](https://tripleten.com)**.
It focuses on automating weekly analytics for **YouTube trending videos**, building a **Tableau dashboard** for ad-planning managers to track category trends and regional differences over time.

The dashboard helps answer:

* Which video categories trended most often last week?
* How were they distributed among regions?
* Which categories were especially popular in the United States?

🔗 **Live Dashboard:** [YouTube Trends Dashboard (Tableau Public)](https://public.tableau.com/app/profile/marcela.stephanie.pereira.maris1628/viz/DashboarddeTendnciasdoYoutube/Dashboard1)
📊 [**Open YouTube Trending Dashboard Presentation (OneDrive)**](https://1drv.ms/b/c/d1aeda57ea1dab69/ETe6SLqfANVPtnPp9PAoVTABSbvMgP2WEDA1WBingSMKIA?e=0Y2jAV)

---

## 🎯 Objectives

* Design and publish an **interactive Tableau dashboard** using raw event data.
* Provide **time-based and regional filtering** to support daily video category analysis.
* Build intuitive visualizations to explore **absolute counts and percentage trends**.
* Automate insight extraction for campaign planning teams.

---

## 📊 Dashboard Features

* 📅 **Date & Country Filters** — affect all visuals simultaneously.
* 🧮 **Trend History (absolute & %)** — stacked area charts showing category evolution over time.
* 🌍 **Regional Distribution** — pie chart of trending videos by region.
* 🔥 **Category × Country Heatmap** — highlights most frequent trending categories per region.
* 🧠 **Fully interactive design** with tooltips and consistent color mapping.

---

## 📂 Data Description

**File:** `trending_by_time.csv`
**Source:** Aggregated YouTube trending history table provided for Sprint 12.
**Fields:**

* `record_id` — unique row ID
* `region` — country or geographic region
* `trending_date` — date of trending event
* `category_title` — YouTube video category
* `videos_count` — number of trending videos on that date

Data is refreshed **daily at 00:00 UTC** and stored locally before upload to Tableau.

---

## 🧩 Tools & Tech Stack

* **Visualization:** Tableau Public
* **Data Handling:** CSV aggregation, date grouping
* **Dashboard Design:** stacked area charts, pie chart, crosstab heatmap
* **Presentation:** Google Slides (summary insights)

---

## 📌 Conclusions

* Categories **Entertainment** and **Music** dominated global trends.
* Regional differences were observed — e.g., **Education** in India and **Gaming** in Japan.
* The dashboard enables **daily self-service exploration** by ad managers.

---

## 💾 Repository Contents

```
data/
 └── trending_by_time.csv
docs/
 ├── Documentation_Project-Youtube_Trends.pdf
 ├── Presentation_Youtube_Trends.pdf
 └── README_data.md
```

---

## 🧭 How to Use

1. Download this repository.
2. Open the live dashboard link above.
3. Use the **filters** to explore trends by category, date, and region.
4. Read the **slides** for summarized insights per country.

