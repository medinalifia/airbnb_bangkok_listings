This repository contains an analysis of Airbnb listings in Bangkok from 2012 to 2022. The goal is to clean and explore the dataset, identify data issues (missing names, duplicates, and unusual pricing), visualize distributions and correlations, and derive business insights and recommendations regarding pricing, host performance, and listing quality.

Work performed:

- Data cleaning & standardization
- Exploratory Data Analysis (histograms, boxplots, heatmaps)
- Outlier detection & price fairness analysis
- Host-level analysis (top hosts, hosts with high availability + few reviews)
- Time series of reviews (2012–2022)
- Revenue estimation (simple proxy)
- Produced a cleaned dataset and multiple visualizations

📚 Data dictionary (summary)

Key columns used in the analysis:

id — unique listing id

name — accommodation name (may be missing)

host_id, host_name — host identifiers and names

neighbourhood, latitude, longitude — location info

room_type — [Entire home/apt / Private room / Shared room / Hotel room]

price — listing price (THB) — treated as price per night in analysis

minimum_nights — minimum stay (nights)

number_of_reviews, reviews_per_month, last_review — review metrics

calculated_host_listings_count — number of listings owned by host in dataset

availability_365 — calendar availability (days/year)

Derived columns: price_per_night, estimated_revenue (price × number_of_reviews), last_review (Year)
