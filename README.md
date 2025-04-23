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

---

## FAQ

**How can I test the *Places365* model to classify images?**  
A complete, step-by-step notebook is available in **`/tutorials/tutorial01`**.

**How can I test the model that maps scenes to different modes of transport?**  
See **`/tutorials/tutorial02`**, which shows how to load, run, and evaluate the transport-scene model.

**How do I determine the status from the app data and create bar plots for different scenes and pollutants alongside the Airquix measurements?**  
Follow the workflow in **`/tutorials/tutorial03`**. The notebook merges all CSV files and generates per-scene pollutant bar plots.

**How can I train a model that predicts status using only the app data?**  
The notebook **`notebooks/Train State Determination Neural Network (1).ipynb`** walks through building, training, and evaluating a neural network for this task.

**How do I train the audio model?**  
Check **`notebooks/audio_dataset_finetune.ipynb`**. It is based on the detailed TensorFlow Model Maker Colab tutorial:  
<https://colab.research.google.com/github/tensorflow/tensorflow/blob/master/tensorflow/lite/g3doc/models/modify/model_maker/audio_classification.ipynb#scrollTo=z2ck_Ghdcgt9>
