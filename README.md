# Weather ETL Pipeline

## Project Overview
This project demonstrates a simple **ETL pipeline** using the following:
- **Python** for ETL logic
- **Jupyter**
- **Airflow** and 
- **OpenWeather API** as the main data source ( https://openweathermap.org/ )

## Project Steps
1. **Extract** weather data from API ( Focus was on 10 East Coast cities).
2. **Transform** by:
   - Adding Fahrenheit temperature, laculation was done
   - Categorizing the temperature, so its easy to understand (Hot, Warm, Cool)
   - Categorizing the humidity (High, Medium, Low)
3. **Load** into a CSV (`data/weather_data.csv`) check the data folder for a sample of what the CSV looks like.

## Running Locally
```bash
# Installing all the required dependencies
pip install -r requirements.txt

# To run the ETL directly
python scripts/weather_etl.py
