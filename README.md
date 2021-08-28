## Part I - WeatherPy
I have created a Python script to visualise the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I have utilised a [simple Python library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api), to create a representative model of weather across world cities.

I have created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Next, I have run linear regression on each relationship. This time separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

## Part II - VacationPy

For this part I have used jupyter-gmaps and the Google Places API.

* Heat map that displays the humidity for every city from Part I.

* Narrowed down the DataFrame to find the ideal weather conditions. For example:

  * A max temperature lower than 80 degrees but higher than 70.

  * Wind speed less than 10 mph.

  * Zero cloudiness.

* Use Google Places API to find the first hotel for each city located within 5km of the coordinates.

* Plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

 ![hotel_map](https://user-images.githubusercontent.com/80393628/131208414-61ac020f-885f-4c60-af15-84eee8b84c82.png)
