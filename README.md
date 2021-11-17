# Booking.com Price Prediction in KSA Project 

* Capstone

In order to predict hotel room pricing in the major cities of Saudi Arabia. This project went through the process of building a tool for the ministry of tourism to predict the accommodation prices in riyals given the number of beds, the rating score and number of reviews. 

# Why Booking.com Prediction Project?

* Help tourists and gov to know hotel prices in KSA. 
* Regulate prices and make them competitive.
* Provide price predictions for hotels in most cities.
* Discovering data error entries and outliers.
* Unstable search results in some cities.

# Data Description
The data scraped is described by 10 features as follows:**
* Field Description:

| Field Name | Description                                                                     |
|------------|---------------------------------------------------------------------------------|
| Hotel Name | Names of hotels.                                                                |
| Location   | eg: Riyadh, Jeddah .. etc                                                       |
| Room Type  | eg: Suite, Romm .. etc.                                                         |
| Price      | Room price.                                                                     |
| Price for  | per 1 night .. etc.                                                             |
| Beds       | Number of beds.                                                                 |
| Rating     | Hotel Rating (1 to 10 scale)                                                    |
| RatingTitle| Title of ratings.                                                               |
| Reviews    | Number of Reviews                                                               |    
| Size       | Room Size in m^2                                                                |

* [Further details on the this dataset](https://www.kaggle.com/asafarji/saudi-arabia-bookingcom-2021) - feel free to download it from my Kaggle account!

# Design
A regression model analysis was conducted that encompasses many features and among them the room price.
To gather hotel data Booking.com has been scraped, one of the top and most visited online travel agencies in KSA.
I utilized several regression models and tested for the best fit; to ensure the accuracy of the predictor tool.

# Algorithms

* Fetch:
To ensure the highest accuracy and to avoid incorporating seasonality in Booking.com data, I scraped the website continuously.

* Clean:
The dataset had several unwanted columns, duplicate observations, NaN values and spaces in between the categorical features, so we used pandas library to prepare the data for the regression model.

* Preprocessing:
The following transformation methods were applied, to standardize the values at an equivalent scale and to linearize some of the features that are not linear in nature against the room price:

          ** Feature Scaling:
          a. Robust scaling
          b. Standard scaling

          ** Guassian Transformations:
          a. Log
          b. Box-Cox
          c. Polynomial


# Best Model Predictor (RF) 

* Random Forest Regressor:
* Evaluate model performance.
* Achieving 96% accuracy in test set.
         - The mean absolute error (MAE) is 0.1974 degrees.

<img width="778" alt="Screen Shot 2021-11-14 at 12 12 44 PM" src="https://user-images.githubusercontent.com/93472219/141674865-861e4e28-f29a-4be6-af36-e76ad873aad4.png">



## Website
* Website to predict hotel prices online.

<img width="915" alt="Screen Shot 2021-11-14 at 12 16 04 PM" src="https://user-images.githubusercontent.com/93472219/141674943-00a409ab-29fa-4aba-ae9b-1fb00215c32e.png">

* [Predicts the Booking.com Prices in KSA 🇸🇦](https://share.streamlit.io/a-safarji/streamlit) - feel free to contact me!

# Tools
Language: Python:

* Data Scraping libraries: Extractor & Selenium

* EDA Libraries: Pandas, numpy, seaborn, matplotlib

* Preprocessing Libraries: sklearn, statsmodel, scipy, pylab

* Model Building Libraries: sklearn and Model Testing libraries sklearn

* Others:
SweetVIS, Plotly Express, Missingno Plotting,
Pycaret, Yellowbrick, SHAPE.

## Conclusion & Recommmendation 

* Model building is iterative over time, to increase the accuracy it's a must.

* Booking.com should handle false information and data entry about hotels in KSA.

* Ministry of Tourism should monitor and control hotels prices and increase tourists' trust in online booking platforms. 

* Ensure data quality.    


## Status
Project is: ![##c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) _done_


