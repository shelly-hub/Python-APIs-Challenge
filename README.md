# Python-APIs-Challenge

## Project Aim
This project aims to study weather conditions of over 500 cities and uses the data collected to plan for holiday destinations. 

## Project Description
This project uses python request , APIs (Application Programming Interface) and JSON traversals to retrieve data using code. Here, it is used generate random geographic coordinates and the nearest city to each latitude and longitude combination. Two files would be generated as Weather.py and Vacation.py

#### First file: Weather.py
The weather observations of 500 cities would be derived from studying four weather parameters against latitude. Relationshops of these parameters would then be deduced.

#### Second file: Vacation.py
Using the derived 500 cities generated from first file, in combindation with desired weather conditions, vacations destinations would then be generated.

### Advantages
 - Python library citipy enables to generate large number of cities without making a list of 500 variables. 
 - Using API keys allow us to access various data across without importing or search for specific file
 
### Disadvantages
- Need to be extra careful when sending files containing API keys.
- Need to know format for each parameters when creating string of URL. 
- When retreiving data from JSON file, always need to be aware of brackets used in JSON format file. 
- Different cities list output would be generated at each query, hence it would take a very long time to create a new cities list when restarting or refreshing  kernel. 

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
 4. 
 4. 
 



References
