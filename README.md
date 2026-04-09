Case Study: Cyclistic Bike-Share Analysis
Author: Andre Siopa

Tools Used: Python (Pandas, Matplotlib, Seaborn), Google Colab, Google Drive

Executive Summary
Cyclistic, a prominent bike-share program, seeks to maximize its profitability by converting casual riders into long-term annual members. As a Data Analyst, I analyzed 12 months of historical trip data to identify the behavioral differences between these two groups.

Key Finding: Casual riders primarily use the service for leisure and sightseeing on weekends, while members utilize the service for consistent daily commuting in industrial and business districts.

Business Task
Primary Question: How do annual members and casual riders use Cyclistic bikes differently?

Goal: Provide data-driven recommendations to help the marketing team design strategies to increase membership conversions.

Data Process 
1. Data Ingestion & Cleaning
Due to the large scale of the dataset (exceeding 100MB per file), I utilized Python and the Pandas library within Google Colab for efficient processing.

Consolidation: Merged 12 individual monthly spreadsheets into one master DataFrame using glob and pd.concat.

Quality Control: Removed exact duplicate entries and utilized strip() to remove leading/trailing white spaces in column headers.

Null Handling: Standardized missing values by filling them with "N/A" to maintain dataset integrity.

2. Data Transformation
To enable deep analysis, I performed the following engineering steps:

Type Casting: Converted started_at and ended_at strings into datetime objects.

Calculated Fields: Created a ride_length column (in minutes) and a day_of_week column to identify temporal trends.

Data Validation: Filtered out "ghost" entries (trips with negative or zero durations).

Key Insights & Analysis

My analysis revealed that while Member usage remains high and stable throughout the work week (Monday–Friday), Casual ridership spikes dramatically on Saturdays and Sundays. On weekends, casual ridership volume nearly equals that of annual members.

Duration & Destination
Casual Riders: Averaged longer trip durations, frequently starting and ending near tourist attractions and sightseeing areas.

Annual Members: Exhibited shorter, more efficient trip durations, primarily centered around industrial and business districts.

Recommendations
Targeted Weekend Promotions: Introduce "Weekend Only" or "Seasonal Pass" memberships specifically targeted at users frequenting sightseeing stations.

Industrial Hub Campaigns: Deploy digital marketing at industrial-area stations to highlight the cost-effectiveness of annual memberships for daily commuters.

Incentivized Conversion: Offer a "First Month Discount" for casual riders who reach a specific trip threshold during peak weekend hours.
