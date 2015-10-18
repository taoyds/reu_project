Mathematical finance project.
Knowledge and Tools: Sampling, Modeling, Financial Mathematics, Statistics, Matlab

The question of constructing an optimal stock portfolio has been a very important topic in financial investing, and various propositions have been developed since 1950s [1]. Here we intend to propose and test some strategies with a unique approach. There is simply no universal optimal portfolio that is appropriate for every investor, since everyone has a dif- ferent investment goal with a unique risk preference. For example, young investors may be willing to take more risk to pursue higher return than senior retirees. Even for investors with same age, income, and education background, they would still have quite different attitudes regarding risk tolerance. With this in mind, we are trying to develop a strategy designed for certain risk characteristics that an investor is willing to take, and expect to achieve a maximum return.

To construct such a portfolio, the key step is to find the correlation matrix of stocks in the portfolio. The most common way in the finance industry to find correlation between stocks is to use daily closed prices. However we would like to propose an alternative way to calculate correlation coefficient since we believe that using daily closed prices would lose much information for high frequency trading given that hundreds or thousands of transac- tions happened in a trading day. Alternatively, we computed correlation coefficients using stock data based on a transaction level. However this method results in asynchronous prices for different stocks because the timeline of prices did not match for any two stock pair. We solved this problem using both Brownian Bridge and linear interpolation to interpolate prices of all stocks at any given specific time. Soon we found that the Brownian bridge and linear interpolation would introduce errors if the degree to which timelines of two stocks prices do not match is relatively high. To measure the degree to which timelines of two stocks prices match, we employed kernel density smoothing as a criterion to select stocks that can be used to compute correlation using our method.
