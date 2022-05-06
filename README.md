# **Bitcoin Exchanges Arbitrage Opportunities**
---
Module 3 I compared bitcoin prices between exchanges Bitstamp and Coinbase between the timeframe of 01-01-2018 to 
03-31-2018. I then specifically looked into 3 seperate dates, 1 from each month, to anaylize aritrage trading opportunities
that covered 1% trading fees.
---
## Technologies

Python
- [Pandas]
- [Pathlib]
- [Matplotlib]

---
## Installtion guide
- ```import pandas as pd```

- ```from pathlib import Path```

- ```%matploblib inline```

---
##  Usage
1. Collect the data
 - Import data from bitstamp.csv and coinbase.csv files using Pandas read_csv function. 
 - Set the index to a timestamp column and close column
2. Prepare the Data
 - Clean the dataframes for both exchanges
 - replace or drop all ```Nan``` or missing values in dataframs
 - Use ```str.replace``` to remove $ from Close column
 - Convert teh data type of the Close column to ```float```
 - Drop duplicated values if necessary
3. Analyze the Data
 - In Close column use ```.describe``` to get the summary stats of the three dates
 - Then use ```.plot``` to seek arbritage trading moments
 - Between the three specific dates calculate the arbitrage profits
---
### Contributors
Daniel Boyne
---
