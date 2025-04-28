🚻 Public Toilet Cleanliness Analysis - NYC
This project analyzes 311 Service Requests related to dirty public restrooms across New York City (NYC) by integrating service complaint data with public restroom location data. We apply spatial, statistical, and regression analysis to uncover restroom accessibility gaps and highlight areas needing improvement.

📂 Repository Structure
toilet_analysis.Rmd — R Markdown containing all analysis steps, code, and explanations

toilet_analysis.pdf — Final compiled report (ready to view)

Public_Restrooms_20250427.csv — Cleaned NYC public restrooms dataset

README.md — Project overview (this file)

⚡ Note: .RData file is not needed to reproduce the project.

⚡ External Large File
Due to GitHub's 100MB limit, the 311 complaints dataset is available separately via Google Drive:

📥 Download 311_Service_Requests_from_2021_to_Present_20250427.csv

After downloading, place the file into your project folder before running the .Rmd.

🛠 How to Run
Clone this GitHub repository locally.

Download the large CSV from the above link and move it into your project folder.

Open Public_Toilet_Analysis.Rproj in RStudio.

Open and knit toilet_analysis.Rmd to generate your HTML/PDF reports.

📊 Key Analysis Performed
Data Cleaning: Refined 311 complaints and restroom datasets.

Exploratory Data Analysis (EDA): Complaint volume patterns by time, borough, and restroom availability.

Spatial Analysis: Calculated nearest restroom distance for every complaint using Haversine distance.

Statistical Modeling:

Multiple Linear Regression: Investigated how Time Group, Restroom Availability, and Borough affect distance to restrooms.

ANOVA and Tukey's HSD Tests: Compared restroom accessibility across boroughs.

Mapping Visualizations:

Complaint hotspot mapping.

Overlay of complaints with public restroom locations.

Heatmaps of complaint densities.

📋 Findings Summary
Complaints are highest during Morning and Afternoon hours.

Restroom availability drops significantly during Evening and Late Night.

Manhattan has the best public restroom accessibility; Staten Island has the worst.

Significant differences in restroom distances were confirmed between boroughs using ANOVA and Tukey HSD tests.

💡 Recommendations
Extend operating hours of public restrooms, especially in the Evening and Late Night.

Prioritize adding new restrooms or maintaining existing ones in underserved areas like Staten Island and parts of Queens.

Focus on areas where complaint hotspots are not well-covered by existing restrooms.

📚 Acknowledgments
NYC Open Data Portal — 311 Service Requests

NYC Open Data Portal — Public Restrooms Dataset

✅ Project Completed: April 2025
👨‍💻 Author: Prashanth Vadityavath | Jeet

