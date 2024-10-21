# stocks-ml-project

## Schedule
![image](https://github.com/user-attachments/assets/859f2099-6de2-483d-b0d6-633352282a4f)

### Code to get dataset
```
import yfinance as yf
import datetime

# Set the stock symbol and date range
stock_symbol = 'AAPL'
start_date = '2000-01-01'
end_date = datetime.datetime.today().strftime('%Y-%m-%d')

# Fetch the stock data
data = yf.download(stock_symbol, start=start_date, end=end_date)

# Save the data to a CSV file
csv_filename = f'{stock_symbol}stock_data_2000_to{end_date}.csv'
data.to_csv(csv_filename)

print(f"Stock data for {stock_symbol} from {start_date} to {end_date} has been saved to {csv_filename}")

```

### Reference projects having simple time series predictions with explanation
- https://github.com/gabrielmayers/apple_stocks_forecasting?tab=readme-ov-file
- https://github.com/kavehbc/market-forecast
