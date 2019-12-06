<h2><u> Stock-Prediction-Analysis </u></h2>

<h3>Buisness Understanding:</h3>
Predicting how the stock market will perform is one of the most difficult things to do. There are so many factors involved in the prediction – physical factors vs. physhological, rational and irrational behaviour, etc. All these aspects combine to make share prices volatile and very difficult to predict with a high degree of accuracy.

<h3>Problem Statement</h3>
<br>
1. What was the daily return of the stock on average? 
<br>
2. What was the correlation between different stocks' closing prices?
<br>
3. What was the correlation between different stocks' daily returns?
<br>
4. How much value do we put at risk by investing in a particular stock?
<br>
5. How clone them according their closing?

<h3>DATASET:</h3>
 The multiple variables in the dataset –> date, open, high, low, last, close, total_trade_quantity, and turnover.
 <br>
 <b>1)Open and Close</b> It represent the starting and final price at which the stock is traded on a particular day.
 <br>
 <b>2)High, Low and Last</b> It represent the maximum, minimum, and last price of the share for the day.
 <br>
 <b>3)Total Trade Quantity</b> It is the number of shares bought or sold in the day and Turnover (Lacs) is the turnover of the   particular company on a given date.
 <br>
Another important thing to note is that the market is closed on weekends and public holidays.Notice the above table again, some date values are missing – 2/10/2018, 6/10/2018, 7/10/2018. Of these dates, 2nd is a national holiday while 6th and 7th fall on a weekend.


<h3>Target Variable:</h3>
The profit or loss calculation is usually determined by the closing price of a stock for the day, hence we will consider the closing price as the target variable.

<h3>ALGORITHMS USED</h3>
<h4>1)Linear Regression:</h4>
<br>
The most basic machine learning algorithm that can be implemented on this data is linear regression. The linear regression model returns  an equation that determines the relationship between the independent variables and the dependent variable. We do not have a set of independent variables. We have only the dates instead. Let us use the date column to extract features like – day, month, year,  mon/fri etc. and then fit a linear regression model.
<br>
Linear regression is a simple technique and quite easy to interpret, but there are a few obvious disadvantages. One problem in using regression algorithms is that the model overfits to the date and month column. Instead of taking into account the previous values from the point of prediction, the model will consider the value from the same date a month ago, or the same date/month a year ago.

<h4>2)KNN REGRESSOR:</h4>
KNN (k nearest neighbours). Based on the independent variables, kNN finds the similarity between new data points and old data points. 
KNN regression is to calculate the average of the numerical target of the K nearest neighbors.
KNN regression uses the same distance functions as KNN classification.
