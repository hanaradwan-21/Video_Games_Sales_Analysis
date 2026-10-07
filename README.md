# Video Games Sales Analysis

An interactive Power BI dashboard that explores global video game sales across platforms, genres, regions and critic scores, with a dedicated look at the PS4 and Xbox One generation.

**Tech stack:** Power BI Desktop · Power Query · DAX

---

## 1. Project Overview

The video game industry generates billions in revenue, but raw sales tables don't answer the questions that matter: *Which genres dominate? Which platforms lead? Do well-reviewed games actually sell more? How do North America, Europe and Japan differ?*

This project turns three sales datasets into a two-page dashboard that answers those questions through KPIs, trends and interactive filters.

## 2. Repository Structure

```
.
├── Video_Games_Sales_Analysis.pbix   # Power BI dashboard (2 pages)
├── images/                           # Dashboard screenshots
├── data/                             # Source datasets (not tracked, see Dataset section)
├── .gitignore
└── README.md
```

## 3. Dataset

The data model contains three tables:

| Table | Description |
|---|---|
| `Video_Games_Sales_as_at_22_Dec_2016` | Historical sales by game, platform, genre and region (NA, EU, JP, Other, Global), with critic scores and ESRB ratings |
| `PS4_GamesSales` | PlayStation 4 game sales, used for the Executive Summary page |
| `XboxOne_GameSales` | Xbox One game sales, used for platform comparison |

The datasets are not included in this repository because of their size. They are publicly available on Kaggle; download them and place the files in a local `data/` folder (ignored by Git).

## 4. Data Model & DAX Measures

Key measures built for the dashboard:

- **Total Global Sales**: total worldwide sales (millions of units)
- **Total NA Sales**: total North America sales
- **Total Games**: number of distinct titles
- **Avg Critic Score**: average critic rating

## 5. Dashboard Pages

### Page 1 – Executive Summary
- KPI cards: **Total Global Sales**, **Total NA Sales**, **Total Games**, **Avg Critic Score**
- Line chart: global sales trend by release year
- Bar chart: global sales by genre

### Page 2 – Platform & Regional Insights
- Donut chart: global sales share by platform
- Scatter plot: critic score vs. global sales, per game
- Clustered column chart: regional comparison (NA vs. EU vs. JP)
- Interactive slicers: **Genre** and **ESRB Rating**, which filter the whole page

## 6. Key Questions Answered

- Which genres and platforms account for the largest share of sales?
- How have sales evolved over the years?
- Does a higher critic score translate into higher sales?
- How do regional markets differ in what they buy?

## 7. How to Run

1. Download the datasets (see the Dataset section) and place them in `data/`.
2. Open `Video_Games_Sales_Analysis.pbix` in Power BI Desktop.
3. Go to **Transform data → Data source settings** and point each source to your local files.
4. Click **Refresh**.

## 8. Author

**Hana** – AI student focused on machine learning, data analysis and computer vision.
Feel free to connect on LinkedIn.
