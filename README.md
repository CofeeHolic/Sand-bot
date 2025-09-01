# Trading Bot

This repository contains a Python-based trading bot that uses the Dhan API for trading.

## Setup and Installation

Follow these steps to set up and run the trading bot on a fresh AWS Ubuntu instance.

### 1. Clone the Repository
First, clone this repository to your local machine or server.
```bash
git clone <repository_url>
cd <repository_directory>
```
Replace `<repository_url>` and `<repository_directory>` with the actual URL and directory name.

### 2. Create a Virtual Environment
It is highly recommended to use a virtual environment to manage dependencies.
```bash
python3 -m venv venv
```

### 3. Activate the Virtual Environment
Activate the newly created virtual environment.
```bash
source venv/bin/activate
```

### 4. Install Dependencies
Install all the required Python packages using the `requirements.txt` file.
```bash
pip install -r requirements.txt
```

### 5. Set Environment Variables
The bot requires API credentials and other configuration to be set as environment variables. Create a `.env` file (which is gitignored) or set them directly in your shell.

Required variables:
- `DHAN_DATA_CLIENT_ID`
- `DHAN_DATA_ACCESS_TOKEN`
- `DHAN_SANDBOX_CLIENT_ID`
- `DHAN_SANDBOX_ACCESS_TOKEN`
- `TELEGRAM_BOT_TOKEN`
- `TELEGRAM_CHAT_ID`

### 6. Run the Bot
Once the setup is complete, you can run the bot.
```bash
python trading_bot.py
```
