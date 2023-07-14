# Bikesharing
## Table of Contents
- [Overview of the Analysis](#overview-of-the-analysis)
    - [Purpose](#purpose)
    - [About the Dataset](#about-the-dataset)
    - [Tools Used](#tools-used)
    - [Description](#description)
- [Results](#results)
    - [Overview of data](#Overview-of-data)
    - [Top starting and ending locations in NYC in August 2019](#Top-starting-and-ending-locations-in-NYC-in-August-2019)
    - [Bike Repairs](#Bike-Repairs)
    - [Checkout times for users](#Checkout-times-for-users)
    - [Checkout times by gender](#Checkout-times-by-gender)
    - [Trips by weekday for each hour](#Trips-by-weekday-for-each-hour)
    - [Trips by gender (weekday per hour)](#Trips-by-gender-(weekday-per-hour))
    - [User trips by gender by weekday](#User-trips-by-gender-by-weekday)
- [Summary](#summary)
- [Link to the Dashboard](#Link-to-the-Dashboard)
- [Contact Information](#contact-information)

## Overview of the Analysis
### Purpose:
The purpose of this analysis is to explore the NYC Citi Bike sharing data to help investors decide if starting a similar bikesharing program in another city would be worthwile.

### About the Dataset:
The dataset is the NYC Citi Bike data for August 2019, from the [Citi Bike System Data page](https://ride.citibikenyc.com/system-data).

### Tools Used:
- Tableau
- Python

The dashboard visualization has been created using Tableau, with data processing done in Python.

### Description:
The values in the Trip Duration column in the original dataset were changed to a datetime format, and the data loaded into a new DataFrame. The code is contained in the file [NYC_CitiBike](https://github.com/SohaT7/Bikesharing/blob/main/NYC_CitiBike.ipynb).

The fields contained within this dataset are as follows:

<img width="200" alt="image" src="https://github.com/SohaT7/Bikesharing/blob/main/Images/Datafields.png"> 

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
### Overview of data
Number of rides in the month of August are 2,344,224 in total. There are 443,865 short-term customers and 1,900,359 annual subscribers to the bike service. Peak hours for bike trips/rentals during the month of August are: 5 PM and 6 PM, followed by 8 AM and 9 AM.

![Overview of data](https://github.com/SohaT7/Bikesharing/blob/main/Images/Tableau_main.png)

### Top starting and ending locations in NYC in August 2019
The highest traffic locations for starting and ending points appear to be in Manhattan. The most popular locations are denoted by symbols which have a larger size and a darker-toned color. The maps below show the top starting locations and top ending locations respectively:

<img style="width:80%" alt="Map showing the Top Starting and Ending Locations" src="https://github.com/SohaT7/Bikesharing/blob/main/Images/ride_map.png">

### Bike Repairs
The tree map helps us visualize how often each bike is used, and which bikes are used most frequently. The bikes that are used most frequently will most probably be the ones that require repairs most often.

![Tree map showing Bike Usage Frequency](https://github.com/SohaT7/Bikesharing/blob/main/Images/BikeRepairs.png)

### Checkout times for users
Most of the bikes are checked out for around 40 minutes or less.

![Graph showing the Checkout times for users](https://github.com/SohaT7/Bikesharing/blob/main/Images/CheckoutTimesForUsers.png)

### Checkout times by gender
Graphs for all genders start to level around the 40 minutes mark, i.e. most bikes are checked out by all genders for 40 minutes or under. Most of these bikes are checked out by males, followed by females, and then others. 

![Graph showing Checkout times by gender](https://github.com/SohaT7/Bikesharing/blob/main/Images/CheckoutTimesByGender.png)

### Trips by weekday for each hour
During the weekdays, the checkout times are highest around 8 AM, 5 PM, and 6 PM. During the weekends, the checkout times are highest around 10 AM to 5 PM.

![Heat map showing Trips by weekday for each hour](https://github.com/SohaT7/Bikesharing/blob/main/Images/TripsByWeekday.png)

### Trips by gender (weekday per hour)
Checkouts are highest around 7 AM, 8 AM, and 5 to 6 PM during the weekdays, and are the highest for males.

![Heat map showing Trips by gender (weekday per hour)](https://github.com/SohaT7/Bikesharing/blob/main/Images/TripsByGender.png)

### User trips by gender by weekday
Annual subscribers appear to utilize bikes more than short-term customers. That said, male subscribers appear to use bikes more than females.

<img style="width:50%" alt="Heat map showing User trips by gender by weekday" src="https://github.com/SohaT7/Bikesharing/blob/main/Images/ride_breakdown.png">

## Summary
The annually subscribed users appear to use bikes more than the short-term customers. Males seem to be utilizing bikes more than females, followed by the other genders thereafter. The peak usage timings are in the morning (8 AM and 9 AM) and evening (5 PM and 6 PM). Most rentals are in Manhattan, and for 40 minutes or less. 

Some other visualizations that can be added are as follows:
- Stations by User Type: This can help determine if the tourists use the same stations as the annual subscribers/locals, and the frequency of usage. We can make use of longitude and latitude fields to generate a geographical map or station names to create a heat map.
- Traffic in each station: This can help gauge how much traffic that uses Citi Bikes passes through each station. We can use Station IDs to generate a tree map for this one. 
- Area by Gender type: This can help determine if there are some areas that are preferred by different genders, or all areas are equally preferred by all of them. We can use the latitude and longitude fields along with the gender field. 
- Area by trip duration: We can use latitude and longitude fields with the trip duration field, to determine if the bikers spend more time in certain areas than others. 

## Contact Information
Email: st.sohatariq@gmail.com
