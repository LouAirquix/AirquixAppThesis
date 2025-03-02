# AirquixAppThesis

**Work in progress** — I’m currently setting up this repository. More details and content will be added soon!

**Thesis Goal**  
This thesis aims to collect contextual information about an environment using an Android app and the Airquix01 device and then link it with air quality data. The result is a context-aware environmental classification that reveals how different environmental states correlate with pollutant concentrations.

---

## Determining the Final Status

1. **Download the App**  
   First, download the app from the `/app` folder. (More details about the app’s development can be found here: [AppAirquix](https://github.com/LouAirquix/AppAirquix))

2. **Data Collection**  
   Use the app together with the Airquix01 device to record measurements.

3. **CSV Export**  
   Once you stop recording, export the CSV files from the app and also download the Airquix01 measurement files from Grafana:  
   [Airquix10 Time Series](https://airq.meteo.physik.uni-muenchen.de/d/e823731f-c343-425f-a855-dbe519132997/airquix10-time-series?orgId=1&from=now-12h&to=now&timezone=browser)

4. **Analysis**  
   Finally, use the Jupyter Notebooks in the `/notebooks` folder to merge all CSV files and determine the final status.
