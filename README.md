# Uber Fares Dataset Analysis  
*Names:* Rukundo Espoir 27678  

---

## Project Overview  
This project aims to analyze Uber fare data to uncover trends, patterns, and actionable insights. The analysis leverages *Python* for data processing and *Power BI* for interactive visualization.

### Goal:  
To provide data-driven insights for optimizing pricing strategies and operations within a ride-sharing context.

### Deliverables:
- Interactive Power BI Dashboard (.pbix file)  
- Detailed Report (this presentation deck)  
- Cleaned CSV dataset (uber_features.csv)  
- GitHub Repository (containing code and resources)  
- Screenshots of key analysis steps and dashboard  

---

## Dataset Description  
*Source:* Uber Fares Dataset from Kaggle

*Key Variables:*  
fare_amount, pickup_datetime, pickup_longitude, pickup_latitude, dropoff_longitude, dropoff_latitude, passenger_count, etc.

---

## Methodology  

### Data Cleaning  
- Checked for and handled missing values (null entries were dropped).  
![Missing Values](./Missing%20Values.PNG)  
- Converted data types (e.g., pickup_datetime to datetime objects).  
- Identified and removed outliers.

### Exploratory Data Analysis (EDA)  
- Examined data structure, data types, unique values, and missingness.  
![Exploratory Data Analysis](./Exploratory%20Data%20Analysis.PNG)  
- Generated summary statistics (mean, median, std, IQR) for fare_amount and distance.  
- Identified outliers and invalid coordinate entries.

### Feature Engineering  
- Extracted new features from pickup_datetime: hour, day, month, and weekday.  
![Dara Engineering](./Dara%20engeeniring.png)  
- Saved the enhanced dataframe as uber_features.csv for Power BI import.

---

## Power BI – Data Import & Dashboard Design  
- Imported the cleaned and engineered uber_features.csv into Power BI.  
![Export to CSV](./Export%20to%20csv.PNG)  

### Dashboard Design Principles:  
- *Clear layout:* KPIs at the top, trends and distribution charts in the center, and interactive filters at the bottom.  
![Dashboard Overview](./Dashboard%20overview.png)  
- *Interactive slicers* for month, weekday, and hour.  
- *Consistent formatting* with a defined theme, colors, and fonts.

---

## Key Insights  

- *Peak Demand:*  
Rides consistently peak during morning (7-9 AM) and evening (5-7 PM) commuting hours.  
![Fare vs Hour](./fare%20vs%20Hour.png)  

- *Weekday Focus:*  
Ride frequency is highest mid-week (Tuesday-Thursday), with a noticeable drop on Fridays and weekends.  
![Fare vs Weekday](./Fare%20vs%20weekday.png)  

- *Seasonal Decline:*  
A significant decline in both ride count and total fare amounts is observed in later months (e.g., November-December), contrasting with higher activity earlier in the year.  
![Fare vs Month](./Fare%20vs%20Month.png)  
![Sum of Month vs Fare](./sum%20of%20month%20vs%20fare(bins).png)  

- *Average Fare:*  
The overall average fare per trip distance is approximately *$11.36*.  
![Avg Fare vs Weekday and Trip Distance](./avg%20fare%20vs%20weekday%20and%20trip%20distance.png)

- *Total Rides:*  
The dataset comprises *9,802* unique fare amounts/rides.

---

## Recommendations  

1. *Optimize Peak Supply:*  
Incentivize drivers during peak morning and evening hours to maximize availability, reduce wait times, and capture more rides.

2. *Boost Off-Peak/Weekend Demand:*  
Implement targeted promotions and explore partnerships for off-peak hours and weekends to stimulate demand during slower periods.

3. *Mitigate Seasonal Decline:*  
Develop specific year-end marketing campaigns or offerings (e.g., holiday travel, shopping promotions, airport transfers) to proactively address the observed revenue drops in months 11–12.

4. *Refine Pricing:*  
Analyze weekday/distance fare variations to identify optimal pricing strategies. Consider dynamic models adapting to real-time supply/demand for competitive and optimal revenue.  
![Fare vs Hour Line Chart](./fare%20vs%20hour%20line%20chart.png)

5. *Improve Dashboard Clarity:*  
Clarify top-level metric definitions and aggregation methods (e.g., "Count of fare_amount") for enhanced consistency and interpretability.

6. *Segment Customers:*  
If feasible, segment users (e.g., commuters, leisure, business) to analyze distinct ride patterns, informing tailored marketing and service development.

---

## Conclusion  

The Power BI dashboard effectively visualizes fare distribution, time-based trends, and fare-distance relationships. These insights are crucial for informed decision-making in pricing strategies and operational planning.

*Future improvements* could involve integrating external factors like *weather* and *event data* for a more comprehensive analysis.
