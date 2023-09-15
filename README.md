# WeatherPy and VacationPy

## Overview

**WeatherPy and VacationPy** are two Python projects that use various libraries, APIs, and data analysis techniques to gather and visualize weather data and identify ideal vacation spots based on specific criteria.

### WeatherPy

WeatherPy is designed to analyze weather data for a list of randomly generated cities around the world. It uses the OpenWeatherMap API to retrieve current weather conditions for each city and then visualizes the data in scatter plots. The project also calculates linear regression models to explore relationships between latitude and weather variables such as temperature, humidity, cloudiness, and wind speed.

### VacationPy

VacationPy complements WeatherPy by using the weather data collected to identify ideal vacation spots. It filters cities with specific weather conditions (e.g., warm temperatures, low humidity, and no cloudiness) and then uses the Geoapify API to find nearby hotels. The project displays these hotels on an interactive map, allowing users to explore potential vacation destinations.

## Table of Contents

- Prerequisites
- Getting Started
- Usage
- How It Works
- Sample Output
- Contributing
- License

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x installed on your system.
- Required Python libraries installed for both projects: `matplotlib`, `pandas`, `numpy`, `requests`, `time`, `scipy.stats`, `json`, and `citipy`.

### WeatherPy Prerequisites

For WeatherPy, you will need to obtain an OpenWeatherMap API key. You can get one [here](https://openweathermap.org/api).

### VacationPy Prerequisites

For VacationPy, you will need to obtain a Geoapify API key. You can obtain it [here](https://geoapify.com/).

## Getting Started

1. Clone this repository to your local machine:

2. Navigate to the project directory:

3. Create a file named `api_keys.py` in the project directory and add your API keys as follows:

   ```python
   # api_keys.py
   weather_api_key = "YOUR_OPENWEATHERMAP_API_KEY_HERE"
   geoapify_key = "YOUR_GEOAPIFY_API_KEY_HERE"
   ```

## Usage

To use WeatherPy and VacationPy, follow these steps:

### WeatherPy

1. Open the WeatherPy.ipynb Jupyter Notebook using Jupyter or JupyterLab.

2. Run the notebook to generate random cities, fetch weather data, and create scatter plots with linear regression models.

3. Analyze the generated plots to explore relationships between latitude and weather variables.

### VacationPy

1. Open the VacationPy.ipynb Jupyter Notebook using Jupyter or JupyterLab.

2. Run the notebook to filter cities with ideal weather conditions and find nearby hotels using the Geoapify API.

3. Explore the interactive map to discover potential vacation destinations with nearby hotels.

## How It Works

### WeatherPy

- Generates a list of random cities worldwide based on latitude and longitude coordinates.
- Retrieves current weather data for each city using the OpenWeatherMap API.
- Creates scatter plots to visualize weather variables (temperature, humidity, cloudiness, and wind speed) against latitude.
- Calculates linear regression models to analyze relationships between latitude and weather variables.

### VacationPy

- Utilizes the weather data from WeatherPy to filter cities with ideal weather conditions for vacation.
- Uses the Geoapify API to find nearby hotels for the selected cities.
- Displays the hotels on an interactive map using Plotly, allowing users to explore potential vacation destinations.

## Sample Output

![WeatherPy Sample Output](WeatherPy/images/weatherpy_sample.png)
![VacationPy Sample Output](VacationPy/images/vacationpy_sample.png)
