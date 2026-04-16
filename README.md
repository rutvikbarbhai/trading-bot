
# Binance Futures Testnet Trading Bot

A Python CLI trading bot for placing Market, Limit, and Stop orders on Binance Futures Testnet (USDT-M).

## Features
Market and Limit orders
Bonus: Stop order
BUY / SELL support
CLI using argparse
Input validation
Logging to file
Error handling
Modular code structure

## Project Structure
trading_bot/
├── bot/
│   ├── client.py
│   ├── orders.py
│   ├── validators.py
│   └── logging_config.py
├── logs/
├── cli.py
├── requirements.txt
└── README.md

## Setup
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

Create .env file:

API_KEY=your_testnet_api_key
API_SECRET=your_testnet_secret_key

Use Binance Futures Testnet keys from-

https://testnet.binancefuture.com

## Usage
### Market Buy
python3 cli.py --symbol BTCUSDT --side BUY --type MARKET --qty 0.001
### Limit Sell
python3 cli.py --symbol BTCUSDT --side SELL --type LIMIT --qty 0.001 --price 150000
### Stop Buy
python3 cli.py --symbol BTCUSDT --side BUY --type STOP --qty 0.001 --price 120000

## Logs
Logs are stored in: logs/app.log

## Tech Stack
Python 3
python-binance
python-dotenv
argparse
logging

## Author

Shalmali Bichkar