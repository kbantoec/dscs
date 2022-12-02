## Preprocessing

## Getting familiar with your trading data

### Resampling data
```python
data_daily = data_hour.resample("D").mean()
```