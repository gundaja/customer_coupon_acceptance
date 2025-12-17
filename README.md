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

Bar coupon related findings:
- Acceptance overall was 41% while non-acceptance stood at 59%. 
- Drivers who **frequently visit a venue** are more likely to accept coupons (~76%)  as compare to the less frequent visitors (~37%) for that venue. 
- Frequent elderly bar visitors are much more likely to accept bar coupons (69%) than less frequent young visitors, who show considerably lower acceptance (33%).
- Frequent elderly bar visitors who do not work in farming, fishing, or forestry show the highest coupon acceptance rate (71%), whereas less frequent young visitors employed in farming, fishing, or forestry display much lower acceptance (29%).
- Bar coupons perform better for drivers who visit bars more than once a month and are **not driving with kids**.  

Coffee coupon related findings:
- About 49.9% of the coffee coupons were accepted.
- Highest acceptance is in the under 21 group at about 69.7%, while over 50 show the lowest at about 42.0%.
- Lower and mid-incomes accept slightly more often: "Less than $12500" (~55.2%), "$12500–$24999" (~54.0%), "$37500–$49999" (~54.2%), and "$87500–$99999" (~55.7%).
- Acceptance is very simlar by gender: females about 49.2% and males about 50.6%.

Recommendations:
- Target bar coupons to drivers who already visit bars at least once or twice per month, are not driving with kids, and are not headed to work.
- Send coffee house or low‑cost restaurant coupons to frequent visitors during appropriate times of day (for example, morning or mid‑afternoon) and near typical destinations like work or school.
- Use customer visit frequency, passenger type, and trip context as key features for deciding when and to whom to deliver coupons, in order to improve overall acceptance rates.


## Repository Contents

- `coupons.csv` – source data  
- `coupon_analysis.ipynb` – main analysis notebook  
- `README.md` – project summary (this file)
