# python_api_Weather
weather and Vacation API
## Part 1: WeatherPy OpenWeatherMap API
In this deliverable, We need to create a Python script to visualize the weather of over 500 cities of varying distances from the equator using the citipy Python library Links to an external site., the OpenWeatherMap API Links to an external site., and using our problem-solving skills to create a representative model of weather across cities.
To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

### Steps 1: Created Plots to Showcase the Relationship Between Weather Variables and Latitude:
To fulfill the first requirement, we use the OpenWeatherMap API to retrieve weather data from the cities list. Next, We created a series of scatter plots to showcase the following relationships:

*Latitude vs. Temperature <br>
Latitude vs. Humidity<br>
Latitude vs. Cloudiness<br>
Latitude vs. Wind Speed <br>*

---

![Fig1](https://github.com/AVI-1213/python_api_challenge/assets/156638175/ba12b363-9ec5-48c5-a7ac-7d5924cb2d9c)

![Fig2](https://github.com/AVI-1213/python_api_challenge/assets/156638175/8be9e8c8-9adb-4e5a-a306-f025299371c8)

![Fig3](https://github.com/AVI-1213/python_api_challenge/assets/156638175/8334e9d2-a34c-40d7-9494-b313c8d5b7e1)

![Fig4](https://github.com/AVI-1213/python_api_challenge/assets/156638175/91619d4e-f96e-4952-ae58-f4e73343df9a)

---
#### Steps 2: Compute Linear Regression for Each Relationship

#### To fulfill the second requirement, we computed the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 
#### Next, created a series of scatter plots including the linear regression line, the model's formula, and the r values as you can see in the following image: 
----

![temp](https://github.com/AVI-1213/python_api_challenge/assets/156638175/90e9738d-1068-4760-91c7-31ab6c949dd0)

![stemp](https://github.com/AVI-1213/python_api_challenge/assets/156638175/389499f1-de7a-4717-8914-e2b34ecc55f0)

**Discussion about the linear relationship:** <br>
##### Nothern Hemisphere <br>
*The negative correlation coefficient (r-value: -0.85) between maximum temperature and latitude in the northern hemisphere suggests a strong linear relationship, As latitude increases (moving northwards), maximum temperatures decreases. This shows that regions farther from the equator experience cooler temperatures.*

##### Southern Hemisphere 
*With r-value of 0.73 in the southern hemisphere, there exists a moderate positive linear relationship between maximum temperature and latitude. it shows area closer to equator having higer temprature.*

![nhumidity](https://github.com/AVI-1213/python_api_challenge/assets/156638175/b1387313-a057-4f4f-86a1-7b03d16d5413)
![shumid](https://github.com/AVI-1213/python_api_challenge/assets/156638175/3e92eacd-2ffd-434b-8d87-38d5069d0076) <br>

*With r-values of 0.28 for the northern hemisphere and 0.27 for the southern hemisphere, the correlation between humidity and latitude appears to be weak in both hemispheres. This shows that latitude not by itself is a strong predictor of humidity levels. Other factors likely have higher impact on humidity levels.*

![ncloud](https://github.com/AVI-1213/python_api_challenge/assets/156638175/2e6a445b-ad0a-4436-8727-c3cef9954a4b)
![scloud](https://github.com/AVI-1213/python_api_challenge/assets/156638175/4cd98f59-25e8-4f1d-ad39-1750edf857f2) <br>

*With r-values of 0.18 for the northern hemisphere and 0.13 for the southern hemisphere, the correlation between cloudiness and latitude is quite weak in both hemispheres. This suggests latitude by itself not be a strong predictor of cloudiness levels.*

![nwind](https://github.com/AVI-1213/python_api_challenge/assets/156638175/0feb17ba-a72a-4912-a6f1-417236a46da1)
![swind](https://github.com/AVI-1213/python_api_challenge/assets/156638175/09576a02-e740-4324-a4be-7410487c2157)

**Discussion about the linear relationship:**<br>
*With r-value of approximately -0.11 for the northern hemisphere and -0.42 for the southern hemisphere, the correlation between wind speed and latitude is weak. In the northern hemisphere, there seems to be a very slight negative correlation, while in the southern hemisphere, the negative correlation is slightly stronger. but overall both correlations are quite weak, indicating that latitude alone may not be a reliable predictor of wind speed.*

----
## Part 2: VacationPy

In this deliverable, We use weather data , Jupyter notebooks, the geoViews Python library, and the Geoapify API.
Our main tasks will be to use the Geoapify API and the geoViews Python library and employ our Python skills to create map visualizations.

#### Step1: Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.
Humidity map
![humidity_map](https://github.com/AVI-1213/python_api_challenge/assets/156638175/4293deca-cb48-47fe-8e23-60458e2e1670)

#### Step 2: Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
*A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness*

#### Step 3: Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

![hotel_map](https://github.com/AVI-1213/python_api_challenge/assets/156638175/7b79a256-b485-46f5-92b6-e7e267b86a42)

====










