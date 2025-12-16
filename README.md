# Will the Customer Accept the Coupon?

This project analyzes survey data from an in‑vehicle coupon recommendation study to explore **which drivers accept or reject mobile coupons** for places like bars, coffee houses, and restaurants.

Link to notebook: https://github.com/gundaja/customer_coupon_acceptance/blob/main/coupon_analysis.ipynb

## Data and Tools

- Dataset: `coupons.csv` with user, trip, and coupon attributes (age, income, passenger, weather, time of day, coupon type, etc.).  
- Tools: Python, `pandas`, `matplotlib`, and `seaborn` for data cleaning, summarization, and visualization.  

## What the Notebook Does

- Cleans the data and handles missing values.  
- Calculates overall coupon acceptance rates (`Y = 1` vs. `Y = 0`). 
- Creates plots to compare acceptance across coupon types and customer segments (e.g., bar frequency, age, passenger type).  
- Includes a focused analysis of **bar coupons** plus one other coupon group.

## Key Insights & Recommendations

- Drivers who **frequently visit a venue** (bar, coffee house, or cheap restaurant) are more likely to accept coupons for that venue.  
- Bar coupons perform better for drivers who visit bars more than once a month and are **not driving with kids**.  
- Coupon campaigns should target customers based on visit frequency, time of day, and passenger type to increase acceptance rates.  

## Repository Contents

- `coupons.csv` – source data  
- `coupon_analysis.ipynb` – main analysis notebook  
- `README.md` – project summary (this file)
