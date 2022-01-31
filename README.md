# World_Weather_Analysis

## Overview of the Project
PlanMyTrip is a leading travel technology company that specializes in internet related services in the hotel and lodging industry.  Jack, who is the head of analysis for the user interface team, has asked for my assistance in collecting and presenting data for customers via the search page. This data can be filtered based on preferred travel criteria to find ideal hotel locations anywhere in the world.  Beta testers raved over the PlanMyTrip app, but made a recommendation to add a weather description to enhance the output.  Users will use input statements to filter for weather preferences that will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the user will choose four cities and create a travel itinerary.  Ultimately, using the Google Maps Directions API, a travel route between the four cities, with a marker layer map, will be available to the user.

### Resources
Data Source: WeatherPy_Database.csv; WeatherPy_vacation.csv

Code: Vacation_Search.ipynb; Vacation_Itinerary.ipynb

Software: Python 3.7.6, Pandas 1.3.5; Jupyter Notebook

## Weather Database Development

A weather database was developed by generating a list of 2000 random sets of latitudes and longitudes, then identifying the closest city to those coordinates.  An API call was made to https://openweathermap.org/ to determine the current weather data.

Specific data used for this application included:
* Latitude
* Longitude
* Maximum Temperature
* Percent Humidity
* Percent Cloudiness
* Wind Speed
* Current Weather

Here is a sample of the data that was collected:

![image](https://user-images.githubusercontent.com/94148420/151720453-912ccd8e-bd6d-4976-bc8a-e5b758ede24e.png)

### Statistal Analysis of Weather Parameters

A statatistical analysis was performed to determine the relationship between latitude and the following weather parameters:
* Maximum Temperature
* % Humidity
* % Cloudiness
* Wind Speed

![image](https://user-images.githubusercontent.com/94148420/151720697-7e71250f-a1a0-4e37-9b0b-a5be1eb1abfc.png)

![image](https://user-images.githubusercontent.com/94148420/151720717-e578e8ae-ccf0-4bd8-bbb9-d1ece13f9b6f.png)

![image](https://user-images.githubusercontent.com/94148420/151720734-1da9c4d9-e7fd-4c72-ba71-c44d6fff8dfb.png)

![image](https://user-images.githubusercontent.com/94148420/151720751-672a4b14-bbdf-4bde-baab-16db46d65d54.png)

In addition, a linear regression was performed comparing the Northern and Southern Hemispheres on the following weather parameters:
* Maximum Temperature
* % Humidity
* % Cloudiness
* Wind Speed


***Maximum Temperature***

![image](https://user-images.githubusercontent.com/94148420/151720920-17693df8-15fe-49b3-a8ff-13f295ec0e45.png)

![image](https://user-images.githubusercontent.com/94148420/151720929-101ab297-2475-4fe2-af91-38562dd4c4a5.png)


***Percent Humidity***

![image](https://user-images.githubusercontent.com/94148420/151720960-e62755cb-542e-4e7f-aa19-397ecf6c2d00.png)

![image](https://user-images.githubusercontent.com/94148420/151720976-b4763309-c2c5-454e-94ea-f5bd285dcc35.png)


***Percent Cloudiness***

![image](https://user-images.githubusercontent.com/94148420/151721009-7d038886-b58b-400e-ad28-c2df5ec1329d.png)


![image](https://user-images.githubusercontent.com/94148420/151721030-9e94411b-e7b5-476f-bb2c-f97400f04959.png)


***Wind Speed***

![image](https://user-images.githubusercontent.com/94148420/151721083-449f9984-57e5-4aca-b9eb-185869deb6d8.png)

![image](https://user-images.githubusercontent.com/94148420/151721105-7052e60d-fa59-4a5e-bf9f-62962fc25fdb.png)


## Vacation Search Based on User's Weather Preferences

By utilizing the functionality of the Jupyter Notebook's gmaps plugin, a user is then able to input weather preferences.  This information will provide data and facilitate a request to the Google Maps and Places API generating a marker layer map with pop-up markers displaying the following information:

* Hotel Name
* City
* Country
* Current Weather
* Maximum Temperature

![image](https://user-images.githubusercontent.com/94148420/151728068-57fadcd5-231c-4037-8dab-b5326b7adb78.png)


## Vacation Itinerary

The final two outputs of the PlanMyTrip app will display a vacation itinerary and city detail map using the Google Directions API with the user identifying four cities.  The examples below were four cities chosen by a user planning a trip to South Africa.  These maps show: 

1. A vacation itinerary
2. An city detail map with pop-ups that include:
      * Hotel Name
      * City
      * Country
      * Current Weather
      * Max Temp

![image](https://user-images.githubusercontent.com/94148420/151728383-5580127a-cedd-4f0f-9c67-3399126473e5.png)

![image](https://user-images.githubusercontent.com/94148420/151728876-048f03b1-3190-410f-90a0-35b4a186978c.png)


