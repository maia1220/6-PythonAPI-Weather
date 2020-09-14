# 6-PythonAPI-Weather


* For Nbviewer versions:

1. Weatherpy:
https://nbviewer.jupyter.org/github/maia1220/python-api-challenge/blob/master/weatherpy/WeatherPy-AQ.ipynb

2. Vacation-P1:
https://nbviewer.jupyter.org/github/maia1220/python-api-challenge/blob/master/vacationpy/VacationPy-Part1.ipynb


3. Vacation-P2: 
https://nbviewer.jupyter.org/github/maia1220/python-api-challenge/blob/master/vacationpy/VacationPy_Part2.ipynb



## Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a [simple Python library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across world cities.

My first step is to create a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

My second step is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, the linear regression will show any relationships between the two variables.


## Part II - VacationPy

I worked with the weather data to plan future vacations and used jupyter-gmaps and the Google Places API for this part of the analysis.

* Create a heat map that displays the humidity for every city from the part I.

* Narrow down the DataFrame to find my ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.
