# Stock_Recommender_WebApp
## Motivaton
  Nowadays, recommender systems are almost everywhere in our life. When watching
YouTube, the homepage shows different sections of videos based on the previous watch history.
Also, Netflix and Amazon have similar systems for recommending content that users may find
interesting. Such recommender systems save users time when browsing, and companies can sell
their products more efficiently.

Similarly, it is hard for individual investors or portfolio managers to pick a few
outstanding stocks from thousands of options in the markets. Screeners exist for financial ratios
but fail to be implemented in a personalized, easy-to-use manner. Meanwhile, current existing
stock recommender systems mostly focus on historical returns or are based on stock price
predictions, which normally recommend a set of similar stocks to all users. This paper tackles a
more personalized approach by applying Machine Learning algorithms to the stock
recommender system to provide investors personalized recommendations.

However, a downside of using these powerful algorithms is losing the ability to easily
explain the recommendations with a certain level of trust and confidence, especially for users not
familiar with the technical knowledge of machine learning algorithms. To tackle this challenge,
the SHAP library was used to intuitively explain how each recommendation gained its
preference score to Buy or Sell.

Lastly, a major driving task for this paper was to implement the model seamlessly to an
end-user. Utilizing the platform Streamlit, a web app was developed for ease of use. This app
creates a tool that mirrors the intuitive platforms of Netflix and Amazon, while still
implementing powerful algorithms. Additionally, the app provides compelling information that
builds trust and confidence in what the application is providing for an investor.

## Data set
The provided dataset has a total of 1240 stocks. 32 stocks are marked as ‘1’ to indicate
that they are owned by the portfolio manager, while the remaining 1208 are labeled
as ‘0’ to indicate stocks that are in a watchlist(or general markets).
Each stock has 30 features representing financial ratios and the ratios compared to the industry
benchmarks. For example, the ratios include the Capex to depreciation ratio, dividend payout
ratio, free cash flow conversion cycle, return on assets, return on equity, etc. All of these 30
features have been normalized before use. 

## Methodology
The stock recommender is built using a random forest algorithm from sklearn. 

The recommendations are explained using the SHAP library. 

The web app was developed using [Streamlit](https://streamlit.io/)

Follow the instructions on the Streamlit website to download the library and run the web app script.

Enjoy!
