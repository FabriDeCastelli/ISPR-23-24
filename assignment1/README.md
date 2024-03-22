## Signal Processing 

Consider the following dataset: https://archive.ics.uci.edu/dataset/360/air+quality

This is a multivariate timeseries,  where features represent measurement from different air quality sensors (every hour for a year). There are missing values marked with value -200. For this reasons I suggest to discard feature NMHC(GT) as it has far too many missing values. For the other features (sensors), handle the missing value by imputation: e.g. use the average value between the preceeding and the following observation or, if many missing value are in a row, copy the measurament from the same sensor, same time, but the day before (or after, up to you).

Analyse the correlation of the sensor measurements by computing the cross-correlation between the timeseries corresponding to different sensors. Are there sensors wich are more correlated? Are there sensors which are less correlated? Report your considerations on the analysis.