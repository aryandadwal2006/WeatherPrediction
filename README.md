Weather Prediction System
Overview
A machine learning-based weather forecasting system that predicts temperature, humidity, and wind speed using Random Forest Regression with multi-target capabilities.

Features
Multi-target weather parameter prediction
Seasonal pattern recognition
7-day forecast generation
Interactive visualizations
Statistical analysis
Realistic weather pattern modeling
Sample Predictions
Summer Forecast (Sample from July 2023)
Temperature Range: 22.6°C to 25.2°C
Average Temperature: 23.8°C
Humidity Range: 50.7% to 68.9%
Average Wind Speed: 8.6 km/h

Winter Forecast (Sample from December 2023)
Temperature Range: 3.3°C to 5.6°C
Average Temperature: 4.7°C
Humidity Range: 70.2% to 83.7%
Average Wind Speed: 14.5 km/h

Installation
Clone the repository:
git clone https://github.com/aryandadwal2006/WeatherPrediction.git
cd WeatherPrediction

Create and activate virtual environment:
python -m venv weather_env

For Windows
weather_env\Scripts\activate

For Unix/MacOS
source weather_env/bin/activate

Install required packages:
pip install -r requirements.txt
Project Structure
WeatherPrediction/
├── weather_env/ # Virtual environment
├── AryanDadwal_Jupyter_notebook.ipynb # Main notebook
├── WeatherPrediction_Documentation.docx # Detailed documentation
├── weather_prediction_model.joblib # Saved model
├── requirements.txt # Package dependencies
└── README.md # This file

Usage
Basic prediction:
from datetime import datetime
Make single day prediction
prediction = make_prediction(
date='2023-07-15',
prev_temp=25,
prev_humidity=65,
prev_wind=10
)

Generate weekly forecast
forecast = generate_weekly_forecast(start_date=datetime.now())

Visualize predictions:
Plot weekly forecast
visualize_weekly_forecast(forecast)

Dependencies
Python 3.x
pandas
numpy
scikit-learn
matplotlib
seaborn
joblib
Model Performance
Accurate seasonal pattern recognition
Realistic parameter relationships
Strong performance in temperature prediction
Reasonable humidity and wind speed forecasts
Limitations
Requires previous day's weather data
Limited to 7-day forecasts
No precipitation prediction
Basic extreme weather handling
Future Improvements
Add precipitation prediction
Incorporate external weather data
Implement extreme weather detection
Add confidence intervals
Extend forecast range
Author
Aryan Dadwal

License
This project is licensed under the MIT License - see the LICENSE file for details.