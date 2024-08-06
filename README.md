# Multi-modal-bankrutpcy
A multi-modal bankruptcy dataset from the American stock market. The dataset includes 6190 public companies in the US stock market (New York Stock Exchange and NASDAQ) with data available in the period from 1999 to 2018. 
Two modalities are presented:
- Accounting variables in the form of time series with a length of 3 years
- Items 1,5 and 7 from the SEC annual reports (10-K filings) as text communications with valuable information to predict bankruptcy events for such companies.

Dataset composition
Each sample of the dataset represents the financial status of a company according to the accounting data of the last 3 financial years and the corresponding two 10-K reports available. In this way, we can leverage both data sources to evaluate the bankruptcy likelihood.

The dataset regarding companies is split into a training set, a validation set, and a test set on a temporal basis as follows:
a) The training set refers to the data from 1999 to 2014. It is composed of 2,739 healthy samples and 403 default cases.
b) The validation set refers to the data of 2015. It is composed of 206 healthy samples and 27 default cases.
c) The test set refers to the data from 2016 to 2019. It is composed of 2,743 healthy samples and 72 default cases.
