# Python API  - Linear Regressions and Scatter Plots



## Part I - WeatherPy

Here I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I  utilized  a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), to create a representative model of weather across world cities.



The first was to create a series of scatter plots to showcase relationships with Temperature vs Latitude, Humiditiy vs Latitude, Cloudiness vs Latitude and Wind speed vs Latitude.

* Temperature (F) vs. Latitude
 ![Weatherpy](output_data/Fig1.png)
* Humidity (%) vs. Latitude
  ![Humidity](output_data/Fig2.png)
* Cloudiness (%) vs. Latitude
  ![Cloudiness](output_data/Fig3.png)
* Wind Speed (mph) vs. Latitude
 ![windSpeed](output_data/Fig4.png)

Secondly I ran linear regression on each relationship. Then separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude![Screen Shot 2022-01-13 at 4 48 00 AM](https://user-images.githubusercontent.com/33403205/149308110-d2fd3fa8-e036-4427-9ae8-ae0e680e7ed0.png)

* Southern Hemisphere - Temperature (F) vs. Latitude![Screen Shot 2022-01-13 at 4 48 05 AM](https://user-images.githubusercontent.com/33403205/149307792-fe0f9e1f-918a-46cf-abd6-4554e94ec943.png)

* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude![Screen Shot 2022-01-13 at 4 48 11 AM](https://user-images.githubusercontent.com/33403205/149308015-b776cfc2-920f-4501-b879-6c9cf76e27f3.png)

* Northern Hemisphere - Cloudiness (%) vs. Latitude![Screen Shot 2022-01-13 at 4 48 16 AM](https://user-images.githubusercontent.com/33403205/149307969-278bc4a9-9ce5-4cf8-8ba8-62afe24c8d84.png)

* Southern Hemisphere - Cloudiness (%) vs. Latitude![Screen Shot 2022-01-13 at 4 48 32 AM](https://user-images.githubusercontent.com/33403205/149307843-ae9a2aeb-ec4f-439a-9ba8-e647a125fcce.png)

* Northern Hemisphere - Wind Speed (mph) vs. Latitude![Screen Shot 2022-01-13 at 4 48 35 AM](https://user-images.githubusercontent.com/33403205/149307925-6172ee99-c0aa-47b7-a8bd-732f8abb569f.png)

* Southern Hemisphere - Wind Speed (mph) vs. Latitude![Screen Shot 2022-01-13 at 4 48 38 AM](https://user-images.githubusercontent.com/33403205/149307630-2b111fe9-7940-4088-b6b4-ab85837a59ba.png)




In addition:

*  500 unique (non-repeat) cities were selected based on latitude and longitude.
*  weather checks on each of the cities were performed using a series of successive API calls.
* Includes a print log of each city as it's being processed with the city number and city name.
* a saved  CSV of all retrieved data and a PNG image for each scatter plot is within the repository.

### Part II - VacationPy


* Created a heat map that displays the humidity for every city from Part I.

  ![heatmap](Images/heatmap.png)

* Utilized Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

  ![hotel map](Images/hotel_map.png)

As final considerations:

* analysis where created using Jupyter notebook via Matplotlib or Pandas plotting libraries.




