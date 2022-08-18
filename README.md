# python-api-challenge

# Description:

### The purpose of this exercise is to use APIs to look at weather around the world and choose the best vacation locations.

# Process

### Weather.ipynb:
    - Generate a random list of coordinates and use citipy to pick the nearest city to each coordinate.
    - Using OpenWeatherMap, API calls are used on the city list to populate a DataFrame with relavent weather and location data for each city.
    - Scatter plots are generated based on latitude vs. "weather parameter" to see if there are observable weather variations throughout various latitudes.
    - Linear regression is applied to the scatter plots to predict how latitude affects various weather parameters.
    
### Vacation.ipynb
    - Data collected from Weather.ipynb is used to determine prime vacation spots based on specific constraints on weather parameters.
    - A heat map is constructed from the humidity parameter using the gmaps Jupyter plugin.
    - Weather constraints are placed on the data collected from Weather.ipynb to create a DataFrame of prime locations to vacation.
    - Google Places API is used on the new DataFrame to locate hotels near the cities of interest, which are then used to populate another DataFrame.
    - Information gathered from the Google Places API is then used to place markers containing relavent information on the heat map.
