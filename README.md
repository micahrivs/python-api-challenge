# Python API Challenge: Weather Analysis 
## Background
Data holds the incredible power to provide definitive answers to various questions. In this project, we will put our Python skills to use by exploring requests, APIs, JSON traversals, and data visualization techniques to address a fundamental inquiry: "What is the weather like as we approach the equator?"

While the initial response to this question may seem obvious - it gets hotter - we aim to go beyond mere assumptions and substantiate this claim with solid evidence. Moreover, we will utilize the weather data we gather to plan future vacations based on preferred weather conditions.

## Project Setup
To embark on this project, we start by creating a new repository called "python-api-challenge" and cloning it to our local machine. Within the repository, we establish a directory named "WeatherPy" to house our main scripts: "api_keys.py," "WeatherPy.ipynb," and "VacationPy.ipynb." It is crucial to include a .gitignore file to ensure the protection of our API key from public exposure.

## Part 1: WeatherPy
In this section, we will create a Python script to visualize the weather of over 500 cities situated at various distances from the equator. Our process involves leveraging the citipy Python library, the OpenWeatherMap API, and our problem-solving skills to develop a representative model of weather conditions across cities.

### Requirements:

Creating plots to showcase the relationship between weather variables and latitude. By utilizing the OpenWeatherMap API, we retrieve weather data for the cities generated in our script. We then create scatter plots to depict the following relationships:

* Latitude vs. Temperature
* Latitude vs. Humidity
* Latitude vs. Cloudiness
* Latitude vs. Wind Speed
Computing linear regression for each relationship. We separate the plots into the Northern Hemisphere (latitude >= 0 degrees) and the Southern Hemisphere (latitude < 0 degrees). Each plot includes the linear regression line, the formula of the model, and the r-values.

After generating each pair of plots, we take the time to explain what the linear regression is modeling and describe any noteworthy relationships or findings we observe.

## Part 2: VacationPy
In this phase, we will utilize the weather data obtained in Part 1 to plan future vacations. Using Jupyter notebooks, the geoViews Python library, and the Geoapify API, we will create map visualizations and narrow down our city options based on preferred weather conditions.

## The steps we take include:

* Creating a map that displays a point for every city in the city_data_df DataFrame, with the size of each point representing the humidity level.

* Narrowing down the city_data_df DataFrame to find our ideal weather conditions based on specified criteria, such as maximum temperature, wind speed, and cloudiness.

* Creating a new DataFrame, hotel_df, to store essential information about each city, including its name, country, coordinates, and humidity.

* Utilizing the Geoapify API to find the nearest hotel within a 10,000-meter radius of the coordinates for each city in hotel_df.

* Enhancing the map by adding the hotel name and country as additional information in the hover message for each city.

## Conclusion
This project showcases the power of Python as we explore requests, APIs, JSON traversals, and data visualization techniques. By analyzing weather data, we can provide concrete answers to fundamental questions and plan future vacations based on preferred weather conditions. Through these endeavors, we gain valuable insights into the relationship between latitude and weather, allowing us to make informed decisions for our travel plans.
