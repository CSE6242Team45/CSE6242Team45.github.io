# HARD: Hedging Agricultural Risk Dashboard

Open-source **[Dashboard](https://cse6242team45.github.io/)**. It provides an interactive dashboard for farmers and ranchers to gather comprehensive information on agricultural information, including geographic data visualization on yields for a variety of crops (e.g., wheat, corns, barley, soybeans, and potatoes). Using the data from the **[United States Department of Agriculture (USDA)](https://www.usda.gov/)**, the dashboard also provides price predictions generated by the trained time series models to guide risk management and decision making for farmers and ranchers. Additionally, users can download the desired data and maps when clicking on the buttons.
<br />

> Features

- `Crop price prediction` from time series models
- `Data download` functionality
- Visualization of `crop production` on the geomap
- `Data filtering` by crop and year(month)
- `Geolocate` functionality

<br />

> Links

- 👉 [Background Reading](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1408234)
- 👉 [Video Demo](https://cse6242team45.github.io/)

<br />

## ✨ Implementation and Development

> Run the Dashboard

You do NOT need to install anything to access the dashboard. Simply go to https://cse6242team45.github.io/

> For developers:

```bash
$ git clone https://github.com/CSE6242Team45/CSE6242Team45.github.io.git
$ cd CSE6242Team45.github.io.git
```
Make the desired modifications and host the code in your own git repo (see more instructions in the **Project Host** section below).

<br />

![Screen Capture1.](/screencaptures/dashboard1.png)
![Screen Capture2.](/screencaptures/dashboard2.png)

<br />

## ✨ Project Host

The app is hosted by **[GitHub Pages](https://pages.github.com/)**.

<br />

> General steps to host any project on **GitHub Pages**:

- [Create a public repository](https://github.com/new) named **[username].github.io**, where [username] is your username (or organization name) on GitHub
- Clone the repository
- Add, commit, and push your files (e.g., HTML)
- Open a browser and go to https://username.github.io

<br />

## ✨ Code-base structure

The project is coded using blueprints, app factory pattern, dual configuration profile (development and production), and an intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- css/
   |    |-- .DS_Store                  # 
   |    |-- reset.css                  #
   |    |-- style.css                  #
   |    |
   |-- data/
   |    |-- BARLEY_data_cleaned_PRODUCTION.csv             # 
   |    |-- BARLEY_data_cleaned_SALES.csv                  #
   |    |-- BARLEY_data_cleaned_YIELD.csv                  #
   |    |-- BARLEY_price_prediction_data.csv               #
   |    |-- CORN_data_cleaned_PRODUCTION.csv               # 
   |    |-- CORN_data_cleaned_SALES.csv                    #
   |    |-- CORN_data_cleaned_YIELD.csv                    #
   |    |-- CORN_price_prediction_data.csv                 #
   |    |-- POTATOES_data_cleaned_PRODUCTION.csv           # 
   |    |-- POTATOES_data_cleaned_SALES.csv                #
   |    |-- POTATOES_data_cleaned_YIELD.csv                #
   |    |-- POTATOES_price_prediction_data.csv             #
   |    |-- SOYBEANS_data_cleaned_PRODUCTION.csv           # 
   |    |-- SOYBEANS_data_cleaned_SALES.csv                #
   |    |-- SOYBEANS_data_cleaned_YIELD.csv                #
   |    |-- SOYBEANS_price_prediction_data.csv             #
   |    |-- WHEAT_data_cleaned_PRODUCTION.csv              # 
   |    |-- WHEAT_data_cleaned_SALES.csv                   #
   |    |-- WHEAT_data_cleaned_YIELD.csv                   #
   |    |-- WHEAT_price_prediction_data.csv                #
   |    |-- county_code.csv                                #
   |-- js/
   |    |-- .DS_Store                                      #    
   |    |-- .Rhistory                                      # 
   |    |-- new.js                                         #
   |-- screencaptures/
   |    |-- dashboard1.png                                 #    
   |    |-- dashboard2.png                                 #    
   |-- .DS_Store
   |-- PricePred.geojson
   |-- README.md
   |-- index.html
   |-- yield.geojson
   |
   ************************************************************************
```
<br />

## ✨ Credits & Links

- [USDA Data Source](https://quickstats.nass.usda.gov/)
- [Course Link](https://omscs.gatech.edu/cse-6242-data-visual-analytics)

<br />
