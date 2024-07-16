# Weather and Vacation Analytics - Python APIs

## Project Overview
This project consists of two main components: WeatherPy and VacationPy. The goal of this project is to analyze weather data across various cities and use the insights to plan future vacations.

### WeatherPy
WeatherPy is a Python script that visualizes the weather of over 500 cities of varying distances from the equator. The data is retrieved using the OpenWeatherMap API and analyzed to understand the relationship between weather variables and latitude.

### VacationPy
VacationPy builds on the weather data obtained in WeatherPy to plan ideal vacation destinations based on specific weather criteria. It uses the Geoapify API to find hotels in the selected cities and visualizes the data on an interactive map.

## Prerequisites
- Python 3.6 or later
- Jupyter Notebook
- Required Python packages listed in `requirements.txt`

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/python-api-challenge.git
    cd python-api-challenge
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Create a file named `api_keys.py` and add your API keys for OpenWeatherMap and Geoapify:
    ```python
    weather_api_key = "YOUR_OPENWEATHERMAP_API_KEY"
    geoapify_key = "YOUR_GEOAPIFY_API_KEY"
    ```

## Usage

### WeatherPy
1. Open `WeatherPy.ipynb` in Jupyter Notebook:
    ```bash
    jupyter notebook WeatherPy.ipynb
    ```

2. Run the cells step-by-step to retrieve weather data, analyze it, and generate various plots. The notebook includes the following steps:
    - **Retrieve Weather Data:** Use the OpenWeatherMap API to get weather data for various cities.
    - **Visualize Data:** Create scatter plots to showcase relationships between latitude and temperature, humidity, cloudiness, and wind speed.
    - **Perform Linear Regression:** Analyze the relationships by computing linear regressions.

### VacationPy
1. Open `VacationPy.ipynb` in Jupyter Notebook:
    ```bash
    jupyter notebook VacationPy.ipynb
    ```

2. Run the cells step-by-step to use the weather data to plan vacations. The notebook includes the following steps:
    - **Load Weather Data:** Load the weather data collected in WeatherPy.
    - **Filter Ideal Locations:** Narrow down the list of cities to find locations with ideal weather conditions.
    - **Find Hotels:** Use the Geoapify API to find hotels in these locations.
    - **Visualize Data:** Create an interactive map showing the locations and details of the hotels.

## Results

### WeatherPy Plots
1. **City Latitude vs. Max Temperature**
    ![City Latitude vs. Max Temperature](./Fig1.png)

2. **City Latitude vs. Humidity**
    ![City Latitude vs. Humidity](./Fig2.png)

3. **City Latitude vs. Cloudiness**
    ![City Latitude vs. Cloudiness](./Fig3.png)

4. **City Latitude vs. Wind Speed**
    ![City Latitude vs. Wind Speed](./Fig4.png)

### VacationPy Map
An interactive map displaying the cities with ideal weather conditions and their respective hotels.

## Conclusion
This project demonstrates how to use APIs to collect and analyze weather data, and then use this data to make informed decisions about vacation planning. The insights gained from WeatherPy help identify the best vacation spots in VacationPy.

## Contributors
- [Sanem Gingery](https://github.com/endoplasmicosmic)

## Resources

- Matplotlib Documentation: https://matplotlib.org/stable/api/index.html
- Pandas Documentation: https://pandas.pydata.org/docs/reference/index.html
- NumPy Documentation: https://numpy.org/doc/stable/reference/index.html
- SciPy Documentation: https://docs.scipy.org/doc/scipy/reference/index.html
- Markdown Guide Cheat Sheet: https://www.markdownguide.org/cheat-sheet/
- Geoapify: https://apidocs.geoapify.com/
- OpenWeather: https://openweathermap.org/
- HoloViews: https://holoviews.org/reference/elements/bokeh/Tiles.html
