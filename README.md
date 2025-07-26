Uber Fares Dataset Analysis
Names: Rukundo Espoir 27678


Project Overview
This project aims to analyze Uber fare data to uncover trends, patterns, and actionable insights. The analysis leverages Python for data processing and Power BI for interactive visualization.

Goal: To provide data-driven insights for optimizing pricing strategies and operations within a ride-sharing context.

Deliverables:

Interactive Power BI Dashboard (.pbix file)

Detailed Report (this presentation deck)

Cleaned CSV dataset (uber_features.csv)

GitHub Repository (containing code and resources)

Screenshots of key analysis steps and dashboard

Dataset Description
Source: Uber Fares Dataset from Kaggle

Key Variables: fare_amount, pickup_datetime, pickup_longitude, pickup_latitude, dropoff_longitude, dropoff_latitude, passenger_count, etc.

Methodology
1. Data Cleaning
Checked for and handled missing values (null entries were dropped).

Converted data types (e.g., pickup_datetime to datetime objects).

Identified and removed outliers.

2. Exploratory Data Analysis (EDA)
Examined data structure, data types, unique values, and missingness.

Generated summary statistics (mean, median, std, IQR) for fare_amount and distance.

Identified outliers and invalid coordinate entries.

3. Feature Engineering
Extracted new features from pickup_datetime: hour, day, month, and weekday.

Saved the enhanced dataframe as uber_features.csv for Power BI import.

4. Power BI – Data Import & Dashboard Design
Imported the cleaned and engineered uber_features.csv into Power BI.

Dashboard Design Principles:

Clear layout: KPIs at the top, trends and distribution charts in the center, and interactive filters at the bottom.

Interactive slicers for month, weekday, and hour.

Consistent formatting with a defined theme, colors, and fonts.

Key Insights
Peak Demand: Rides consistently peak during morning (7-9 AM) and evening (5-7 PM) commuting hours.

Weekday Focus: Ride frequency is highest mid-week (Tuesday-Thursday), with a noticeable drop on Fridays and weekends.

Seasonal Decline: A significant decline in both ride count and total fare amounts is observed in later months (e.g., November-December), contrasting with higher activity earlier in the year.

Average Fare: The overall average fare per trip distance is approximately $11.36.

Total Rides: The dataset comprises 9,802 unique fare amounts/rides.

Recommendations
Based on the analysis, the following recommendations are proposed to optimize operations and revenue:

Optimize Peak Supply: Incentivize drivers during peak morning and evening hours to maximize availability, reduce wait times, and capture more rides.

Boost Off-Peak/Weekend Demand: Implement targeted promotions and explore partnerships for off-peak hours and weekends to stimulate demand during slower periods.

Mitigate Seasonal Decline: Develop specific year-end marketing campaigns or offerings (e.g., holiday travel, shopping promotions, airport transfers) to proactively address the observed revenue drops in months 11-12.

Refine Pricing: Analyze weekday/distance fare variations to identify optimal pricing strategies. Consider dynamic models adapting to real-time supply/demand for competitive and optimal revenue.

Improve Dashboard Clarity: Clarify top-level metric definitions and aggregation methods (e.g., "Count of fare_amount") for enhanced consistency and interpretability.

Segment Customers: If feasible, segment users (e.g., commuters, leisure, business) to analyze distinct ride patterns, informing tailored marketing and service development.

Conclusion
The Power BI dashboard effectively visualizes fare distribution, time-based trends, and fare-distance relationships. These insights are crucial for informed decision-making in pricing strategies and operational planning. Future improvements could involve integrating external factors like weather and event data for a more comprehensive analysis.
