# PairTrading

Learned how to do it from Auquan tutorials. 


According to Quantopia it can be more optimized by using:
Augmented-Dickey Fuller test, Hurst exponent, Half-life of mean reversion inferred from an Ornstein–Uhlenbeck process and Kalman filters.

I did not check for Cointegration as I took conintegrated stocks namely Walmart and Target. You can check whether the stocks you chose are cointegarated or not by using coint from statsmodels.tsa.stattools

Took Z scores for the ratios and 10 day moving average.
Simulated trading by going long if Z>1 and short when Z<-1. Cleared all the positions when abs(Z) < 0.5
If you clear the positions by being even more tight (0.4, 0.3 etc) your profits will reduce.
