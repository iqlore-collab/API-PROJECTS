# API-PROJECTS
API Weather, API Flights, etc.
# Weather and Flight Operations — Advanced API Analytics Project

This project combines OpenWeather forecast data with AeroDataBox flight operations data.

It extends the previous combined notebook by adding:

- arrivals and departures
- more airports and countries
- delay-related fields
- weather risk features
- operational risk scoring
- dashboard-ready outputs
- database-ready tables

## Notebook

`weather_flights_advanced_operations_project_EN.ipynb`

## Project Goal

The goal is to create a practical airport operations analytics dataset by combining:

1. weather forecast data
2. flight arrivals and departures
3. delay-related information
4. airport-day operational summaries

This project does not prove that weather causes delays.  
It builds a structured dataset that can support future delay and disruption analysis.

## APIs Used

- OpenWeather API
- AeroDataBox API via RapidAPI

## Required API Keys

You need:

- OpenWeather API key
- RapidAPI key with AeroDataBox access

The notebook asks for keys at runtime using `getpass`.

## Main Outputs

The notebook exports:

- `fact_weather_forecast.csv`
- `weather_daily_summary.csv`
- `fact_flight_operations.csv`
- `flight_operations_daily.csv`
- `weather_operations_combined_daily.csv`
- `dashboard_airport_daily.csv`
- `dim_airports.csv`
- `weather_api_log.csv`
- `flight_api_log.csv`
- `metadata.json`

## Analytics Included

The notebook creates:

- weather daily summaries
- arrival and departure summaries
- delay indicators
- cancellation indicators
- weather risk levels
- operational risk scores
- dashboard-ready airport-day table

## Suggested Dashboard Views

Good dashboard charts include:

- total flights by airport
- arrivals vs departures
- delay rate by airport
- max wind speed by airport
- weather risk level by airport
- operational risk score by airport

## Limitations

- API data is time-sensitive.
- Free API plans may have rate limits.
- Delay fields may be missing depending on API response.
- Weather data is forecast data, not historical observation.
- This is a prototype, not a production ETL system.

## Production Next Steps

Recommended improvements:

1. convert notebook to Python scripts
2. store API keys in environment variables
3. schedule daily runs with GitHub Actions, Airflow, or cron
4. append outputs to a database
5. build a dashboard in Looker Studio, Power BI, Tableau, or Streamlit
