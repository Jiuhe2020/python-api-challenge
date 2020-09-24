# What's the Weather Like?
## Challenge Instructions 
This project utilizes a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities. A Python script was created to visualize the weather of 500+ cities across the world of varying distance from the equator.

## WeatherPy
Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude. Then, perform a weather check on each of the cities using a series of successive API calls. Include a print log of each city as it's being processed with the city number and city name. Save a CSV of all retrieved data and a PNG image for each scatter plot.
- Create a series of scatter plots to showcase the following relationships:
  - Temperature (F) vs. Latitude
  - Humidity (%) vs. Latitude
  - Cloudiness (%) vs. Latitude
  - Wind Speed (mph) vs. Latitude
- Run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
  - Northern Hemisphere - Temperature (F) vs. Latitude
  - Southern Hemisphere - Temperature (F) vs. Latitude
  - Northern Hemisphere - Humidity (%) vs. Latitude
  - Southern Hemisphere - Humidity (%) vs. Latitude
  - Northern Hemisphere - Cloudiness (%) vs. Latitude
  - Southern Hemisphere - Cloudiness (%) vs. Latitude
  - Northern Hemisphere - Wind Speed (mph) vs. Latitude
  - Southern Hemisphere - Wind Speed (mph) vs. Latitude
 - To optimize the code, write a function that creates the linear regression plots.
## VacationPy

## List of Files
1. Weather.ipynb: using the OpenWeatherMap API to visualize the weather of over 500 cities across the world
2. VacationPy.ipynb: searching for the most ideal vacation destination(s) with preferred weather

---
### Copyright
Jiuhe Zhu © 2020. All Rights Reserved.
