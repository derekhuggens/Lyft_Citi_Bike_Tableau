# Lyft_Citi_Bike_Tableau
Creating worksheets, Dashboards, and Stories with Tableau

## Overview of the Analysis
* Uncovering insights about Citi Bike's ride-sharing program (powered by Lyft!).
* Using Tableau Public Server, available data on (url) for August, 2019 was downloaded and imported for analysis. Learning objectives about Tableau's program design, such as importing various filetypes, using and changing column datatypes, measures, dimensions, continuous vs. discrete values, filters, pages, marks, dashboard, and stories were covered.

### Links to my Tableau Public Profile and the NYC Citi Bike Tableau Presentation:
[link to profile](https://public.tableau.com/app/profile/derek.huggens)

[link to citi bike project](https://public.tableau.com/app/profile/derek.huggens/viz/CitiBikeDashboardStory/NYCCitiBikeStory)

## Results

Number of Rides
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/number_of_rides.png)
* The number of rides given in the Citi Bike NYC August, 2019 dataset.
Customer Type
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/customer_type.png)
* A pie graph showing the ratio of short-term customers to long-term subscribers.
Gender Breakdown
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/gender_breakdown.png)
* A pie graph showing the ratio of Unknown, Female, and Male gender users.
August Peak Hours
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/aug_peak_hours.png)
* A horizontal bar graph showing hours in 24H format, highlighting most busy and least busy hours
Avg. Trip Duration by Age
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/avg_trip_duration.png)
* An area graph showing the relationship between age (by birth year) and average trip duration in minutes. See graph annotation.
Bike ID Ride Count
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/bike_repairs.png)
* Horizontal bar graph of count of bike rides per bike ID (later reduced to top 10%). Helps identify types of use per bike.
Avg. Trip Duration Per Bike (Bike Utilization)
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/bike_utilization.png)
* A sphere image that present average trip duration measurements detailed by the size of spheres with relevant bike ID details.
Top Starting Locations
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_starting_locations.png)
* A map showing the top starting locations for bike rentals with varying color according to the count of rentals.
Top Ending Locations
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_ending_locations.png)
* A map showing the top ending locations for bike rentals with varying color according to the count of rentals.
Checkout Times for Users
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/checkout_times_users.png)
* Bike count records relationship to checkout times by 24H 00:00:00 format thanks to a int64 to datetime conversion within pandas and Jupyter Notebook.
Checkout Times by Gender
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/checkout_times_gender.png)
* Bike count records relationship to checkout times by 24H 00:00:00 format with per gender comparison via color labeled lines.
Trips by Weekday per Hour
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trips_by_weekday_per_hour.png)
* A heatmap showing the start time vs stop time relationship, colored by count of number of rides.
Trips by Gender (Weekday per Hour)
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trips_by_gender_weekday_per_hour.png)
* A heatmap showing the start time vs stop time relationship, colored by count of number of rides and is filterable by gender.
User Trips by Gender by Weekday
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/user_trips_gender_by_weekday.png)
* A heatmap showing the relationship between two types of users (customer and subscriber) as well as their corresponding genders, and when (by weekday) they are more or less actively renting bikes.

## Summary
*  Three suggested visualizations for future analysis.

Starting locations with binned trip amounts. Using if, else-if, and, and then statments. Helpful to pinpoint the busiest starting location compared to the least busy.
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_starting_locations_specific.png)

Top 10% rented bikes based on ride count. Helpful to see if frequently rented bikes suffer differently than less rented, long duration rented bikes in regards to repairs.
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/top_10_percent_rented_bikes.png)

Trip duration & ride count relationship. A graph to show that the bikes with the longest trip duration are not the most rented. Somewhat obvious relationship in that a bike that is rented for long durations cannot be rented to another user during that time. May be able use this information to market products to long distance riders (athletic wear/nutrition/hydration).
[image](https://github.com/derekhuggens/Lyft_Citi_Bike_Tableau/blob/eb7695636f24c4972bbdefe5f3658368d1a9f26d/README%20IMAGES/trip_duration_ride_count_relationship.png)

