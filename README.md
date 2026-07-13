# Weather ETL Pipeline

## Project Overview
A simple ETL (Extract, Transform, Load) pipeline built for Week 7 of the AnalystLab Africa Data Analytics internship. Pulls live weather data from an API, cleans it, stores it, and pulls out quick insights.

## Data Source
Weather data from the [OpenWeather API](https://openweathermap.org/api) — current weather endpoint. Collected data for 3 Nigerian cities: Lagos, Abuja, and Ibadan.

## ETL Process
Extract: Connected to OpenWeather using an API key and pulled current weather data for each city in a loop, one request per city.

Transform: Broke down the raw JSON response for each city into a clean table using pandas — city name, temperature, humidity, weather condition, wind speed, and date/time.

Load: Saved the cleaned dataset two ways — as a CSV file and into a SQLite database.

## Tools Used
- Python
- Pandas
- Requests
- SQLite3
- Google Colab
- OpenWeather API

## Key Findings
- Lagos was the hottest city at 26.52°C
- Abuja was the coldest at 22.73°C
- Abuja also had the highest humidity at 91%
- Lagos and Ibadan both showed rain, while Abuja was cloudy

## How to Run This
1. Clone this repo
2. Get a free API key from OpenWeather
3. Open the notebook in Google Colab
4. Paste your API key into the API_KEY variable
5. Run all cells
