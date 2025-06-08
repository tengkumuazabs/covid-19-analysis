# Spatial Analysis on COVID-19

## Web App

You can visit the live Streamlit app here:  
[https://covid-19-data-visualizer.streamlit.app](https://covid-19-data-visualizer.streamlit.app)

*Note:* Due to inactivity, the app sometimes requires hitting the **Reboot** button to start again.

## Features

- Displays worldwide and country-specific COVID-19 confirmed cases and deaths.
- Interactive map showing deaths by country with adjustable thresholds.
- Time-series line charts of confirmed cases and deaths by selected country.
- Pie chart visualization of fatality ratio.
- Resampled bar charts for daily, monthly, and yearly intervals.
- Searchable country list with metrics.

## Technologies Used

- Streamlit for web app interface
- Pandas for data processing
- Plotly Express for interactive charts
- Folium for map visualization
- Additional libraries: `st_keyup`, `streamlit_folium`, `folium.plugins.HeatMap`

## Data

- Aggregated COVID-19 data from a CSV file (`countries-aggregated.csv`)
- Country coordinates from a CSV file (`country_coordinates.csv`)

## How to Run

1. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the app:
    ```bash
    streamlit run app.py
    ```

---

*Data valid as of April 2022.*
