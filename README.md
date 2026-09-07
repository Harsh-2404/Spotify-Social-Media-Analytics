# 🎵 Spotify Social Media Analytics & Strategic Branding Solution

![Excel](https://img.shields.io/badge/Tool-Microsoft_Excel-1DB954?style=for-the-badge&logo=microsoft-excel)
![Domain](https://img.shields.io/badge/Domain-Social_Media_&_Brand_Analytics-blue?style=for-the-badge)
![Analytics](https://img.shields.io/badge/Focus-Campaign_ROI_&_Growth_Attribution-darkgreen?style=for-the-badge)

## 📌 Executive Summary & Business Context
Spotify operates promotional campaigns across multiple social platforms (**Instagram, Twitter, YouTube, Facebook**) to drive listener acquisition, feature adoption (Podcasts, Wrapped), and brand loyalty. 

As a **Data Analyst**, I built an end-to-end **Social Media Intelligence Solution in Microsoft Excel**. This model unifies post-level interactions, weekly advertising spend, audience retention dynamics, and campaign metadata to solve core business challenges around platform spend allocation, campaign ROI, and content performance.

---

## 🛠️ Data Architecture & Schemas

The analytics model processes three core datasets structured in Microsoft Excel:

1. **Posts Dataset (300 Post Entries):** Tracks `Post ID`, `Platform`, `Date`, `Content Type`, `Likes`, `Shares`, `Comments`, `Impressions`, `Reach`, `Clicks`, `Hashtags`, and `Campaign_Name`.
2. **Engagement Summary Dataset (200 Weekly Records):** Tracks weekly performance including `Week_Start_Date`, `Platform`, `New_Followers`, `Unfollows`, `Total_Followers`, `Engagement_Rate`, `Ad_Spend`, and `Net Follower Gain`.
3. **Campaign Metadata Dataset:** Strategic timelines, budgets ($160k–$225k), objectives, and primary hashtags for campaigns: **ChillVibes**, **IndieWave**, **SummerBeats**, and **Wrapped2024**.

---

## 🔑 Technical Tasks & Analytics Implementation

### 🧹 Task 1: Data Preprocessing & Hygiene
* **De-duplication:** Identified and eliminated duplicate post entries across platforms.
* **Schema Standardization:** Normalized date formats, unified platform string names, and formatted numerical values (`Likes`, `Impressions`, `Ad_Spend`).
* **Hashtag Parsing:** Extracted multi-hashtag strings into structured modular fields (`Hashtag 1`, `Hashtag 2`) for granular frequency mapping.

### 📊 Task 2: Engagement Analysis & Post-Level Benchmarking
* **Custom Metric Formulation:** Calculated post-level **Engagement Rate (ER)**:
  $$\text{Engagement Rate} = \frac{\text{Likes} + \text{Comments} + \text{Shares}}{\text{Impressions}}$$
* **Top Performers:** Extracted Top 10 viral posts sorted by ER (top post achieved **26.06% ER** on Twitter).
* **Pivot Models:** Built aggregations for total interaction counts (`Likes`, `Shares`, `Comments`) segmented by Content Type (`Story`, `Text`, `Reel`, `Video`) and Platform.
  <img width="1248" height="475" alt="image" src="https://github.com/user-attachments/assets/26e43124-189e-4fda-a4fd-04cb3bb3f948" />


### 🌐 Task 3: Platform Performance & Spend Optimization
* **Platform Benchmarking:** Compared average engagement rates across platforms (**Twitter: ~6.89%**, **YouTube: ~6.72%**, **Instagram: ~6.46%**).
  <img width="757" height="355" alt="chart1" src="https://github.com/user-attachments/assets/2ae77cae-8ff3-4dc7-bc3e-3daaecd513bf" />

* **Growth Tracking:** Analyzed weekly follower acquisition trends and percentage growth rates across platforms.
* **Platform Decision:** Validated continuing a **multi-platform strategy** with channel-specific budget reallocations based on performance data.

### 🏷️ Task 4: Hashtag & Content Strategy
* **Hashtag Master Index (`Hashtag_Master`):** Ranked top-performing hashtags by post frequency and average engagement rate (`#NowPlaying`: 143 occurrences, ~9.86% ER; `#SoundtrackOfLife`: 109 occurrences, ~9.44% ER).
  <img width="932" height="433" alt="image" src="https://github.com/user-attachments/assets/2cdaea52-09e3-4baf-8d55-97d0078b1302" />

* **Format-Platform Matrix:** Evaluated optimal combinations, identifying high conversion rates for visual stories and text-based updates.

### 🎯 Task 5: Campaign Effectiveness & ROI Evaluation
* **Campaign Aggregations:** Computed total and average impressions, likes, and clicks across major campaigns (*ChillVibes*, *IndieWave*, *SummerBeats*, *Wrapped2024*).
* **Campaign Uplift:** Quantified engagement uplift during active campaign windows vs. pre-campaign baseline levels (e.g., *ChillVibes* drove an **8.60% engagement uplift**).
* **ROI Measurement:** Evaluated engagement yield per advertising dollar spent ($\text{Engagement} / \text{Ad Spend}$).
  <img width="1441" height="402" alt="image" src="https://github.com/user-attachments/assets/62163c49-3d81-4396-aa69-4c7afd21214b" />


### 📉 Task 6: Audience Retention, Trends & Loyalty
* **Retention Analysis:** Derived weekly `Net Follower Gain` ($\text{New Followers} - \text{Unfollows}$) and identified peak gain weeks.
  <img width="1426" height="450" alt="image" src="https://github.com/user-attachments/assets/c3f68db2-72d6-4d86-9636-86dac6349444" />

* **Moving Averages & Correlation:** Implemented trend lines and evaluated correlation between `Ad_Spend` allocations and net audience growth.

---

## 📊 Key Strategic Business Insights & Recommendations

1. **Budget Reallocation:** Shift a higher percentage of top-of-funnel ad spend toward **Twitter & Instagram Stories/Posts**, which consistently yield maximum engagement per impression.
2. **Hashtag Optimization:** Mandate the usage of high-converting hashtag clusters (`#NowPlaying`, `#SoundtrackOfLife`, `#DiscoverWeekly`) across all organic content.
3. **Campaign Scaling:** Scale high-ROI campaigns like **ChillVibes** and **Wrapped2024**, which demonstrate strong engagement uplift relative to acquisition costs.

---

## 📁 Repository Navigation

```text
├── data/
│   ├── Task_1_Analysis.xlsx         # Cleaned Datasets & Schema Standardizations
│   └── Task_2_to_Task_6.xlsx        # Complete Excel Analysis Workbook (Pivots, Formulas, Tasks 2-6)
└── README.md                        # Professional Portfolio Documentation
