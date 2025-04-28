---

# NYC Public Restroom Analysis 🚻

> **Spatial and statistical analysis of NYC public restroom complaints using 311 data and restroom datasets.**

---

# 📑 Table of Contents
- [Project Overview](#-project-overview)
- [Data Sources](#-data-sources)
- [Analysis Workflow](#-analysis-workflow)
- [Key Findings](#-key-findings)
- [Download Data](#-download-data)
- [How to Reproduce](#-how-to-reproduce)
- [Project Structure](#-project-structure)
- [Final Notes](#-final-notes)

---

# 📂 Project Overview
This project analyzes the relationship between public restroom availability and 311 cleanliness-related complaints in New York City.  
It combines geospatial mapping, statistical testing, and visualization to better understand restroom accessibility and related citizen concerns.

---

# 📚 Data Sources
- **NYC Open Data 311 Service Requests (2021 - Present)**
- **NYC Parks and Libraries Restroom Locations Dataset**

> *(Note: Large datasets are available via [Google Drive Link](#-download-data).)*

---

# 🛠️ Analysis Workflow
The analysis was conducted in structured steps:

1. **Data Cleaning**
   - Filter operational restrooms
   - Extract and standardize operating hours
   - Assign time groups (Morning, Afternoon, Evening, Late Night)

2. **Complaints Data Preparation**
   - Filter 311 complaints related to public restrooms
   - Assign complaint timestamps into time groups

3. **Geospatial Distance Calculation**
   - Calculate distance from each complaint to nearest public restroom

4. **Exploratory Data Analysis (EDA)**
   - Distance distributions across time groups
   - Borough-wise restroom availability analysis

5. **Statistical Modeling**
   - Multiple Linear Regression
   - ANOVA Tests
   - Tukey's HSD Post-Hoc Analysis

6. **Geospatial Mapping**
   - Hotspot identification
   - Overlay of restroom locations and complaint density

7. **Conclusions & Recommendations**
   - Insights to improve restroom coverage and maintenance in NYC

---

# 📈 Key Findings
- Complaints during **Morning** and **Late Night** periods show slightly higher restroom inaccessibility.
- **Staten Island** has the highest average distance to public restrooms among boroughs.
- **Regression results** show borough and restroom availability significantly influence complaint distances.
- **Heatmaps** revealed specific complaint hotspots requiring better restroom availability.

---

# 📥 Download Data
You can download the full 311 service request dataset here:

🔗 [311_Service_Requests_from_2021_to_Present_20250427.csv (Google Drive Link)](https://drive.google.com/drive/folders/1CrIuw_c6kXsgvKGLi9GucV4uVyHpsyU1?usp=drive_link)

> *(Large file excluded from GitHub repository due to 100MB limit.)*

---

# 🚀 How to Reproduce

1. **Clone this Repository**
   ```bash
   git clone https://github.com/vadityavathprashanth/NYC_Restroom_Analysis.git
   ```

2. **Install Required R Packages**
   ```r
   install.packages(c("dplyr", "tidyverse", "lubridate", "geosphere", "broom", "ggplot2", "tidyr", "forcats"))
   ```

3. **Open and Knit**
   - Open `toilet_analysis.Rmd` in RStudio.
   - Knit the document to generate the final report PDF.

---

# 📊 Project Structure

```bash
Public_Toilet_Analysis/
├── Data/                     # (Optional) Data directory
├── toilet_analysis.Rmd        # RMarkdown analysis
├── toilet_analysis.pdf        # Final report (generated)
├── README.md                  # Project overview (this file)
└── .gitignore
```

---

# 📋 Final Notes
- **Project Completed:** April 2025
- **Potential Future Work:** Adding time-series prediction of restroom usage trends based on complaints over seasons.

---

# 🌟 Thank you for visiting the project!

> Feel free to ⭐️ star the repo if you find it interesting!

---

