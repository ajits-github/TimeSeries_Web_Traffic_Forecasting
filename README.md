# TimeSeries_Web_Traffic_Forecasting
Forecasting future web traffic for approximately 145,000 Wikipedia articles

This project focuses on the problem of forecasting the future values of multiple time series, as it has always been one of the most challenging problems in the field. More specifically, it aims to test state-of-the-art methods to forecast future web traffic for approximately 145,000 Wikipedia articles.

Sequential or temporal observations emerge in many critical real-world problems, ranging from biological data, financial markets, and weather forecasting, to audio and video processing. The field of time series encapsulates many different issues, ranging from analysis and inference to classification and forecast. What can we do to help predict future views?

The training dataset consists of approximately 145k time series. Each of these time series represents a number of daily views of a different Wikipedia article, starting from July, 1st, 2015 up until December 31st, 2016.
For each time series, the name of the article, as well as the type of traffic that these time series represent (all, mobile, desktop, spider), are provided. We may use this metadata and any other publicly available data to make predictions. Unfortunately, the data source for this dataset does not distinguish between traffic values of zero and missing values. A missing value may mean the traffic was zero or that the data is not available for that day.

**File descriptions:**

* train_*.csv - contains traffic data. This a csv file where each row corresponds to a particular article and each column correspond to a particular date. Some entries are missing data. The page names contain the Wikipedia project (e.g. en.wikipedia.org), type of access (e.g. desktop) and type of agent (e.g. spider). In other words, each article name has the following format: 'name_project_access_agent' (e.g. 'AKB48_zh.wikipedia.org_all-access_spider').
* key_*.csv - gives the mapping between the page names and the shortened Id column used for prediction
