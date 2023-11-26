# Multivariate Time Series Forecasting
This was a project created as a solution to the PS provided by TATA InfoCom. for the ML Hackathon conducted by Techfest, IIT B. <br>
It is inspired by the concept of Multivariate time series forecasting wherein multiple variables will vary over time. Each variable depends not only on its past values but also has some dependency on other variables. <br>
![eda1](https://github.com/vedang-04/MVSTF/images/eda1.PNG)
The given dataset consisted of 3915 regions and their business potential for the past 6 years (1-72 months). I was expected to build a projection of the business potential for each of the 3915 regions for the next 12 to 15 months (72-87 months).<br>
I first modeled for each region individually using univariate series analysis and forecasting using models using classical ML models along with sequential Neural Networks and Univariate Statistical Time Series Models. After this, I used Multivariate Series Analysis wherein I considered only the regions that were correlated to the given region with a threshold greater than 0.5 using Sequential Neural Networks and Multivariate Statistical Time Series Models. The results can be seen below.<br>
![results](https://github.com/vedang-04/MVSTF/images/results.PNG)
The analysis of results reveals that the most effective model is the Vector Auto Regression (VAR) model. The VAR solution was developed by selectively incorporating correlated series to construct the sub-dataset for the concerned region. Univariate time series models demonstrated lower efficiency due to stationarity concerns, while sequential neural networks exhibited strong performance on the provided time series data, surpassing traditional machine learning models.<br>

