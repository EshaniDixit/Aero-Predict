# Air Quality Monitoring and Prediction

This project is a web application that continuously monitors air quality across a city, predicts pollution levels based on historical data, and provides actionable measures to mitigate poor air quality. The app uses a machine learning model to predict the Air Quality Index (AQI) and display the current air quality status for different cities.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Dataset](#dataset)
5. [How the Model Works](#how-the-model-works)
6. [Installation and Setup](#installation-and-setup)
## Project Overview

This project is an AI-powered air quality monitoring and prediction system that uses various sensors to collect real-time data on air pollutants and environmental conditions. The system employs Intel optimized libraries, including oneAPI Data Analytics Library (oneDAL) and oneAPI Deep Neural Network Library (oneDNN), for efficient data analysis and AI model performance. The system is designed to predict air quality levels and provide insights for proactive decision-making to improve environmental health and sustainability.

## Features

- Predicts AQI and pollutant levels (PM2.5, PM10, NO2, O3) based on city input.
- Displays real-time air quality classification (Good, Moderate, Unhealthy, etc.).
- Visualizes missing data using heatmaps for quality assurance.
- Utilizes a machine learning model trained on historical air quality data.
- Web-based interface built using Flask for easy user interaction.

## Technologies Used

- *Python*: Programming language used for the backend and model development.
- *Flask*: Web framework for hosting the application.
- *Pandas*: For data preprocessing and manipulation.
- *Seaborn & Matplotlib*: For data visualization.
- *Scikit-learn*: Used for training the machine learning model.
- *HTML/CSS/JavaScript*: Frontend interface design.
- *Joblib*: For saving and loading the trained machine learning model.

## Dataset

The air quality data used in this project comes from historical records of air quality in India. The data contains key pollutants like PM2.5, PM10, NO2, and O3, as well as other environmental variables. The dataset includes multiple CSV files for different time resolutions (hourly and daily data).

## How the Model Works

1. *Data Collection*: The historical data is preprocessed to handle missing values, outliers, and scaling.
2. *Feature Selection*: Important features like PM2.5, PM10, NO2, temperature, and humidity are extracted to predict AQI.
3. *Model Training*: A Random Forest Regressor is trained on the dataset, using features as inputs and AQI as the output.
4. *Prediction*: Once trained, the model predicts the AQI for new inputs provided by the user.
5. *Integration*: The model is integrated with Flask, allowing real-time predictions via the web interface.

## Installation and Setup

### Prerequisites

- Python 3.x installed on your system.
- Install the necessary Python libraries and intel libraries by running the command:

```bash
pip install -r requirements.txt
python app.py
