# EVM-Token-Analysis-Telegram-Bot

A powerful Telegram bot for real-time analysis of EVM-compatible blockchain tokens, providing detailed insights and analytics for crypto traders, investors, and researchers.

<p align="center">
  <img src="https://github.com/steven228312/EVM-Token-Analysis-Telegram-Bot-Portfolio/blob/main/EVM%20Token%20Analysis%20Bot.gif" alt="Main Menu">
</p>

## 🔍 Overview

This advanced blockchain analytics bot connects to multiple data sources (primarily Dune Analytics) to fetch and analyze token information across Ethereum, Binance Smart Chain (BSC), and Base networks. Users can query comprehensive token information directly through Telegram, making on-chain data analysis accessible and convenient for everyone.

## ✨ Key Features

### Free Features
- **First Buyers & Profits Analysis**: View the first 1-50 wallets that bought a token with detailed statistics including buy & sell amounts, total trades, PNL, and win rate (3 token scans/day)
- **Most Profitable Wallets**: Discover the most profitable wallets holding a specific token, including buy & sell totals and net profit (3 token scans/day)
- **Market Cap & ATH Analysis**: View the all-time high market cap of any token, including ATH date and percentage from ATH (3 token scans/day)

### Premium Features
- **Deployer Wallet Scan**: Reveal the deployer wallet and all tokens deployed by it, including ATH market cap and x-multipliers
- **Top Holders & Whale Watch**: See the top 10 holders and whale wallets of a token, with notifications when Dev, whales, or top 10 holders sell
- **High Net Worth Holders**: Scan for wallets holding over $10,000 worth of a token, including total worth in USD, token amount, and average holding time
- **Unlimited Access**: Premium subscribers get unlimited access to all features

### Technical Features
- **Multi-Chain Support**: Analyze tokens across Ethereum, Binance Smart Chain, and Base networks
- **Intelligent Caching System**: Efficient data retrieval with smart caching to minimize API calls
- **Real-time Updates**: Receive timely information directly in Telegram

## 🚀 Installation

### Prerequisites

- Python 3.8+
- Telegram Bot Token
- Dune Analytics API credentials

### Setup

1. Clone the repository:

```bash
git clone https://github.com/steven228312/EVM-Token-Analysis-Telegram-Bot.git
```

2. Navigate to the project directory:

```bash
cd EVM-Token-Analysis-Telegram-Bot
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Create a `.env` file with your credentials:

```bash
# DB Configuration
MONGODB_URI="mongodb://localhost:27017/"
DB_NAME="evm_token_analysis"

# API Keys
DUNE_API_KEY=your_dune_api_key_here
ZENROWS_API_KEY=your_zenrows_api_key_here
MORALIS_API_KEY=your_moralis_api_key_here

# ===== BLOCKCHAIN CONFIGURATION =====
# Ethereum Mainnet
ETH_PROVIDER_URL=https://mainnet.infura.io/v3/your_infura_key_here
ETH_CHAIN_ID=1
ETH_ADMIN_WALLET=your_admin_wallet_address

# Binance Smart Chain Mainnet
BNB_PROVIDER_URL=https://bsc-dataseed.binance.org/
BNB_CHAIN_ID=56
BNB_ADMIN_WALLET=your_admin_wallet_address

# Subscription Check Interval (in seconds)
CHECK_INTERVAL=60

# TELEGRAM BOT SETTING
TELEGRAM_TOKEN=your_telegram_bot_token_here

# Free tier limits
FREE_TOKEN_SCANS_DAILY=3
FREE_WALLET_SCANS_DAILY=3
FREE_PROFITABLE_WALLETS_LIMIT=5

# Premium tier limits
PREMIUM_TOKEN_SCANS_DAILY=100
PREMIUM_WALLET_SCANS_DAILY=100
PREMIUM_PROFITABLE_WALLETS_LIMIT=50

# Additional API keys
WEB3_PROVIDER_URI=https://mainnet.infura.io/v3/your_infura_key_here
ETHERSCAN_API_KEY=your_etherscan_api_key_here
```

5. Start the bot:

```bash
python src/main.py
```

## 📱 Usage

1. Start a chat with the bot on Telegram
2. Select your desired network (ETH, BSC, or Base)
3. Choose a feature from the menu or send a token address prefixed with the chain identifier:
   - `eth:0x...` for Ethereum tokens
   - `bsc:0x...` for Binance Smart Chain tokens
   - `base:0x...` for Base tokens

4. The bot will respond with detailed analysis about the token based on the selected feature

## 💡 Tips for Best Results
- Always use the correct contract address for tokens
- Select the right network for your token (ETH, BSC, Base)
- For premium features, ensure your subscription is active

## 🔌 API Reference

The bot uses several API endpoints to gather comprehensive blockchain data:

- **Token Deployer Projects**: Fetches all tokens deployed by the same address
- **First Buyers Analysis**: Retrieves data about the earliest token purchasers
- **Profit Analysis**: Calculates profit/loss metrics for token holders
- **Market Cap Data**: Retrieves historical market cap information
- **Holder Analysis**: Identifies and analyzes significant token holders

## 🏗️ Architecture

The application follows a modular architecture:
- API layer for external data sources (primarily Dune Analytics)
- Caching system for performance optimization
- Telegram bot interface for user interaction
- Subscription management for premium features

## 💎 Subscription Model

The bot operates on a freemium model:
- **Free Tier**: Access to basic features with daily usage limits (3 token scans/day)
- **Premium Tier**: Unlimited access to all features including exclusive premium analytics

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the [MIT License](./LICENSE)

## 📞 Contact Information

- Gmail: [steven0822.dev@gmail.com](mailto:steven0822.dev@gmail.com)
- GitHub: [Steven Leal(steven228312)](https://github.com/steven228312)
- Telegram: [@steven228312](https://t.me/steven228312)
- Twitter: [@steven228312](https://twitter.com/steven228312)
- Instagram: [@steven228312](https://www.instagram.com/steven228312/)

## 🔑 Keywords

blockchain analysis, cryptocurrency tracking, token analytics, EVM networks, Ethereum scanner, BSC analysis, Base chain, Telegram crypto bot, crypto trading tools, DeFi analytics, token metrics, market cap tracker, whale watching, token deployer analysis, blockchain intelligence, crypto research platform, profit analysis, holder analysis, on-chain data, smart contract scanner, web3 tools, crypto investment analysis, token scanner, blockchain explorer, crypto API integration, Dune Analytics, Moralis integration, wallet tracking, crypto portfolio management, token security analysis, DEX trading analysis, crypto market intelligence, blockchain data visualization, token price alerts, crypto whale alerts
