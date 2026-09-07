# 🎵 Spotify Social Media Analytics for Strategic Branding

![Excel](https://img.shields.io/badge/Domain-Social_Media_Analytics-brightgreen)
![Tool](https://img.shields.io/badge/Tool-MS_Excel_/_Advanced_Pivot_Tables-blue)
![Data](https://img.shields.io/badge/Dataset-Spotify_Marketing_Data-1DB954)

## 📌 Business Overview & Problem Statement
Spotify operates across multiple digital channels (Instagram, Twitter, Facebook, YouTube) running targeted music campaigns and artist collaborations. The marketing team faced challenges in unifying performance metrics, evaluating campaign ROI, and understanding content engagement dynamics across platforms.

As a Data Analyst, I built an end-to-end **Social Media Intelligence Solution** in Microsoft Excel to evaluate performance, optimize platform spend, and deliver data-backed growth recommendations.

---

## 🛠️ Data Architecture & Workflow

The analytics framework processes 3 main data streams across multiple analytical modules:

1. **Posts Dataset:** 300+ entries tracking engagement metrics (Likes, Shares, Comments, Impressions, Reach, Clicks, Hashtags).
2. **Engagement Summary:** Weekly performance metrics tracking Ad Spend, Follower Growth, App Downloads, and Clicks.
3. **Campaign Metadata:** Strategic campaign timelines (e.g., ChillVibes, Wrapped 2024, IndieWave) and target objectives.

---

## 🔑 Key Analytics & Insights (Tasks Covered)

### 1. Data Preprocessing & Hygiene (Task 1)
* Standardized date/platform formatting and cleaned duplicated posts.
* Formatted numeric types (Likes, Impressions, Ad Spend) and split multi-hashtag columns into modular fields (`Hashtag 1`, `Hashtag 2`).

### 2. Engagement Dynamics (Task 2 & Task 4)
* Calculated custom **Engagement Rate (ER)** formula:  
  $$\text{Engagement Rate} = \frac{\text{Likes} + \text{Comments} + \text{Shares}}{\text{Impressions}}$$
* Identified top-performing content types and hashtag clusters (e.g., `#SoundtrackOfLife`, `#DiscoverWeekly`).

### 3. Platform & Campaign Performance (Task 3 & Task 5)
* Analyzed platform-wise return on engagement and content-type alignment.
* Evaluated **Campaign ROI** ($\text{Engagement} / \text{Ad Spend}$) to identify peak acquisition drivers.

### 4. Retention & Growth Trends (Task 6)
* Computed moving averages for net follower growth trends.
* Performed correlation analysis between **Ad Spend vs. App Downloads** & **Follower Growth**.

---

## 📊 Strategic Business Recommendations

1. **Content-Platform Fit:** Reallocate ad spend towards high-performing visual formats (Reels/Stories on Instagram & Twitter) which yield maximum Engagement Rate per impression.
2. **Campaign Optimization:** Scale top ROI campaigns like *ChillVibes* while adjusting underperforming promotional ad frequency.
3. **Hashtag Strategy:** Standardize high-conversion hashtag pairs (`#DiscoverWeekly`, `#NowPlaying`) to increase organic discovery.

---

## 📁 Repository Structure

```text
├── data/
│   ├── Task_1_Analysis.xlsx         # Preprocessed Data & Standardized Schemas
│   └── Task_2_to_Task_6.xlsx        # Complete Analytics Models, Pivots & Trend Analyses
└── README.md                        # Project Documentation
