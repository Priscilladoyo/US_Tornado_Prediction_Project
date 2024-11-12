# US Tornado Project

## Project Overview
This project analyzes historical storm and tornado data across the United States, focusing on patterns, frequencies, and other key attributes from 1950 to 2021. Using two datasets, `storm.csv` and `us_tornado_dataset_1950_2021.csv`, the analysis aims to uncover insights into tornado occurrences and their impacts on regions across the country.

## Project Files
- **`storm.csv`**: Contains general storm data, including dates, storm categories, locations, and other relevant metrics.
- **`us_tornado_dataset_1950_2021.csv`**: Specifically focused on tornado events from 1950 to 2021, detailing each event’s location, magnitude, casualties, damages, and additional relevant metrics.

## Goals and Objectives

### 1. Analyze Temporal and Geographic Trends of Tornado Occurrences
   - **Objective**: Understand yearly, monthly, and time-of-day patterns in tornado occurrences across the U.S., with a focus on identifying trends and seasonal variations.
   - **Key Questions**:
      - How many tornadoes have occurred from 1950 to 2021?
      - Are tornadoes becoming more or less frequent over time?
      - What are the monthly and seasonal patterns of tornado occurrences?
      - Which states or regions experience the highest number and intensity of tornadoes?

### 2. Examine Tornado Intensity, Impact, and Environmental Factors
   - **Objective**: Analyze tornadoes by intensity (Enhanced Fujita scale) and assess correlations between intensity and impact metrics, such as fatalities, injuries, and property damage.
   - **Key Questions**:
      - What is the distribution of tornado intensities, and how does this vary over time?
      - How do fatalities, injuries, and property damages relate to tornado intensity?
      - Are there any environmental factors, such as temperature and humidity, associated with tornado occurrences?

### 3. Conduct a Detailed Analysis of Tornadoes in Texas
   - **Objective**: Study the specific characteristics and impact of tornadoes in Texas, examining trends, intensity distribution, and regional hotspots.
   - **Key Questions**:
      - How many tornadoes have occurred in Texas, and what is the trend over time?
      - When do tornadoes most frequently occur in Texas, by month or season?
      - What are the intensity distribution and impacts (fatalities, injuries, damages) of tornadoes in Texas?
      - How does tornado frequency and intensity in Texas compare to other states?

### 4. Explore the Predictive Potential for Tornado Occurrences
   - **Objective**: Identify key variables and build predictive models to determine whether tornadoes can be forecasted based on historical data, focusing on temporal and geographic predictions.
   - **Key Questions**:
      - Are there specific factors that strongly correlate with the occurrence of tornadoes?
      - Can a time series model capture seasonal or monthly patterns in tornado activity?
      - What is the accuracy and reliability of predictive models in forecasting tornado occurrences and severity?

## Project Summary
The US Tornado Project is a data analysis initiative that seeks to uncover patterns, trends, and impacts of tornado occurrences across the United States from 1950 to 2021, using the `storm.csv` and `us_tornado_dataset_1950_2021.csv` datasets. This project explores temporal and geographic trends, tornado intensity and impact, environmental factors, and provides a focused study on Texas, comparing its tornado activity to other states. Additionally, it investigates the feasibility of predicting tornado occurrences using historical data, assessing model accuracy and key predictive features.

Through these analyses, the project aims to deepen understanding of tornado behaviors, inform risk assessments, and support efforts in tornado prediction and disaster preparedness.

---

## Tornado Prediction Analysis
The data analysis identified several key features with predictive potential for tornado intensity and severity:

- **Tornado Path Length (`len`)**: This feature shows a moderate positive correlation with tornado intensity (magnitude). Longer tornado paths are often associated with more intense tornadoes, making path length a primary predictive feature for intensity.
- **Tornado Width (`wid`)**: Similar to path length, tornado width has a moderate positive relationship with intensity. Wider tornadoes tend to be more intense, making width a valuable feature for predicting tornado severity.
- **Wind Speed (`wind`)**: Although wind speed has a weaker correlation with tornado intensity, it still adds value to the prediction models, especially in classification tasks where it aids in distinguishing severity.
- **Atmospheric Pressure (`pressure`)**: Like wind speed, pressure shows a weak correlation with tornado intensity. However, when combined with other features, it can slightly improve model accuracy, particularly for distinguishing high and low-risk tornado events.

### Summary
Path length and width are the strongest predictors of tornado intensity in this dataset, while wind speed and pressure contribute additional predictive value, especially in severity classification tasks. The average conditions during tornado occurrences in this dataset show an approximate wind speed of 50.27 mph and atmospheric pressure around 992.21 hPa. Together, these features provide a foundation for predicting both the severity and intensity of tornadoes.
