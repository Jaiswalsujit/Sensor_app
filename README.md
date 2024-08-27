# Tracking App

The **Tracking App** is designed to monitor road conditions, traffic levels, and area types (residential, business, restricted) by utilizing various sensors available on a smartphone. The app collects data such as jerk, noise levels, speed, and street address, and stores this information in a database for further analysis.

## Features

- **Jerk Calculation:** 
  - Uses the phone's accelerometer sensor to measure jerk values while traveling.
  - Helps in determining the road condition in a specific area.

- **Noise Level Measurement:**
  - Utilizes the phone's microphone to assess noise levels.
  - Useful for predicting traffic and distinguishing between different area types.

- **Speed and Street Address Detection:**
  - Employs functions related to the Fused Location Provider Client in the GPS library to calculate speed and obtain the street address based on latitude and longitude.

- **Data Storage:**
  - All collected data is transmitted to a server via HTTP requests using the Retrofit library.
  - Data is stored in a PostgreSQL database for further processing and analysis.

## Technology Stack

- **Frontend:**
  - Android Development (Java, XML)
  
- **Backend:**
  - Retrofit Library for HTTP requests
  - PostgreSQL for data storage
  - Server-side implementation to handle and store data

## Use Cases

- **Road Condition Monitoring:**
  - The jerk value provides insights into road quality, which can be used by municipal authorities or transportation companies.

- **Traffic Prediction:**
  - Noise and speed data help predict traffic conditions and classify areas (e.g., residential, business).
