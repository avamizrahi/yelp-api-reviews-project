# Yelp Restaurant & California Population Analysis

## Overview
End-to-end data pipeline project analyzing the relationship between 
California city population and Yelp restaurant ratings. Integrates 
live API data with census data via a MySQL database hosted on AWS RDS.

## Data Sources
- Yelp Fusion API — restaurant business and review data for CA cities
- California Demographics CSV — population by city (2022 census data)
- Data not included in repo due to API credentials and file size

## Tech Stack
Python, SQL, MySQL (AWS RDS), Jupyter Notebook, pandas, seaborn, 
matplotlib, yelpapi

## Data Schema
Three tables in MySQL database:
- `businesses` — Yelp business info (rating, location, price, etc.)
- `reviews` — individual reviews linked to businesses and city
- `CA_population_data` — city-level population data

## Key Queries & Analysis
1. Most populated city in California (Los Angeles — 3.88M)
2. Average Yelp rating per city using GROUP BY aggregation
3. Distribution of ratings across Italian restaurants (pie chart)
4. Correlation between city population and average restaurant rating
5. Distribution of businesses across cities

## Key Findings
- No significant correlation between city population and restaurant 
  ratings (r ≈ 0)
- 65% of Italian restaurants rated 5 stars; most fall in the 3.4–4.5 range
- Mammoth Lakes accounted for 30% of sampled businesses by city

## Tools & Libraries
Python, pandas, MySQL Connector, yelpapi, matplotlib, seaborn, 
Google Colab, AWS RDS
