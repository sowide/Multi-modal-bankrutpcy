# Multi-modal-bankrutpcy
A multi-modal bankruptcy dataset from the American stock market. The dataset includes 6190 public companies in the US stock market (New York Stock Exchange and NASDAQ) with data available in the period from 1999 to 2018. 
Two modalities are presented:
- Accounting variables in the form of time series with a length of 3 years
- Items 1,5 and 7 from the SEC annual reports (10-K filings) as text communications with valuable information to predict bankruptcy events for such companies.

According to the Security Exchange 146 Commission (SEC) a company in the American market is considered bankrupt in two cases:
- If the firm’s management files Chapter 11 of the Bankruptcy Code to "reorganize" its business: Management continues to run the day-to-day business operations but all significant business decisions must be approved by a bankruptcy court
- If the firm’s management files Chapter 7 of the Bankruptcy Code: the company stops all operations and goes completely out of business.

When these events occur we label the fiscal year before the chapter filling as "Bankruptcy" (1) for the next year. Otherwise, the company is considered alive (0). he dataset has no missing values or synthetic and imputed added values.

Dataset composition
Each sample of the dataset represents the financial status of a company according to the accounting data of the last 3 financial years and the corresponding two 10-K reports available. In this way, we can leverage both data sources to evaluate the bankruptcy likelihood.

The dataset regarding companies is split into a training set, a validation set, and a test set on a temporal basis as follows:
- The training set refers to the data from 1999 to 2014. It is composed of 2,739 healthy samples and 403 default cases.
- The validation set refers to the data of 2015. It is composed of 206 healthy samples and 27 default cases.
- The test set refers to the data from 2016 to 2019. It is composed of 2,743 healthy samples and 72 default cases.
