# Video Game Market Analysis

## Overview

This project delivers a **data-driven strategic framework** for video game publishers by analyzing historical global sales across genres, platforms, and regions. The analysis identifies high-growth market segments and consumer preferences to inform game development and marketing investment decisions.

**Key Focus:**
- Identify top-performing genres and platforms globally
- Uncover regional consumer preference differences
- Determine factors driving commercial success in gaming
- Provide actionable business recommendations

---

## Dataset

**Source:** Video game sales data spanning 1980–2020

**Size:** 16,598 game records with 11 variables

**Variables:**
- **Game Characteristics:** Name, Platform, Genre, Publisher
- **Market Performance:** Global Sales, Regional Sales (North America, Europe, Japan, Other)
- **Temporal Data:** Release Year
- **Competitive Data:** Publisher Rankings, Platform Dominance
<img width="781" height="358" alt="image" src="https://github.com/user-attachments/assets/72ce7ff9-0598-421e-b086-db48a983fe0d" />

**Data Cleaning:**
- Removed 271 entries (1.63%) with missing release years
- Converted sales columns to numeric format
- Minimal data loss with negligible impact on analysis
<img width="849" height="484" alt="image" src="https://github.com/user-attachments/assets/0071171e-17d0-444c-b9ae-0f28efbf6e70" />

---

## Tools & Technologies

- **Language:** R
- **Libraries:** 
  - `tidyverse` (data manipulation & visualization)
  - `ggplot2` (advanced graphics)
  - `dplyr` (data wrangling)
  - `readr` (data import)
  - `scales` (axis formatting)

---

## Methodology

### 1. **Data Preprocessing**
   - Filtered missing values
   - Converted data types
   - Created temporal period groupings (5-year intervals)

### 2. **Exploratory Data Analysis (EDA)**
   - Summary statistics before/after filtering
   - Identified top performers by genre, platform, and region
   - Analyzed temporal trends and lifecycle patterns

### 3. **Visualization Techniques**
   - **Heat Maps:** Genre performance trends across time periods
   - **Facet Line Charts:** Platform-specific sales lifecycles
   - **Faceted Bar Charts:** Regional preference comparisons
   - **Bubble Charts:** Publisher efficiency metrics

---

## Key Insights & Findings

### Genre Performance
- **Action, Shooter, and Sports** genres drive long-term commercial success
- Action games peaked at **583M USD** (2010–2014)
- Shooter genre experienced rapid growth post-2000, reaching **378M USD** by 2014
- Legacy genres (Puzzle, Strategy, Adventure) show diminishing commercial viability
<img width="918" height="609" alt="image" src="https://github.com/user-attachments/assets/c6416ed4-17a2-4e9e-867d-8231539047a6" />

### Platform Dynamics
- **Console Lifecycle:** PS2, PS3, Wii, DS follow predictable **5–7-year bell-curve patterns**
  - Rapid uptake → Sharp peak → Decline (generational turnover)
- **PC Platform:** Uniquely stable and hardware-independent, providing **long-tail revenue**
- Peak industry sales occurred around **2008** across all major platforms
<img width="1182" height="661" alt="image" src="https://github.com/user-attachments/assets/53086256-ce5a-405a-b5d0-22f097b29ef1" />

### Regional Preferences
- **North America & Europe:** Synchronized markets dominated by Action, Sports, and Shooter games (Xbox 360, PS3)
- **Japan:** Distinct ecosystem with overwhelming preference for Role-Playing games (300M+ USD) and Nintendo DS
- Western markets drive majority of global revenue
- Japan requires culturally tailored, niche strategies
<img width="966" height="638" alt="image" src="https://github.com/user-attachments/assets/34b2f0b0-349c-4928-a1f5-4189137af90b" />

### Publisher Efficiency
- **Quality over Quantity:** High average sales per game correlates with higher success rates
- **Nintendo** emerges as the global efficiency leader (highest avg sales/game, lean release volume)
- Competitors like Activision, EA, Sony, Take-Two achieve high volume but with lower per-game yields
- Focus on **focused franchises** reduces development risk and improves risk-adjusted returns
<img width="1109" height="777" alt="image" src="https://github.com/user-attachments/assets/12f3f8bd-0868-49a6-ad42-5b9278337e50" />

---

## Business Recommendations

### 1. **Optimize Development Pipeline**
   - Reduce low-yield, speculative releases
   - Adopt quality-over-quantity approach
   - Prioritize high-potential franchises (following Nintendo's model)

### 2. **Implement Region-Specific Strategies**
   - **Western Markets:** High-budget Action, Sports, and Shooter games on major consoles
   - **Japan:** Niche focus on Role-Playing games and Nintendo DS platform support

### 3. **Expand PC Portfolio**
   - Leverage stable, hardware-independent ecosystem
   - Build long-term revenue streams
   - Support product longevity

---

## Conclusions

The video game market success is driven by **platform lifecycle timing**, **genre consistency**, **regional preferences**, and importantly, **publisher efficiency**. The data demonstrates that commercial longevity requires strategic focus on quality titles aligned with regional demands rather than high-volume releases. Publishers adopting efficiency-driven models achieve superior risk-adjusted returns.

**Future Enhancement:** Predictive modeling (e.g., Naive Bayes classification) can further optimize development and marketing investment decisions.

---

## Project Structure

```
├── README.md
├── data/
│   └── video_games_sales.csv
├── scripts/
│   └── analysis.R
└── visualizations/
    ├── genre_heatmap.png
    ├── platform_trends.png
    ├── regional_preferences.png
    └── publisher_efficiency.png
```


---

## References

- Knaflic, C.N. (2025). *Storytelling with Data: A Data Visualization Guide for Business Professionals*
- Schwabish, J. (2021). *Better Data Visualizations*
- García, S., Luengo, J., & Herrera, F. (2015). *Data Preprocessing in Data Mining*
