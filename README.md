# Spatial Analysis on COVID-19

## Web App

You can visit the live Streamlit app here:  
https://covid-19-data-visualizer.streamlit.app

*Note:* Due to inactivity, the app sometimes requires hitting the **Reboot** button to start again.

---

## 📌 Problem

The COVID-19 pandemic generated a vast amount of global data, making it challenging for users to:

- Understand how cases and deaths evolve over time  
- Compare countries effectively  
- Identify high-risk regions quickly  
- Interpret trends without technical tools  

**Goal:**  
Provide an intuitive and interactive dashboard that enables users to explore **spatial and temporal COVID-19 trends** efficiently.

---

## 📊 Data

This project uses aggregated country-level COVID-19 data with the following attributes:

- Confirmed cases  
- Deaths  
- Recovered cases  
- Date (time series)  
- Geographic coordinates (latitude & longitude)  

### Data Sources
- `countries-aggregated.csv` → main COVID-19 dataset  
- `country_coordinates.csv` → geographic mapping data  

### Data Processing
- Converted date column into datetime format  
- Aggregated global ("Worldwide") data  
- Calculated:
  - Total cases and deaths per country  
  - Death ratio (%)  
  - Daily new cases and deaths (via differencing)  
- Resampled time series into:
  - Daily  
  - Monthly  
  - Yearly  

---

## 🔍 Insight

The dashboard provides several key insights:

### 🌍 Global Patterns
- COVID-19 impact is uneven across countries  
- A small number of countries dominate global case and death counts  

---

### 🗺️ Spatial Insights
- The interactive map highlights countries exceeding death thresholds  
- Clear geographic clustering of high-impact regions  

**Insight:**  
High mortality is concentrated in specific regions rather than evenly distributed.

---

### 📈 Temporal Trends
- Time-series charts reveal infection waves  
- Each country shows unique patterns in growth and decline  

**Insight:**  
Pandemic progression varies significantly by country in both timing and intensity.

---

### ⚖️ Fatality Ratio
- Pie chart compares confirmed cases vs deaths  

**Insight:**  
Differences in fatality ratios suggest variations in:
- Healthcare capacity  
- Testing availability  
- Government response  

---

### 📊 Resampled Trends
- Daily, monthly, and yearly views highlight:
  - Short-term spikes (outbreaks)  
  - Long-term trends  

**Insight:**  
Different time granularities reveal different patterns and behaviors.

---

## 💡 Recommendation

Based on the analysis, the following recommendations can be derived:

### 🏥 Public Health
- Improve healthcare capacity in high fatality regions  
- Increase early detection and testing  

---

### 🌍 Policy Makers
- Use spatial insights to:
  - Identify high-risk regions  
  - Allocate medical resources efficiently  

---

### 📊 Data Strategy
- Maintain real-time and transparent reporting  
- Standardize global data collection practices  

---

### 👥 For Analysts & Users
- Use interactive dashboards to:
  - Monitor trends dynamically  
  - Compare countries effectively  
  - Detect emerging waves early  

---

### 🚀 Future Improvements
- Add vaccination data  
- Include per capita metrics (cases per population)  
- Implement forecasting models  
- Enable region-level (sub-country) analysis  

---

## ⚙️ Features

- Displays worldwide and country-specific COVID-19 confirmed cases and deaths  
- Interactive map showing deaths by country with adjustable thresholds  
- Time-series line charts of confirmed cases and deaths by selected country  
- Pie chart visualization of fatality ratio  
- Resampled bar charts for daily, monthly, and yearly intervals  
- Searchable country list with metrics  

---

## 🛠️ Technologies Used

- Streamlit for web app interface  
- Pandas for data processing  
- Plotly Express for interactive charts  
- Folium for map visualization  
- Additional libraries:
  - `st_keyup`  
  - `streamlit_folium`  
  - `folium.plugins.HeatMap`  

---

## 📂 Data

- Aggregated COVID-19 data from CSV file (`countries-aggregated.csv`)  
- Country coordinates from CSV file (`country_coordinates.csv`)  

---

## ▶️ How to Run

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
