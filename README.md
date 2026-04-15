Case Study: Cyclistic Bike-Share Analysis

Author: Andre Siopa
LinkedIn: www.linkedin.com/in/andré-siopa-5a9b91324

Tools Used

Python (Pandas, Matplotlib, Seaborn), Google Colab, Google Drive

Executive Summary

Cyclistic, a prominent bike-share program, aims to increase profitability by converting casual riders into annual members.

This analysis of 12 months of historical trip data reveals clear behavioral differences between user types.

Key Insight:

Casual riders primarily use bikes for leisure and sightseeing, especially on weekends.
Annual members use bikes consistently for daily commuting, particularly in business and industrial areas.

![Comparison of Member vs Casual Usage](bar_graph.png)

Business Task

Primary Question:
How do annual members and casual riders use Cyclistic bikes differently?

Goal:
Provide data-driven recommendations to support marketing strategies that increase membership conversions.

Data Process

Data Ingestion & Cleaning:
-Processed large datasets (>100MB per file) using Python (Pandas) in Google Colab
-Merged 12 monthly datasets into a single DataFrame using glob and pd.concat
-Removed duplicate records
-Cleaned column names using .strip()
-Standardized missing values using "N/A"

Data Transformation:
-Converted started_at and ended_at into datetime format
-Created new features:
   ride_length (minutes)
  day_of_week
-Removed invalid trips (negative or zero duration)

Key Insights

Usage Patterns:

-Members show stable usage Monday–Friday
-Casual riders spike significantly on weekends
-Weekend casual usage nearly matches member volume

Duration & Location:

Casual Riders:
-Longer rides
-Popular in tourist and sightseeing areas

Annual Members:
-Shorter, efficient rides
-Concentrated in business and industrial districts


Recommendations:

-Targeted Weekend Promotions
Introduce weekend or seasonal membership plans for casual riders
-Industrial Hub Campaigns
Promote memberships in commuter-heavy locations
-Incentivized Conversion
Offer discounts for casual users who reach ride thresholds
