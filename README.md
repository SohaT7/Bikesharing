# Bikesharing
## Overview of the Analysis
### Purpose:
The purpose of this analysis is to explore the NYC Citi Bike sharing data to convince investors to start a similar program in the town of Des Moine.

### About the Dataset:
The dataset is the NYC Citi Bike data for August 2019, from the [Citi Bike System Data page](https://ride.citibikenyc.com/system-data).

### Tools Used:
The dashboard visualization has been created using Tableau, with some modifications to the original dataset made using Python.

### Description:
The Trip Duration in the original dataset was changed to a datetime format and the data loaded into a new DataFrame. The fields contained wihtin this dataset are as follows:

![Data Fields](https://github.com/SohaT7/Bikesharing/blob/main/Images/Datafields.png)

Using this new dataset, several visualizations were then created in Tableau:
- Number of rides
- Users breakdown by subscription type and gender
- August peak hours
- Top starting locations in NYC in August 2019
- Top ending locations in NYC in August 2019
- Bike Repairs
- Checkout times for users
- Checkout times by gender
- Trips by weekday for each hour
- Trips by gender (weekday per hour)
- User trips by gender by weekday

## Results
### (a) Overview of data:
Number of rides in the month of August are 2,344,224 in total. The proportion of short-term customers of the bike service to its annual subscribers is 443,865 customers to 1,900,359 subscribers. Peak hours for bike trips/rentals during the month of August are: 5 PM and 6 PM, followed by 8 AM and 9 AM.

![Overview of data](https://github.com/SohaT7/Bikesharing/blob/main/Images/Overview.png)

### (b) Top starting and ending locations in NYC in August 2019
The highest traffic locations for starting and ending points appear to be in Manhattan. The most popular locations are denoted by symbols which have a larger size and a darker-toned color, as can be seen in the maps below, which show the top starting locations and top ending locations respectively:

![Map showing the Top Starting Locations](https://github.com/SohaT7/Bikesharing/blob/main/Images/TopStartingLocations.png)

![Map showing the Top Ending Locations](https://github.com/SohaT7/Bikesharing/blob/main/Images/TopEndingLocations.png)

### (c) Bike Repairs
The tree map helps us visualize how often a bike is used and which among all are used most frequently. The latter will most probably require repairs most often.

![Tree map showing Bike Usage Frequency]()

### (d) Checkout times for users
Most of the bikes are checked out for around 40 minutes or less.

![Graph showing the Checkout times for users]()

### (e) Checkout times by gender
Graphs for all genders start to level around the 40 minutes mark, i.e. most bikes are checked by all genders for 40 minutes or under. Most of these bikes are checkout by males, followed by females, and then others. 

![Graph showing Checkout times by gender]()

### (f) Trips by weekday for each hour
During the weekdays, the checkout times are highest around 8 AM, 5 PM, and 6 PM. During the weekends, the checkout times are highest around 10 AM to 5 PM.

![Heat map showing Trips by weekday for each hour]()

### (g) Trips by gender (weekday per hour)
Checkouts are highest around 7 AM, 8 AM, and 5 to 6 PM during the weekdays, with them being the highest for males.

![Heat map showing Trips by gender (weekday per hour)]()

### (h) User trips by gender by weekday
Annual subscribers appear to utilize bikes more than short-term customers. That said, male subscribers appear to use bikes more than females.

![Heat map showing User trips by gender by weekday]()

## Summary
The annually subscribed users appear to use bikes more than the short-term customers. Males seem to be utilizing bikes more than females, followed by the other genders thereafter. The peak usage timings are in the morning (8 AM and 9 AM) and evening (5 PM and 6 PM). Most rentals are in Manhattan, and for 40 minutes or less. 
Some other visualization that can be added are:
(a) Stations by User Type: This can help us figure if tourists use some stations/areas more or different than the annual subscribers/locals. We can make use of longitude and latitude fields to generate a geographical map or station names to create a heat map.
(b) Traffic in each station: This can help gauge how much traffic that uses Citi Bikes passes by through each station. We can use Station IDs to generate a tree map for this one. 
(c) Area by Gender type: This can help us determine if there are some areas that are preferred by different genders, or all areas are equally preferred by all of them. We can use the latitude and longitude fields alogn with the gender field. 
(d) Area by trip duration: We can use latitude and longitude fields with the trip duration field, to determine if the bikers spend more time in certain areas than others. 

### Link to Dashboard:
[Click here to be directed to the dashboard!](https://public.tableau.com/app/profile/sturr/viz/Book_bikesharing/NYCStory)

## Contact Information
Email: st.sohatariq@gmail.com
