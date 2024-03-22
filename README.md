 Develop and test/verify a correlation-based algorithm to correlate when the Schiller P/E ratio is very high (spikes upward significantly) 
 and the S&P500 is also high (peaking or ready to peak).  
 Thus, your algorithm will act as a predictor of when to "sell" the S&P500 index (as if it were a stock or Exchange-Traded Fund (ETF)) 
 by outputting a correlation coefficient in the range [-1, 1], where values in the range [0.9, 1] (or similar range) would be your "sell indicator".  

https://www.longtermtrends.net/sp500-price-earnings-shiller-pe-ratio/

Design and develop a convolutional neural network (CNN) in Python that will recognize A-B-C-D-wave patterns in the S&P500 data ,  
using libraries such as PyTorch (and, if necessary, Tensor Flow).  

Train your CNN and RNN on your Training Set (S&P500 data and/or Schiller P/E data, from above) 
then test to ensure it functions correctly when predicting the next one, two, three, and four trading data


Test your CNN and RNN accuracy over Test Data on which you did not train, to determine how well your neural networks generalize -- specifically, 
in terms of predicting the next one, two, three, and four datapoints in the dataset from 1 Jan 1980 (or whenever your dataset begins)
through the present day (or whenever your dataset ends).  
To determine response to input nonergodicity, it is suggested that you use a sliding sampling window of N datapoints for testing your algorithm, 
sliding the window along the test data and applying your CNN+RNN algorithm to determine how well (at each data point in the Test Data)
your algorithm predicts the next one to four datapoints.  

Accuracy will be computed in terms of error defined as 
prediction_error := (predicted_price - actual_price) / actual_price 

