Concept and Motivation
In financial markets, optimizing trading decisions can significantly improve investment returns. Our goal is to develop a trading bot that automates the trading process by identifying potential buying and selling opportunities. This trading bot is based on machine learning technology and is able to predict highs and lows in the market as buying and selling opportunities.

Definition of High and Low
In this project, "High" and "Low" refer to the local high and low price of the stock. I used argrelextrema to define the high and low points and then used machine learning to predict these high points date and low points date, these points represent potential sell and buy signals.

Data Retrieval and Annotation
Data comes from the Yahoo Finance API and includes historical stock prices and trading volumes. I preprocessed and cleaned the data, including measuring its Trend indicators, Momentum indicator, Volume indicator and Volatility indicator using the Talib technology package. Then I take the last ten days of price movement to mark the stock's direction. Finally, the Hang Seng Index was also referred to to complete its missing values.

Application of Machine Learning Models
I use 4 machine learning models: Random Forest, SVM, Logistic Regression and Decision Tree. These models were chosen because of their strong performance in handling nonlinear problems and avoiding overfitting. They predict whether each trading day will be a high or a low, and output the accuracy and F1 score as a reference. Finally, Random Forest was selected as the prediction model for actual performance.

Training and Validation
These models are trained on historical data and optimized by changing parameters. During the validation process, I monitor performance metrics such as accuracy, recall, and F1 score to ensure the model's ability to generalize.

Trading Mechanism
Trading decisions are based on buy signals predicted by the model,and each transaction involves a fixed number of shares (100 shares). Sell signals are divided into 4 different strategies and set different stop loss and take profit points to manage risk. Finally, there are also direct predictions of buying and selling signals based on the model as a reference strategy, demonstrating the different profitability of each strategy.

