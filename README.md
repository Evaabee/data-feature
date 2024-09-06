# **Flight Delay Predictor - Weather and Flight Status Checker**

This Jupyter notebook demonstrates the creation of a simple prototype that helps users check flight statuses and determine if weather conditions might cause delays.

## **Features**
- Retrieves flight status using the **AviationStack API**.
- Fetches weather data for a specified city using the **Visual Crossing Weather API**.
- Analyzes weather conditions such as precipitation probability, wind speed, and general conditions to determine if the weather might impact flight delays.
- Displays the flight status and informs the user if bad weather conditions are likely to cause delays.

## **Prerequisites**
To run this notebook, you need to set up API keys for:
- **AviationStack API** (for retrieving flight status information)
- **Visual Crossing Weather API** (for fetching weather data)

Make sure to add these API keys to the **SECRETS** tab in Google Colab or store them securely in your environment.

## **Usage**
- Run the notebook cells in order.
- When prompted, enter:
  - A **flight number** (e.g., `DL1087`).
  - A **city name** (e.g., `London,UK`) to retrieve the current weather.
  
The notebook will then display:
- The flight status (e.g., on-time, delayed).
- The current weather conditions in the specified city.
- Whether the flight might be affected by bad weather based on precipitation, wind speed, or weather conditions such as rain or snow.

## **Example Output**

```
Enter the flight number (e.g., DL1087): DL1087
Enter the city for weather (e.g., London,UK): London,UK

Flight Status for DL1087: on-time

Current Weather in London,UK: Rain, Overcast
Precipitation Probability: 100.0%
Wind Speed: 11.0 mph
Bad weather detected in London,UK.
The flight is currently on time, but bad weather may cause delays.
```

## **Note**
This is a simple prototype intended for educational purposes. In a real-world application, additional features such as a user interface, detailed weather forecasts, real-time updates, multiple flights, and more robust error handling would be implemented.

