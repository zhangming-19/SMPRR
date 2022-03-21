# RRSMP
This repository releases a comprehensive dataset for long-term stock movement prediction from Chinese research reports and historical stock prices. Please cite the following paper [bib] if you use this dataset.


> Stock movement prediction is a challenging problem: the market is highly *stochastic*, and we make *long-term* predictions from *chaotic* data. We treat these three complexities and present a novel long-term stock movement prediction approach based on research reports. In detail, a new Research Report dataset for Stock Movement Prediction (RRSMP) is proposed. RRSMP is one of the few datasets for long-term stock movement prediction, which is mainly composed of long-form, formal, and professional research reports and labeled data. We demonstrate the state-of-the-art performance of our proposed model on the new stock movement prediction dataset which we collected.

You might also be interested in our code for stock movement prediction.

Should you have any query please contact me at [zhangming@hccl.ioa.ac.cn](mailto:zhangming@hccl.ioa.ac.cn).

## Dataset Overview
The research reports between 07/23/2009 and 03/02/2022 are downloaded from the Eastmoney.com, which are publicly available on the web. Correspondingly, the historical prices of related stocks are obtained from the public finance [API](https://tushare.pro/) for the last ten years.

## Data Component
This dataset comprises two main components,

* **./reports**: textual data from [reasearch reports](https://data.eastmoney.com/)
* **./price**: price data from finance [API](https://tushare.pro/)

Each component contains their raw data, preprocessed data, and finished data organized by year,

* **./reports/Raw**
* **./reports/Pre**
* **./reports/Finished**
* **./reports/Modules**

and

* **./price/Raw**

## Data Format

###Raw Research Report Data
Format: PDF

Keys: see more in the [Eastmoney.com](https://data.eastmoney.com/)

##Preprocessed Research Report Data
Format: XLS
Keys: 'Title', 'Links', 'Org.', 'Author', 'Rate', 'Date', 'Text'

###Finished Research Report Data
Format: CSV 
Keys: 'id', 'text', 'category', 'rating'

###Modules Research Report Data
Format: CSV 
Keys: 'id', 'text', 'category', 'rating'

### Raw Price Data
Format: CSV 
Entries: date, open price, high price, low price, close price, adjust close price, volume  








