# RRSMP
This repository releases a comprehensive dataset for long-term stock movement prediction from Chinese research reports and historical stock prices. Please cite the following paper [bib] if you use this dataset,

You might also be interested in our code for stock movement prediction.

Should you have any query please contact me at zhangming@hccl.ioa.ac.cn.

# Dataset Overview
The research reports between 07/23/2009 and 03/02/2022 are downloaded from the Eastmoney.com, which are publicly available on the web. Correspondingly, the historical prices of related stocks are obtained from the public finance API (https://tushare.pro/) for the last ten years.

# Data Component
This dataset comprises two main components,

(1) ./reports: textual data from reasearch reports
(2) ./price: price data from Yahoo Finance
Each component contains their raw data and preprocessed data organized by stocks,
#
##
./tweet/raw
./tweet/preprocessed
and

./price/raw
./price/preprocessed
Data Format
