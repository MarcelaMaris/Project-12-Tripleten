# 📊 Project Documentation — YouTube Trending Videos Analysis

## 🧠 Part 1 – Technical Requirements Specification

### 1. Project Objective
The purpose of this project is to build a **visual and interactive dashboard**, published on **Tableau Public**, to help advertising managers (Melanie and Ashok) automate and quickly answer the following key questions:

- Which video categories were trending last week?  
- How were these categories distributed across different regions?  
- Which categories were especially popular in the United States?  

---

### 2. End Users
The dashboard will be used by the company’s **video advertising planning managers**, who require **clear and dynamic visualisations** for daily analytical use.

---

### 3. Frequency of Use
The dashboard will be accessed **at least once per day** as part of the routine decision-making process.

---

### 4. Data Used
The data source is the file **`trending_by_time.csv`**, an aggregated table stored in the **YouTube** database.

**Dataset fields:**
- `record_id`: unique row identifier  
- `region`: country or geographical region (e.g. Japan, France)  
- `trending_date`: date when the video appeared in the trending section  
- `category_title`: video category (e.g. Education, Film)  
- `videos_count`: number of trending videos for that day, country, and category  

Data is updated **every 24 hours**, at **midnight UTC**.

---

### 5. Dashboard Content and Structure
The dashboard follows the visual prototype defined during the project design phase.  
It is divided into **three main sections**:

#### 🟦 Upper Section
- Dashboard title and description  
- Date filter  
- Country filter  

#### 🟨 Middle Section (Main Charts)
- **Chart 1: “Trend History” (Absolute Values)**  
  - Type: Stacked area chart  
  - X-axis: `trending_date`  
  - Y-axis: `videos_count`  
  - Colour: `category_title`  
  - **Purpose:** show the total number of trending videos per category over time.  

- **Chart 2: “Trending Videos by Country” (Relative Values)**  
  - Type: Pie chart  
  - **Purpose:** display the percentage distribution of trending videos across the selected countries.

#### 🟩 Lower Section
- **Chart 3: “Trend History (%)”**  
  - Type: 100% stacked area chart  
  - Calculation: percentage of total per day using *Quick Table Calculation*  
  - **Purpose:** show the proportion of each category in the total of trending videos per date.  

- **Chart 4: “Trending Videos by Country and Category” Table**  
  - Type: Crosstab with visual highlighting (*heatmap table*)  
  - Columns: `region`  
  - Rows: `category_title`  
  - Cells: sum of `videos_count`  
  - **Note:** cells are colour-coded by value to facilitate visual comparison.  

---

### 6. Grouping Parameters
Data are grouped by:
- Trending date (`trending_date`)  
- Video category (`category_title`)  
- Country or region (`region`)

---

### 7. Interactive Controls
The dashboard includes two main filters:
- **Date filter**  
- **Country filter**

Both filters are **applied simultaneously** to all visualisations.

---

### 8. Chart Importance
All charts and visual elements are **equally important**.  
The layout must be **balanced, intuitive, and functional**, enabling multiple analytical perspectives from the same dataset.

---

### 9. Technical Considerations
- The dashboard is built **locally** in **Tableau Public** using `trending_by_time.csv`.  
- It is **published publicly** on Tableau Public.  
- All charts must be properly linked to **global filters**.  
- The final structure follows the layout of the approved **project visual prototype**.  

---

## ⚙️ Part 2 – Building the Dashboard

The dashboard was developed using **Tableau Public**, based on the dataset **`trending_by_time.csv`**.  
Below are the main implementation highlights:

---

### 1. Dashboard Access
**Tableau Public:**  
[https://public.tableau.com/app/profile/marcela.stephanie.pereira.maris1628/viz/YoutubeTreendingDashboard-final/Dashboard1](https://public.tableau.com/app/profile/marcela.stephanie.pereira.maris1628/viz/YoutubeTreendingDashboard-final/Dashboard1)

---

### 2. Results Presentation
**Slides with analysis and managerial insights:**  
[**Open YouTube Trending Dashboard Presentation (OneDrive)**](https://1drv.ms/b/c/d1aeda57ea1dab69/ETe6SLqfANVPtnPp9PAoVTABSbvMgP2WEDA1WBingSMKIA?e=0Y2jAV)

---

### 3. Implemented Functionalities
- Interactive **date and country filters** applied to all charts.  
- **Custom tooltips** across all visuals to enhance data readability.  
- **Consistent colours per category** for easy comparison.  
- Properly labelled **titles and axes**.  
- **Three-block layout** (top, middle, bottom) following the design prototype.  

---

### 4. Visualisation Types
- Stacked area charts (absolute and percentage values)  
- Pie chart (share by country)  
- Crosstab with heatmap highlighting  

---

### 5. Key Insights
- The most recurrent global categories are **Entertainment** and **Music**.  
- Countries such as **India** and **the United States** show strong concentration in these categories.  
- **Japan** and **Russia** exhibit greater diversity in trending categories.  
- **Comedy** stands out in **France** and **Japan**, but not as a dominant trend elsewhere.  

---

### 6. Validation
The dashboard was tested in different browsers and is **publicly accessible**.  
All filters and interactions were validated to ensure **consistency, accuracy, and smooth navigation**.

---

## ✅ Project Details
**Author:** Marcela Maris  
**Course:** Data Analytics – TripleTen  
**Sprint:** 12  
**Date:** 02/07/2025
