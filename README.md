# Exploratory Data Analysis and Visualization for Art Auction Data

## Introduction

This project performs an exploratory analysis and visualization on a dataset containing the historical auction prices of thousands of pieces of art. Whether you come from the arts and humanities, or economics and finance, art is an interesting and complex field. With new data starting to become available, for the first time we have the ability to analyze and better understand this historically opaque industry. It is a potential treasure trove for data scientists.

For hundreds of years fine art has been valued by cultures throughout the world for its aesthetic and beauty, but fine art as an asset class also appeals to many people today as an attractive alternative investment that is largely non-correlated to the traditional stock market. The fine art asset class is estimated to have a global market value of over $60 billion in annual turnover and has historically outperformed the S&P 500 in terms of compound annual growth (specifically, 15-year CAGR). Geographically, the art market has for decades been dominated by the United States, United Kingdom and China with the greatest concentration of art sales in the entire world occurring right here in New York City.

Each of our team members has a diverse background. In addition to experience as data scientists, a few of us have a background in economics and have worked for financial services and tech companies. A few of us have also worked in the art industry for galleries or collectors. This topic was a cross-section of our experiences and interests that allowed us to explore timely questions about the prices and dynamics of the fine art market.

From a high level, the questions that intrigued us most were related to knowing more about the auction sale prices (called hammer prices) for pieces of art (called lots) in terms of different artists, location and time periods. We initially developed a large list of potential questions, and narrowed these down based on viability in terms of the data we had available as well as the scope and time constraints for the project. Some of the specific questions we decided to look at are:

1. What is the distribution of quantity of lots and auctions by location, year, and season?
2. What are the lot titles that have higher price or appear more?
3. How is price related to artist’s era/when he/she was born?
4. Do auction prices vary by location and season?
5. Did Financial Crisis have any effect on the auctions?
6. Does the order in which the lot is presented affect the overall sell price?

The detailed final report of the analysis are shared in this repo for your convinience.

## Interactive Component
Link to the interactive part: https://edav-art-viz.firebaseapp.com

### Description
Our interactive visualization is a scatter plot of lot prices over time built with HTML, CSS, Bootstrap and JavaScript.

The visualization allows users to see all of the lots sold according to their price and locations each year. Each color represents a different location, and the black horizontal average line indicates the average hammer price for all lots during the selected year. This visualization supports the project’s main hypothesis that location and season significantly affect the auction performance in terms of the prices of works sold.

We built the interactive visualization so that it would be scalable and versatile if we want to add more features in the future. A few things that we had in mind as features but did not implement due to time constraints included taking the average per auction, and connecting these points with a trend line. We also thought of adding a box plot for each auction that could have been toggled in a similar matter to the jitter feature. Another feature we had hoped to add was the ability to toggle based on location, which would have allowed users to click each location on or off and show the corresponding lot data points. Finally, our time line only allows for scrolling by year, but ultimately the idea would be to have a continuous scroll and even zoom in and out so the user would have full control over their time frame of analysis.

Lastly, both for the interactive visualization and our analysis on a whole, future work would include extending our project to not only analyze auction data from Sotheby’s, but also to analyze data from other auction houses like Christie’s and Phillip,s or museums and other online art data sources to see if our conclusions are consistent for these other data sources as well.

### Instructions

Each vertical line indicates an auction, and all the data points along that line are the lots (pieces of art) that were sold in that auction. Auctions are colored by location so users can see where in the world the auction took place. The average line indicates the average price at which lots were sold in aggregate for the selected year. Additionally, there are a number of ways users can interact with this scatter plot including:

Change Year - Click on the arrows next to the year to either move a year forward or backwards (2006-2018). This can help to compare the different distributions and average price of lots across all years in our dataset.
See Lot Details - Hover over each circle to see the details of the lot transaction. You should expect to see the realized hammer price (sale price) as well as a picture of the actual piece of art. Keep in mind that many of the lots have their pictures copyright protected by Sothebys and will not be display. Nonetheless, most of the more recent images (2017-18) are available. :)
Spread Data Points - Since there are so many data points per auction plotted along the same day, users can add jitter to better observe each data point and counteract overplotting. Click the button that says “Jitter” and this will spread the points from their original location to better see all options. One can easily bring the points back to proper location by unclicking the button.
