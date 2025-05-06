# Crypto Trading Signal Bot

This bot scans Binance markets using technical indicators and candlestick patterns, sends alerts to Telegram, and logs signals to Google Sheets.

## 🚀 Features
- Scans symbols across 4h, 1d, 1w timeframes
- RSI, MACD, volume spike filters
- Detects bullish candlestick patterns (Hammer, Engulfing, Morning Star)
- Sends alerts to Telegram with chart images
- Logs signals to Google Sheets

## 🛠 Setup

1. Clone this repo and deploy to [Railway](https://railway.app)
2. Set these environment variables in Railway:
   - `TELEGRAM_TOKEN`
   - `TELEGRAM_CHAT_ID`
   - `GOOGLE_CREDS_JSON` (paste entire service account JSON)

3. No secrets should be hardcoded — use `.env.example` as a reference.

## 📦 Installation (Locally)
```bash
pip install -r requirements.txt
python bot.py
```

## 📄 Files
- `bot.py`: Main bot logic
- `patterns.py`: Candlestick pattern functions
- `requirements.txt`: Python dependencies
- `.env.example`: Example config (no secrets)
- `.gitignore`: Files to exclude from version control
