# Backend-API-for-Weather-Forecast

# Weather API with Flask
This project implements a simple weather API using Flask, 
allowing users to retrieve current weather information for multiple locations. 
The weather data is fetched from the OpenWeatherMap API.

### Prerequisites
- Python 
- Flask
- Requests library

### Procedure

1. Install the required libraries.
2. Get your OpenWeatherMap API key.
3. Run the application.
4. Open Postman and create a new request to `http://127.0.0.1:5000/weather` with the `GET` method.
5. Add a query param `location` with the value being the city and state (eg: `Bengaluru, KA`).
6. Send the request and check the output. 
