# 🌦 Weather Dashboard with Air Quality Insights

This project visualizes live weather data and air quality indices (AQI) for multiple cities using Power BI, powered by data from a Weather API.

## 🔹 Project Workflow

### 1. Data Collection

    - Extracted weather data from a Weather API for 6 cities: Ajmer, Alwar, Delhi, Goa, Bangalore, Hyderabad.

    - Stored each city’s records in separate tables.

    - Appended all 6 tables to create a unified Master Table.

### 2.Data Modeling

    - Created reference tables from Master Table:

          - Current → Only current weather records

          - Forecast Hour → Hourly forecasts (excluded current & daily)

          - Forecast Day → Daily forecasts (excluded current & hourly)

    - Applied transformations and hid unnecessary tables, keeping only Current, Forecast_Hour, Forecast_Day visible.

### 3.Measure Creation (DAX)

    - Developed measures for temperature, precipitation, visibility, wind speed, humidity, AQI values, and color coding.

    - Example measures:

          - AQI_Status → Categorizes AQI as Good, Moderate, Unhealthy, Hazardous.

          - AQI_Suggestion → Provides health recommendations based on AQI.

          - Color coding measures (CO Color, O3 Color, PM10 Color, SO2 Color) for better visualization.

          - Curr_Temp_C, For_Temp_C, Pressure, Wind_Speed, etc.

### 4.Dashboard Design

    - Built an interactive Power BI dashboard with:

          - Current Weather: Temperature, humidity, wind, UV index, precipitation.

          - Forecast Weather: Line chart of upcoming daily temperatures.

          - Air Quality Index (AQI): Category-wise breakdown with suggestions.

          - Sunrise & Sunset timings.

          - Chances of Rain with progress bars.

### 🖼 Dashboard Preview
<img width="1319" height="740" alt="Screenshot 2025-09-10 153400" src="https://github.com/user-attachments/assets/c1494545-91b7-41c9-83c1-3892fe6c22c2" />



### 🚀 Tech Stack

    - Power BI (Data modeling, DAX measures, dashboarding)

    - Weather API (Data source)

    - DAX (Custom measures for AQI, weather attributes, and color logic)
