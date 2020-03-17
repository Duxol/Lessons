# API Keys  
BarChart API Key:  
8547ccf034a6743d7c8c847977840b90  

Alpha Vantage API Key:  
5X4QL9J3BULDXOQR


# How to use Alpha Vantage in Python:  

```
from alpha_vantage.timeseries import TimeSeries`  
ts = TimeSeries(API_KEY)`  
dictionary, meta = ts.get_monthly(symbol=ticker)
```  

Alpha Vantage API returns values as a nested dictionary!!!

`get_monthly()` returns a date in this format "2018-01-31"

This means that it gets data from the **FIRST** day of that month (i.e. 1st of January) despite the date being 2018-01-31

