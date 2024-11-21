# Ann Arbor Weather Analysis (2005-2015)

## Overview

This project analyzes historical weather data from Ann Arbor, Michigan, collected by the National Centers for Environmental Information (NCEI) Global Historical Climatology Network daily (GHCNd). It visualizes record high and low temperatures over the years 2005–2014 and highlights instances in 2015 where new records were set.

---

## Project Objectives

The main objectives of this project are:
1. Visualizing Historical Temperature Records:
 - Plot the record high and record low temperatures for each day of the year (2005–2014).
 - Shade the area between the record highs and lows for better visualization.
2. Identifying 2015 Extremes:
 - Scatter plot any 2015 temperatures (highs or lows) that exceed the 2005–2014 records.
3. Leap Year Handling:
 - Exclude February 29th from the dataset for consistency across non-leap years.

---

## Dependencies and Installations

To use this repository and run the notebooks, you will need to have Python and the following libraries installed:
1. Pandas
2. NumPy
3. Matplotlib
- code: pip install numpy pandas matplotlib jupyter

To get started with this repository, clone it to your local machine:
- code: git clone https://github.com/Lazycodes/Ann_Arbor_Weather_Analysis_2005-2015.git

Navigating to directory
- code: cd Ann_Arbor_Weather_Analysis_2005-2015

---

## Dataset

The dataset used for this project is:
1. <a href="https://github.com/Lazycodes/Ann_Arbor_Weather_Analysis_2005-2015/blob/main/BinSize_d400.csv">BinSize_d400.csv</a>: contains location of dataset
2. <a href="https://github.com/Lazycodes/Ann_Arbor_Weather_Analysis_2005-2015/blob/main/fb441e62df2d58994928907a91895ec62c2c42e6cd075c2700843b89.csv">Daily_Climate_Records</a>
Each row in this datafile corresponds to a single observation from a weather station, and has the following variables:
 - id : station identification code
 - date : date in YYYY-MM-DD format (e.g. 2012-01-24 = January 24, 2012)
 - element : indicator of element type
   - TMAX : Maximum temperature (tenths of degrees C)
   - TMIN : Minimum temperature (tenths of degrees C)
 - value : data value for element (tenths of degrees C)

---

## Project Steps

1. Data Preparation:
- Load the dataset and convert value to Celsius.
- Remove leap days (February 29th).
- Split data into TMAX and TMIN records.

2. Data Analysis:
- Group data by day of the year for 2005–2014 to determine daily record highs and lows.
- Identify 2015 temperatures that exceeded these records.

3. Visualization:
- Create a line graph of record highs and lows (2005–2014).
- Shade the area between the highs and lows.
- Overlay scatter plots for 2015 records-breaking temperatures.

---

## Results
1. The visualization demonstrates a clear range of daily temperature variations for 2005–2014.
2. Several instances of extreme temperatures in 2015 suggest a potential increase in weather volatility.

Sample Picture
![Example_image](https://github.com/Lazycodes/Ann_Arbor_Weather_Analysis_2005-2015/blob/main/Screenshot%202024-11-21%20at%2020.35.37.png)
