# What's the Weather Like?
![Latitude](https://upload.wikimedia.org/wikipedia/commons/thumb/5/56/World_map_longlat.svg/550px-World_map_longlat.svg.png)

## Challenge Instructions 
This project utilizes a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities. A Python script was created to visualize the weather of 500+ cities across the world of varying distance from the equator.

## WeatherPy
Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude. Then, perform a weather check on each of the cities using a series of successive API calls. Include a print log of each city as it's being processed with the city number and city name. Save a CSV of all retrieved data and a PNG image for each scatter plot.
- Create a series of scatter plots to showcase the following relationships:
  - Temperature (F) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/output_data/Fig1.png">
</p>

  - Humidity (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/output_data/Fig2.png">
</p>

  - Cloudiness (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/output_data/Fig3.png">
</p>

  - Wind Speed (mph) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/output_data/Fig4.png">
</p>

- Run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):
  - Northern Hemisphere - Temperature (F) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Northern_Temp_Lat.png" height="50%" width="50%">
</p>

  - Southern Hemisphere - Temperature (F) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Southern_Temp_Lat.png" height="50%" width="50%">
</p>

  - Northern Hemisphere - Humidity (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Northern_Humidity_Lat.png" height="50%" width="50%">
</p>

  - Southern Hemisphere - Humidity (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Southern_Humidity_Lat.png" height="50%" width="50%">
</p>

  - Northern Hemisphere - Cloudiness (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Northern_Cloud_Lat.png" height="50%" width="50%">
</p>

  - Southern Hemisphere - Cloudiness (%) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Southern_Cloud_Lat.png" height="50%" width="50%">
</p>

  - Northern Hemisphere - Wind Speed (mph) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Northern_Wind_Lat.png" height="50%" width="50%">
</p>

  - Southern Hemisphere - Wind Speed (mph) vs. Latitude
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Southern_Wind_Lat.png" height="50%" width="50%">
</p>

- To optimize the code, write a function that creates the linear regression plots

## VacationPy
Use jupyter-gmaps and the Google Places API to plan future vacations based on preferred weather conditions.
- Create a heat map that displays the humidity for every city from WeatherPy.
- Narrow down the DataFrame to find the ideal weather condition. For example:
  - A max temperature lower than 80 degrees but higher than 70
  - Wind speed less than 10 mph
  - Zero cloudiness
  - Humidity lower than 70 but higher than 40
  - Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/City_List.png" height="75%" width="75%">
</p>

- Using Google Places API to find the first hotel for each city located within 5000 meters of the filtered coordinates.
<p align="center">
  <img src="https://github.com/Jiuhe2020/python-api-challenge/blob/master/images/Hotel_List.png" height="75%" width="75%">
</p>

- Plot the hotels on top of the humidity heatmap with each pin containing the <b>Hotel Name</b>, <b>City</b> and <b>Country</b>

## List of Content
1. Weather.ipynb: using the OpenWeatherMap API to visualize the weather of over 500 cities across the world
2. VacationPy.ipynb: searching for the most ideal vacation destination(s) with preferred weather conditions

---
### Copyright
Jiuhe Zhu © 2020. All Rights Reserved.
