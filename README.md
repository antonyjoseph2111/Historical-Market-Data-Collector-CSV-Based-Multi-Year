
# Historical Market Data Collector (CSV-Based, Multi-Year)

## Overview
This script allows you to download and aggregate historical market data from public archives. The script supports multiple time intervals (1m, 1h, 1d) and can collect data for several years at once, compiling it into a single CSV file for analysis.

## Features
- **No API required**: Data is downloaded directly from public archives.
- **Multiple time intervals**: Collect data in 1-minute, hourly, or daily intervals.
- **Multi-year data**: Collect years' worth of market data at once.
- **Data cleaning**: Automatically processes, extracts, and saves the data into a CSV file.

### Install Dependencies
You need to install the required libraries:
```bash
pip install requests pandas
```

## Setup & Configuration

### 1. Copy The Code To Colab And Run It.Edit the Changes As Per Your Need. I will attach all trade pairs in the main repo

### 2. Configure the Script

- `symbol`: Set to the trading pair you want (e.g., `BTCUSDT`, `ETHUSDT`).
- `interval`: Choose the time interval (e.g., `1m`, `1h`, `1d`).
- `years`: Specify the list of years for which you want to download data.

```python
symbol = 'BTCUSDT'      # You can use anything in the list attached to the repo'
interval = '1m'         # Example: '1m', '1h', '1d'
years = [2022, 2023]    # Example: [2021, 2022, 2023] You can add years to the list in the given code
```


### 4. Output File
The script will save the combined data to a CSV file. The filename will follow the pattern:
```
{symbol}_{interval}_{start_year}_{end_year}.csv
```
Example:
```
BTCUSDT_1m_2022_2023.csv
```

The CSV file will contain columns such as:
- `timestamp`
- `open`
- `high`
- `low`
- `close`
- `volume`
- `quote_asset_volume`
- `number_of_trades`
- `taker_buy_base_volume`
- `taker_buy_quote_volume`

## Customization

You can customize the script further by modifying the configuration section:
- **symbol**: Change the symbol to any supported trade pair (e.g., `ETHUSDT`, `BNBUSDT`).
- **interval**: Supported intervals are `1m`, `1h`, and `1d`.
- **years**: Modify the list of years for which you want to download the data.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
