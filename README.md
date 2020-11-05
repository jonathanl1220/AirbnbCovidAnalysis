# An analysis of COVID – 19’s effect on the Airbnb market in Manhattan; focused on June 2019 and June 2020
As a New Yorker I am interested in how the home rental market was affected by Covid - 19 in Manhattan. 
The objective is to observe if there was a change in the Mean Price and Listing for the two periods. 

# Data Source 
I gathered my data from http://insideairbnb.com/get-the-data.html.
The data consist of June 2019 and June 2020 Listings data.

# Background Information
-Average daily rates were higher for rentals in July 2020 versus July 2019 in the United States — from about $300 to $323. 

-Home rentals have outperformed hotels in 27 global markets since the onset of Covid-19.

-Airbnb is the biggest player in the short-term rental space 7 million listings in over 220 countries.

# Exploratory Data Analysis

To better understand the data, I wanted to use some exploratory data analysis to determine what section of the dataset I  would utilize.
The data consist of listing through the five boroughs, so I wanted to start with the listings per borough for June 2019 and 2020.

![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/PieChartJune2019.png)
![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/Treemap%20June%202020.png)

Although, Brooklyn almost has a similar count to Manhattan, I thought it would be best to analyze Manhattan's listings. To better analyze Manhattan, I broke the listing up by Neighborhoods  in Manhattan, and got a count of the listings. I wanted to know if there is a difference  in the number of listings between the two periods.

![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/ManhattanListingScatter.png)

With the dataset being divided into their neighbourhoods I wanted to guage the listing prices for the sections of Manhattan. I also wanted to see observe if there was a difference in **Price** of the listings for the two periods. 

![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/ManhattanScatterJunePrice.png)
![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/SlopeChart.png)
At this point I arrived at the realization that this a Supply and Demand situation. The supply of listings remained  approximately the same in the two periods. The **Price** in the two periods did change with the average increasing by $25. This tells me that the demand for Airbnb has increased in June 2020.


























After making my previous observation I decided to run an OLS regression on the **Price** for the two periods. I used **Accommodates** as X value because it was the most statistically significant.
![image](https://github.com/jonathanl1220/AirbnbCovidAnalysis/blob/master/img/Regression2.png)

