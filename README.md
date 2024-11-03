# Walmart Store Weather Impact Analysis
This project aims to map Walmart locations across the USA with real-time and future weather data. Through predictive modeling, it assesses the impact of various weather conditions on each store, generating risk levels and alerts. Using machine learning techniques, it enables proactive measures based on forecasted weather impacts.

## Project Overview
**Walmart Location Mapping:**   Identify all Walmart locations and map them to current weather conditions.  
**Data Preprocessing & Transformation:** Clean, transform, and preprocess weather data, categorizing it into defined impact levels.  
**Training & Testing:** Train a predictive model using current weather data to forecast impact levels and alerts.  
**Future Weather Impact Prediction:** Test future weather data against the trained model to classify impact levels and generate alerts.  
**Visualization:** Plot Walmart locations with impact levels on an interactive map to visualize real-time and forecasted weather effects.  

# File Descriptions
## Notebooks & Code
### walmart store weather impact.ipynb:
The primary notebook where data preprocessing, transformation, training, and testing of both current and future weather data occur.

## Data Files
### walmart_store_data_copy1.csv & walmart_store_data_copy2.csv (input files): 
Walmart store location data, split into two files due to API call limitations.
### weather_output_df1.csv & weather_output_df2.csv:
Weather data output files corresponding to walmart_store_data_copy1.csv and walmart_store_data_copy2.csv.
### walmart_weather_df_output.csv:
Combined weather data output file created by appending weather_output_df1.csv and weather_output_df2.csv. This file includes processed and categorized weather data.

## Model & Forecast Data
### multi_output_rf_model.pkl:
Trained Random Forest model used to predict future weather impact levels and alerts.
### walmart_weather_with_alerts.csv:
The file containing impact levels and alerts generated for the future weather data.
### future_forecast_weather_data.csv:
The latest forecast weather data retrieved via API, used for testing against the trained model.
### predicted_impact_alert_levels_multi_output.csv:
Output file containing future forecast impact levels and alerts based on the trained model predictions.
### predicted_impact_alert_levels_with_coordinates.csv:
Final tested output file with Walmart store coordinates, used for plotting.

## Visualization Files
### figure_52.html:
Initial map plot displaying Walmart store locations with current weather data.
### figure_56.html: 
Enhanced map plot with Walmart store locations and current impact levels and alerts.
### figure_128.html: 
Final interactive map plot displaying Walmart store impact levels and alerts based on future weather forecasts.

# Project Workflow
**Data Collection:** Gather Walmart store data and real-time weather data through API calls.  
**Data Processing:** Clean and preprocess data, merging location and weather data into a single file.  
**Categorization:** Classify weather data into defined impact levels (Low, Medium, High, Severe) and generate alerts.  
**Model Training:** Train a multi-output Random Forest model on current data, saving the model as multi_output_rf_model.pkl.  
**Forecast Testing:** Test future forecast data using the trained model to generate impact levels and alerts.  
**Visualization:** Plot Walmart locations and predicted impact levels on an interactive map using Plotly.  

### How to Run
**Clone the Repository:** git clone https://github.com/varma9803/Walmart-Store-Weather-Impact  
**Install Dependencies:** Ensure you have Python and the required libraries installed (pandas, scikit-learn, plotly, joblib).  
**Run the Notebook:** Execute walmart store weather impact.ipynb to preprocess data, train the model, and generate forecasts.  
**View Visualizations:** Open figure_52.html, figure_56.html, or figure_128.html in a web browser to view Walmart locations with impact levels and alerts. (Note: check the newly generated file name in iframe folder).
  
### Results & Insights 
### This project provides a comprehensive view of Walmart store vulnerability to current and future weather conditions, allowing for:

**Identification of high-risk stores during severe weather events.**  
**Predictive alerts to aid in proactive store management and customer safety.**  
**Visual insights through interactive maps to support decision-making.**  

### Future Improvements
**Real-time Updates:** Integrate real-time data fetching for continuous updates on impact levels and alerts.  
**Enhanced Features:** Incorporate additional weather attributes for a more robust predictive model.  
**Automated Report Generation:** Enable automated generation of reports based on forecasted impact for each location.  
