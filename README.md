# Lyft_Citi_Bike_Tableau
Creating worksheets, Dashboards, and Stories with Tableau

## Overview of the Analysis
* Uncovering insights about Citi Bike's ride-sharing program (powered by Lyft!).
* Using Tableau Public Server, available data on (url) for August, 2019 was downloaded and imported for analysis. Learning objectives about Tableau's program design, such as importing various filetypes, using and changing column datatypes, measures, dimensions, continuous vs. discrete values, filters, pages, marks, dashboard, and stories were covered.

### Links to my Tableau Public Profile and the NYC Citi Bike Tableau Presentation:
[link to profile](https://public.tableau.com/app/profile/derek.huggens)

[link to citi bike project](https://public.tableau.com/app/profile/derek.huggens/viz/CitiBikeDashboardStory/NYCCitiBikeStory)

## Results

Number of Rides<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/8ff1d8faee5d7a86963cec10665104626b15747b/README%20IMAGES/number_of_rides.png)<br>
The number of rides given in the Citi Bike NYC August, 2019 dataset.<br><br>
Customer Type<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/customer_type.png)<br>
A pie graph showing the ratio of short-term customers to long-term subscribers.<br><br>
Gender Breakdown<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/gender_breakdown.png)<br>
A pie graph showing the ratio of Unknown, Female, and Male gender users.<br><br>
August Peak Hours<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/aug_peak_hours.png)<br>
A horizontal bar graph showing hours in 24H format, highlighting most busy and least busy hours.<br><br>
Avg. Trip Duration by Age<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/avg_trip_duration.png)<br>
An area graph showing the relationship between age (by birth year) and average trip duration in minutes. See graph annotation.<br><br>
Bike ID Ride Count<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/bike_repairs.png)<br>
Horizontal bar graph of count of bike rides per bike ID (later reduced to top 10%). Helps identify types of use per bike.<br><br>
Avg. Trip Duration Per Bike (Bike Utilization)<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/bike_utilization.png)<br>
A sphere image that present average trip duration measurements detailed by the size of spheres with relevant bike ID details.<br><br>
Top Starting Locations<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_starting_locations.png)<br>
A map showing the top starting locations for bike rentals with varying color according to the count of rentals.<br><br>
Top Ending Locations<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_ending_locations.png)<br>
A map showing the top ending locations for bike rentals with varying color according to the count of rentals.<br><br>
Checkout Times for Users<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/checkout_times_users.png)<br>
Bike count records relationship to checkout times by 24H 00:00:00 format thanks to a int64 to datetime conversion within pandas and Jupyter Notebook.<br><br>
Checkout Times by Gender<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/checkout_times_gender.png)<br>
Bike count records relationship to checkout times by 24H 00:00:00 format with per gender comparison via color labeled lines.<br><br>
Trips by Weekday per Hour<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trips_by_weekday_per_hour.png)<br>
A heatmap showing the start time vs stop time relationship, colored by count of number of rides.<br><br>
Trips by Gender (Weekday per Hour)<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trips_by_gender_weekday_per_hour.png)<br>
A heatmap showing the start time vs stop time relationship, colored by count of number of rides and is filterable by gender.<br><br>
User Trips by Gender by Weekday<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/user_trips_gender_by_weekday.png)<br>
A heatmap showing the relationship between two types of users (customer and subscriber) as well as their corresponding genders, and when (by weekday) they are more or less actively renting bikes.<br><br>

## Summary
Three suggested visualizations for future analysis.

Starting locations with binned trip amounts. Using if, else-if, and, and then statments. Helpful to pinpoint the busiest starting location compared to the least busy.<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_starting_locations_specific.png)<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/8ff1d8faee5d7a86963cec10665104626b15747b/README%20IMAGES/top_starting_locations_specifi_calc.png)
<br><br>
Top 10% rented bikes based on ride count. Helpful to see if frequently rented bikes suffer differently than less rented, long duration rented bikes in regards to repairs.<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_10_percent_rented_bikes.png)<br><br>

Trip duration & ride count relationship. A graph to show that the bikes with the longest trip duration are not the most rented. Somewhat obvious relationship in that a bike that is rented for long durations cannot be rented to another user during that time. May be able use this information to market products to long distance riders (athletic wear/nutrition/hydration).<br>
![image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trip_duration_ride_count_relationship.png)<br><br>

