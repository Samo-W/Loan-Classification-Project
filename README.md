# Food Delivery Time Analysis

## Overview
This project analyzes food delivery performance using a real-world dataset.  
The goal is to understand which operational factors most strongly affect delivery duration and identify patterns that could help optimize logistics efficiency.

The analysis focuses on data cleaning, exploratory analysis, and visualization to interpret operational behavior rather than building a predictive machine learning model.

---

## Problem Statement
Food delivery services depend on reliable delivery times to maintain customer satisfaction.  
However, delivery duration varies due to multiple conditions such as distance, traffic, weather, courier experience, and time of day.

The objective of this project is to:
- Identify key drivers of long delivery times
- Detect operational bottlenecks
- Provide interpretable insights using data analysis

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## Project Structure
FoodDelivery-3.ipynb  # main analysis notebook
Food_Delivery_Times.csv          # raw delivery dataset (https://www.kaggle.com/datasets/denkuznetz/food-delivery-time-prediction?resource=download)
The Jupyter notebook contains all of the analysis steps, from importing the data through to the final visualizations. The delivery.csv file holds the raw delivery data, which includes features such as:
 - Delivery_Time_min – total delivery time in minutes
 - Distance_km – distance between restaurant and customer
 - Traffic_Level – categorical traffic condition at the time of delivery
 - Weather – weather condition (e.g. clear, rainy)
 - Time_of_Day – time of day when the order was placed (morning, afternoon, evening)
 - Vehicle_Type – mode of transport used (bike, scooter, car)
 - Courier_Experience_yrs – number of years of experience for the courier

---

## Installation
1. Open **Google Colab**
2. Upload the project files (`FoodDelivery-3.ipynb` and `Food_Delivery_Times.csv`)
3. Install dependencies if needed:

```python
pip install pandas numpy matplotlib seaborn

---

##Usage
Run all cells in the notebook from top to bottom. The notebook will:
	1	Import the delivery dataset and display its basic structure and summary statistics.
	2	Handle missing values by filling categorical features (Weather, Traffic_Level, Time_of_Day) with their mode and numerical features such as Courier_Experience_yrs with the median.
	3	Visualize the distribution of Delivery_Time_min using boxplots and compute the 25th, 50th (median) and 75th percentiles. The 75th percentile is used to define a “late” delivery.
	4	Create scatter and box plots to explore relationships between delivery time and distance, traffic levels, weather conditions, time of day and vehicle type.
	5	Plot a regression line showing how courier experience relates to delivery time.

---

##Results/Output
The analysis reveals several insights:
	•	Delivery time distribution: Most deliveries fall within a manageable time window, but times above the 75th percentile are classified as late deliveries.
	•	Distance vs. time: Delivery time increases with distance, though the relationship is not strictly linear; scatterplots help visualize the spread.
	•	Traffic and weather impacts: Orders placed during heavy traffic or adverse weather conditions tend to have longer delivery times, as shown in the boxplots.
	•	Time of day: Peak ordering periods (e.g. evenings) correlate with higher median delivery times.
	•	Vehicle and experience: Different vehicle types and courier experience levels show subtle differences in delivery performance; a regression line suggests that more experienced couriers may deliver slightly faster.

---

##Dataset source
Kaggle — Food Delivery Time Prediction Dataset
https://www.kaggle.com/datasets/denkuznetz/food-delivery-time-prediction.



