# VapeLabs Auto Bot

An automated bot for TheVapeLabs airdrop platform that handles battery tapping and daily missions automatically.

## Register [HERE](https://app.thevapelabs.io/login?ref=27fd7d5c-0117-44da-8841-7dd1e780494c)

- Connect With Telegram

## Features

- ✅ Auto-tapping battery when below 50% until it reaches 100%
- ✅ Multi-account support with token-based authentication
- ✅ Proxy support for rotating IPs
- ✅ Daily check-in automation
- ✅ Automatic mission completion
- ✅ Interactive terminal UI with real-time status updates
- ✅ Auto-switching between accounts for monitoring

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/BidyutRoy2/TheVapeLabs.git
   cd TheVapeLabs
   ```

2. Install dependencies:
   ```bash
   npm install
   ```
3. Enter Your Access Token & Save `tokens.txt` File
```
nano tokens.txt
```
![image](https://github.com/user-attachments/assets/504b717d-67cf-42b5-841c-4c8d7dc54590)

4. Run the bot:
   ```
   npm start
   ```
## Stop Bot Type - q

## Configuration

### Token Setup

There are two ways to set up your VapeLabs tokens:

#### Option 1: Using tokens.txt file (Recommended)

Create a `tokens.txt` file in the root directory and add one token per line:

```
token1_here
token2_here
token3_here
```

#### Option 2: Using .env file

Create a `.env` file in the root directory and add your tokens:

```
TOKEN_1=your_first_token_here
TOKEN_2=your_second_token_here
TOKEN_3=your_third_token_here
```

### Proxy Setup (Optional)

Create a `proxies.txt` file in the root directory and add one proxy per line in the format `ip:port` or `ip:port:username:password`:

```
http://123.45.67.89:8080
http://username:password@ip:port
```

## Usage

The bot features an interactive terminal UI:

- Use **Arrow Keys** (← →) to navigate between accounts
- Press **Q** to quit the bot

### Battery Tapping Logic

- When battery is **below 50%**, the bot will automatically tap (5 taps every 20 seconds) until it reaches 100%
- When battery is **100%**, the bot will wait until it drops below 50% to start tapping again
- When battery is **between 50% and 100%**, the bot will wait until it drops below 50%

## Troubleshooting

- If you're experiencing rate limiting (429 errors), consider:
  - Adding more proxies to `proxies.txt`
  - Increasing the delay between requests

## Disclaimer

This project is for educational purposes only. Use at your own risk. The developers are not responsible for any consequences that may arise from using this bot.
