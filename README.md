# Timeseries-anomaly-detection
Detection of abnormal patterns in electricity usage via time series forecasting

The test and train data consists of seven years of electric usage for a mixed research/office facility logged in 15 minute intervals along with outside temperatures.

The pipeline consists of data cleaning, one step ahead time series forecasting, calculation of an acceptable intervals for the subsequent real data, and then flagging two classes of anomalies. The first class consists of instantaneous anomalies where the point directly falls outside the acceptabled statistical interval, and the second type consists of sustained anomalies such that the sum of the difference (integrated diference) from the prediction over a short time interval is statistically unlikely.

The performance is tested by assessment of the anomalies it identifies in the real life data and on artificial anomalies added to the data.
