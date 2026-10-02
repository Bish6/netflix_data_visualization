Netflix Data Visualization Dashboard (Power BI)

An interactive Power BI dashboard that explores the Netflix catalog: what type of content it holds, how ratings are distributed, which countries produce the most titles, and how content additions have changed over time.

📌 Project Overview

Netflix hosts thousands of movies and TV shows, but the raw data says little on its own. This project cleans the Netflix titles dataset and turns it into a one-page dashboard that answers questions such as:

How many titles are on Netflix, and what is the Movie vs. TV Show split?
Which age ratings dominate the catalog?
Which countries contribute the most content?
When did Netflix grow its library fastest?
Which release years are most represented?

📊 Key Metrics (KPIs)
Metric	        Value
Total Titles  	~8.8K (8,807)
Total Movies	  ~6.1K
Total TV Shows	~2.7K
Movie %       	~70%

🖼️ Dashboard Components
Visual	Type	Purpose
KPI Cards	Card	Total Titles, Movie %, Total Movies, Total TV Shows
Content Type	Slicer	Filter by Movie / TV Show
Rating	Slicer	Filter by rating (G, NC-17, NR, PG, ...)
Year Added	Range slicer	Filter by the year content was added
Netflix Titles by Rating	Bar chart	Distribution of titles across rating categories
Netflix Content Added Over Time	Line chart	Yearly trend of titles added
Titles by Country	Bar chart	Top content-producing countries
Netflix Content by Type	Donut chart	Movie vs. TV Show share
Movies vs TV Shows Added Over Time	Stacked column chart	Yearly additions split by type
Netflix Titles by Release Year	Column chart	Number of titles by original release year

🔍 Key Insights
Movies dominate: about 70% of the catalog is movies and 30% is TV shows.
Mature content leads: TV-MA (3,207 titles) and TV-14 (2,160 titles) are the two largest rating categories.
United States leads by a wide margin (about 2.8K titles), followed by India and the United Kingdom.
Content additions peaked around 2019 (about 2.0K titles added in a year), followed by a decline in later years.
Most titles were released in the late 2010s, with the release-year peak around 2018 (1,147 titles).
Data quality note: "Unknown" is one of the top country values, meaning a notable share of titles has no country recorded.
🛠️ Tools & Technologies
Power BI Desktop for data modelling, DAX measures and visualization
DAX for KPI measures (Total Titles, Total Movies, Total TV Shows, Movie %)
Dataset: Netflix Movies and TV Shows (netflix_titles), cleaned into netflix_titles_CLEANED
🧹 Data Preparation

Describe the cleaning you did here, for example:

Handled missing values in country, rating, director, cast
Converted date_added to a date type and extracted Date Added Year
Standardized text columns and removed duplicates
Replaced missing countries with "Unknown"

📁 Repository Structure
├── Netflix_Data_Visualization_project.pbix   # Power BI report file
├── assets/
│   └── dashboard-preview.png                 # Dashboard screenshot
└── README.md

🚀 How to Use
Clone or download this repository.
Open Netflix_Data_Visualization_project.pbix in Power BI Desktop (free).
Use the Content Type, Rating and Year Added slicers to filter every chart on the page.
Hover over any chart to see exact values.
🔮 Future Improvements
Add a Genre / listed_in breakdown
Add a Director and Cast analysis page
Add a map visual for country-level content
Publish to Power BI Service and embed a live link
