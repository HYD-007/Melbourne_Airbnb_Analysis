# Melbourne Airbnb Market Analysis

**Status:** In progress

## Business question
Where in Melbourne should a new short-stay investor buy, and at what nightly price?

## Data
- Source: [Inside Airbnb](https://insideairbnb.com/get-the-data/), Melbourne listings snapshot ([snapshot date])
- 25,715 listings, 90 columns

## Initial findings (data audit)
- 15 columns are completely empty in this snapshot and were dropped.
- 6,711 listings (26%) have no price, likely inactive; excluded from pricing analysis.
- Price is stored as text ("$80.00") and needs converting before analysis.
- Neighbourhoods are council areas (LGAs), not suburbs. City of Melbourne holds ~33% of listings.
- 74% of listings are entire homes/apartments; the analysis focuses on these as the product relevant to an investor.

## Plan
1. Clean and filter data (Python, pandas)
2. Median price and estimated revenue by council area (SQL: CTEs, window functions)
3. Interactive dashboard
4. Business recommendations memo

## Tools
Python (pandas), SQL, Google Colab
