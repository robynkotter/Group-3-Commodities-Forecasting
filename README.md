# Group-3-Commodities-Forecasting
## Business Problem
Swire’s profitability is greatly affected by fluctuations in commodities pricing. To optimize procurement strategies and inventory management, a more in-depth understanding of Aluminum, Sugar, Cotton, Corn, Coffee, Soybean, and Soybean Oil prices is needed. Historical commodities prices will help us better understand the behavior of these prices over time and allow us to develop accurate forecasting models to help achieve near and long-term business objectives. 

## Analytical Objective
We have explored many different time-series prediction models and evaluated each one for comparison with RMSE as the first hurdle in determining whether each model is effective for these historical commodities’ prices. Our goal has been to select the most appropriate models and produce accurate 3- and 12-month predictions as our final deliverables for this project. 

## Presentation Materials 
The exploration of these models is outlined in our Presentation here: [Presentation Slide Deck](https://github.com/robynkotter/Group-3-Commodities-Forecasting/blob/00ba5384f02d11964bbaf2db867c2b5c685c1ab9/MSBA_Project_final.pptx) 

A complete score sheet for the performance of each model can be found here <hyperlink> 

R code for EDA and ARIMA and SARIMA Models can be found here: [R code](https://github.com/robynkotter/Group-3-Commodities-Forecasting/blob/33c50ea014fb5ae43ccbad2ca38a1b4ff050fdfc/Capstone_Kotter_Robyn.Rmd)

## Commodity Findings and Conclusion

### Price
The price of commodities sugar, cotton, corn, coffee, soybean, soybean oil and aluminum show high correlation. We see this in both a heatmap and trendlines. In trend line plots, we also see a high degree of volatility in the price. Whenever there have been disruptions in demand or supply of commodities, we see price reactions amongst all commodities that follow similar trends.  

Using the consumer price index, we discovered that the inflation rate follows the same trends as the change of price rate. In times of volatility, the price would sometimes outpace the rate of inflation especially during demand price shocks. However, with the recent supply shocks and high inflation, CPI changes seem to be outpacing commodity prices. For the commodities corn and aluminum, they have seen long-term price drops when factoring for inflation.  

There are many factors within the market impacting price. One of the biggest drivers is interest rates and government policies. Increased interest rates have been used by governments to regulate the price of commodities historically. Other factors include emerging technologies, population growth, climate change and heterogeneity amongst commodities.  

According to a comprehensive study from the World Bank, 50% of commodity price volatility stems from demand. Emerging technologies are an example of how demand for certain commodities can change. 20% of volatility stems from supply shocks. Crop yield disruptions or pandemics are examples of what can impact supply and can impact price volatility.  

The price of commodities did not show seasonality trends. We also checked for weekly and daily trends on price and did not find any. The price was more strongly correlated with market cyclicality.

### Modeling 
The chosen model for predicting this type of data is Standard GARCH. This model was particularly good at measuring the highly volatile data. The model measures for large variances in price called homoskedasticity and uses it for predictions. Models such as ARIMA factor out homoskedasticity leading to a false sense of precision in confidence intervals and worse overall performance. In testing the models, we saw that the GARCH predictions consistently had the lowest AIC and BIC values performing the best. Because of these factors, this is the recommended model for predictions.  

### Recommendations/Conclusion 
The first recommendation would be to prioritize using the GARCH model for price forecasting. Prices are highly volatile and follow market cyclicality. Various market trends can be monitored in addition to modeling to set expectations of price movement.  

Once the forecasted results are received a decision model can be built which will be valuable in helping decide when to buy and procure commodities. Given the confidence intervals, we can estimate when to buy to maximize cost savings. 
