# Nike Stocktwits Machine Learning
**Introduction**\
I aim to identify any relationships between StockTwits posts on Nike and how that reflects on Nike's stock prices.
With the prominence of r/WallStreetBets and increase in retail investors, public opinion and commentary has become more influencial than ever.
In an attempt to predict stock price movement using text data, I utilize the TF-IDF metric in addition to moving averages and volume polarity.

**Methodology**\
I first conducted exploratory analysis using Tableau to analyze stock price trends for Nike.
Then I organized the StockTwits text data into TF-IDF metrics, moving averages, and polarities.
I restructured the dataframe using simple inner joins and adjusted t-day price changes into binary (up or down).
I conducted Naive-Bayes and Logistic Regression classification on whether the stock price would go up or down based on term frequencies.
High accuracy for training data but extremely overfit as test accuracy was low.
Next, I applied ordinary linear regression on the continuous t-day price change. Again, extremely successful training accuracy and R^2,
but overfit when it came to test dataset.

**Results**\
Naive-Bayes Accuracy for t-day Price Changes\
<img src="https://user-images.githubusercontent.com/31304876/121604047-b1651500-c9fe-11eb-89df-58786a24fe1b.png" width="200" height="200">

Logistic Regression Accuracy for t-day Price Changes\
<img src="https://user-images.githubusercontent.com/31304876/121604399-4d8f1c00-c9ff-11eb-90d5-a19c40ec5c4f.png" width="200" height="200">

Training Set Results for Ordinary Linear Regression\
<img src="https://user-images.githubusercontent.com/31304876/121604729-e58d0580-c9ff-11eb-9855-c347751fe790.png" width="400" height="200">

Test Set Results for Ordinary Linear Regression\
<img src="https://user-images.githubusercontent.com/31304876/121604348-351f0180-c9ff-11eb-8976-7e8199b83001.png" width="400" height="200">

**Reflection**\
I really enjoyed this project. I was able to expand my understanding of the data analytics pipeline, including data visualization, exploratory data analysis,
database management, as well as machine learning! Ultimately, my dataset is extremely overfit and helped me realize the intense challenges when working with
text data. Furthermore, I learned that machine learning can assist investors to further understand how stock prices move; however, stocks, like many other
aspects of life, are simply unpredictable. I hope to further expand on this project over the next few months: applying different algorithms, feature selections,
simply acquiring more data.
