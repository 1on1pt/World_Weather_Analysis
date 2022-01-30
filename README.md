# World_Weather_Analysis

## Overview of the Project
PlanMyTrip is a leading travel technology company that specializes in internet related services in the hotel and lodging industry.  Jack, who is the head of analysis for the user interface team, has asked for my assistance in collecting and presenting data for customers via the search page. This data can be filtered based on preferred travel criteria to find ideal hotel locations anywhere in the world.  Beta testers raved over the PlanMyTrip app, but had made recommendations to add a weather description to the weather data that had been collected.  Beta testers will use input statements to filter for weather preferences that will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities and create a travel itinerary.  Ultimately, using the Google Maps Directions API, a travel route between the four cities, with a marker layer map, will be available to the user.

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

## Vacation Search

## Vacation Itinerary
