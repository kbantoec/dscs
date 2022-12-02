## Preprocessing

## Getting familiar with your trading data

### Resampling data
```python
# Supose that data_hour is a pandas DataFrame
data_daily = data_hour.resample("D").mean()
```

### Computing returns
### Discrete returns
```python
# Suppose that stock_data is a OHLCV pandas DataFrame
stock_data["daily_return"] = stock_data["Close"].pct_change()
```