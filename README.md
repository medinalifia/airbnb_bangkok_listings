This repository contains an analysis of Airbnb listings in Bangkok from 2012 to 2022. The goal is to clean and explore the dataset, identify data issues (missing names, duplicates, and unusual pricing), visualize distributions and correlations, and derive business insights and recommendations regarding pricing, host performance, and listing quality.

Work performed:

- Data cleaning & standardization
- Exploratory Data Analysis (histograms, boxplots, heatmaps)
- Outlier detection & price fairness analysis
- Host-level analysis (top hosts, hosts with high availability + few reviews)
- Time series of reviews (2012–2022)
- Revenue estimation (simple proxy)
- Produced a cleaned dataset and multiple visualizations

In addition to the core analysis, I also prepared the following documents for better understanding:
- 🎥 Video of the presentation (https://drive.google.com/file/d/1rn9PebpHsOUFHZVOGA7xzfxW6Krkk2xY/view?usp=sharing)
- 📓 Jupyter Notebook containing all data cleaning, analysis, and visualizations in detail
- 📊 Presentation slides (PPT) summarizing key insights and recommendations
- 🌐 Interactive Tableau Dashboard (https://public.tableau.com/views/MedinaAlifiaJuniarto-FixAirbnbListingsBangkok-Capstone2/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

📚 Data dictionary

Key columns used in the analysis:

1) id — unique listing id
2) name — accommodation name (may be missing)
3) host_id, host_name — host identifiers and names
4) neighbourhood, latitude, longitude — location info
5) room_type — [Entire home/apt / Private room / Shared room / Hotel room]
6) price — listing price (THB) — treated as price per night in analysis
7) minimum_nights — minimum stay (nights)
8) number_of_reviews, reviews_per_month, last_review — review metrics
9) calculated_host_listings_count — number of listings owned by host in dataset
10) availability_365 — calendar availability (days/year)
11) derived columns: price_per_night, estimated_revenue (price × number_of_reviews), last_review (Year)
