# Python-APIs-Challenge

## Project Aim
This project aims to study weather conditions of over 500 cities and uses the data collected to plan for holiday destinations. 

## Project Description
This project uses python request , APIs (Application Programming Interface) and JSON traversals to retrieve data using code. Here, it is used generate random geographic coordinates and the nearest city to each latitude and longitude combination. Weather data would then be extracted to be used in the studies. Finally, Python map visualisations would be used to point the holiday destinations. Two files would be generated as Weather.py and Vacation.py. 

#### First file: Weather.py
A random over 500 cities would be generated using python library citypy. Then, a series of weather observations of over 500 cities would be derived from studying four weather parameters against latitude. Relationships of these parameters would then be deduced.

#### Second file: Vacation.py
Using the derived of over 500 cities generated from first file, in combination with desired weather conditions, vacation destinations in terms of hotels location would then be generated.

### Advantages
 - Python library citipy enables to generate large number of cities without making a list of 500 variables. 
 - Using API keys allow us to access various data across without importing or search for specific file
 - Geoview map allows us to visualise cities in world global map easily
 
### Disadvantages
- Need to be extra careful when sending files containing API keys.
- Need to know format for each parameters when creating string of URL. 
- When retreiving data from JSON file, always need to be aware of brackets used in JSON format file. 
- Different cities list output would be generated at each query, hence it would take a very long time to create a new cities list when restarting or refreshing  kernel. 
- These two project files are linked, hence if file one has refreshed its cities list output, second file would also need to bre refreshed and regenerated. 

## Project Method
### File: Weather.py

    1. Download citypy library
    2. Create OpenWeatherMap API as weather_api_key
    3. Import all related libraries.
    4. Generate cities list by using citypy library
    5. Set up URL from openweathermap website, by inserting parameters such as cities, and units in metric.
    6. Create empty dataframe that has following varibales:
     - City name
     - Latitude of the city
     - Longitude of the city
     - Maximum Temperature
     - Humidity
     - Cloudiness
     - Windspeed
     - Country

     7. Scatter plot is then used to plot all these weather variables (temperature, humidity, cloudiness, windspeed) against latitude. 
     8. Linear regression plot of each weather variables with northern and southern hemispheres latitude are also plotted
     9. Relationships of each linear regression plot, in combination with each calculated r-squared value is analysed and described within Jupyter notebook under each variable plot.
 
 ### File: Vacation.py
    1. Download Geoview Python libray, and PATHLIB module
    2. Create Geoapify API as geoapify_key
    3. Import cities list created from File: Weather.py into Vacation.py using path from pathlib module
    4. Geoview map is created to point all cities locatios on world map, and humidity data is used to determine size of each city points.
    5. Data is then filter to ideal weather conditions
    6. New filter data is named as hotel_df
    7. Identify surrounding hotels under the cities list within hotel_df
    8. Create a geoview map that points all the hotels location with its related information in hover columns. 

 



References
