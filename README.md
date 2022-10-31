*insert general picture*

# Predicting Housing Prices in the Top Growing Metros
This repository was created to show proof of concept in using timeseries models to predict housing prices for a real estate investment firm.

By: Sarah Jack and Clay Hunn


# Overview & Repository Structure
So for this dataset we have the median prices of home sales in over 14,000 zipcodes across the U.S from Zillow housing data dating from April 1996 to April 2018.  Our objective is to use time series models to help a real estate firm in making investment decisions with their current and future portfolio of properties.  








# Data Analysis
So after looking through the data, we decided to sort our zipcodes by SizeRank which is the only other descriptor included besides location and price.  After focusing in on the top 500 zipcodes, we decided to sort them by Growth Rate/ROI. We created this by dividing the most recent price by the farthest back price and subtracting by one.  This created a overall growth rate of every zipcode in our Top 500.  Once we had our Growth Rate, we pulled out the top 5 Metros by growth rate. These ended up being New York City, Los Angeles, Miami, Chicago, and Dallas/Fort Worth.  

*insert picture of growth rate graph*



# ARIMA Models
All of our models were first made stationary then from there we did a train/test split. Our training being April, 1996 to March, 2017 and testing being April, 2017 to April, 2018.  Some of the metrics we utilized include Dickey-Fuller Test for stationarity, ACF & PACF for  order of p d q, p-value, coefficents, skew, heteroskedasticity, and kurtosis for model tuning, and finally mean square error, root mean square error, and residuals for model evaluation.


*pictures of our models*

# Conclusion
In conclusion we can accurately capture the general trend of these metros, and can definitely recreate this for any other metros our client is interested in.  The knowledge of future price action can help influance high level descisions to help fuel real estate portfolio growth.  Using our models a real estate firm can keep on the cutting edge of technology and remain one step ahead of competitors.  It almost seems if you are in any kind of competitive market based on price movements and you are not using time series models, you will forever be a step behind.  



# Future Investigation
In the future we would like to add in the last 4 years of market prices as the past years have been a very volatile time period for housing. We would like to see how that impacts our models performance and how accurate our model would perform in the more recent market.  We would also like to add in inflation rates and interest rates to assist in our models performance.   



# More Information
jupyter notebook 

questions 



# Repository Structure

├── README.md                        <- The top-level README for reviewers of this project
├── final.ipynb                      <- Narrative documentation of analysis and modeling in Jupyter notebook
├── presentation.pdf                 <- PDF version of project presentation
├── data                             <- Both sourced externally and generated from code
└── images                           <- Both sourced externally and generated from code

