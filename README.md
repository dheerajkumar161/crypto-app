# Crypto Price App 📈

A real-time cryptocurrency price tracking and analysis web application built with Streamlit. This app retrieves live cryptocurrency data from CoinMarketCap and provides interactive visualizations, historical price analysis, and market insights.

## 🚀 Features

- **Real-time Data**: Live cryptocurrency prices and market data from CoinMarketCap
- **Interactive Visualizations**: 
  - Bar charts showing price changes (1h, 24h, 7d)
  - Market cap comparisons
  - Market share pie chart (Bitcoin, Ethereum, Alt Coins)
  - Historical price trends (30-day line charts)
- **Multi-currency Support**: View prices in USD or BTC
- **Customizable Selection**: Choose from 100+ cryptocurrencies
- **Data Export**: Download selected cryptocurrency data as CSV
- **Responsive Design**: Full-width layout with sidebar controls

## 📊 Data Sources

- **Primary Data**: [CoinMarketCap](https://coinmarketcap.com) - Live cryptocurrency prices and market metrics
- **Historical Data**: Cryptocurrency historical market price data via `cryptocmd` library

## 🛠️ Technologies Used

- **Frontend**: Streamlit
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Web Scraping**: BeautifulSoup, Requests
- **Cryptocurrency Data**: cryptocmd library

## 📋 Prerequisites

- Python 3.7 or higher
- pip (Python package installer)
- Internet connection for real-time data fetching

## 🔧 Installation

### Option 1: Using pipenv (Recommended)

1. **Clone or download the project files**
   ```bash
   git clone <repository-url>
   cd crypto_price_app
   ```

2. **Run the installation script**
   ```bash
   chmod +x installations.sh
   ./installations.sh
   ```

3. **Install required packages**
   ```bash
   pipenv install streamlit pandas matplotlib seaborn beautifulsoup4 cryptocmd pillow
   ```

### Option 2: Manual Installation

1. **Create a virtual environment**
   ```bash
   python -m venv crypto_env
   source crypto_env/bin/activate  # On Windows: crypto_env\Scripts\activate
   ```

2. **Install required packages**
   ```bash
   pip install streamlit pandas matplotlib seaborn beautifulsoup4 cryptocmd pillow
   ```

## 🚀 Usage

1. **Activate your environment**
   ```bash
   # If using pipenv
   pipenv shell
   
   # If using virtual environment
   source crypto_env/bin/activate  # On Windows: crypto_env\Scripts\activate
   ```

2. **Run the application**
   ```bash
   streamlit run crypto_price_app.py
   ```

3. **Open your browser**
   - The app will automatically open at `http://localhost:8501`
   - If it doesn't open automatically, navigate to the URL manually

## 📱 How to Use the App

### Sidebar Controls
- **Currency Selection**: Choose between USD or BTC for price display
- **Cryptocurrency Selection**: Multi-select from available cryptocurrencies (default: BTC, ETH, ADA, DOGE, BNB)
- **Time Frame**: Select percentage change time frame (1h, 24h, 7d)

### Main Dashboard
- **Price Change Bar Chart**: Visualizes top gainers/losers and selected cryptocurrencies
- **Market Cap Chart**: Compares market capitalization of selected cryptocurrencies
- **Market Share Pie Chart**: Shows Bitcoin, Ethereum, and Alt Coins market dominance
- **Historical Price Chart**: 30-day price trend for any selected cryptocurrency
- **Data Tables**: Detailed price and percentage change data with CSV download option

## 📁 Project Structure

```
crypto_price_app/
├── crypto_price_app.py    # Main application file
├── installations.sh       # Installation script
├── logo.png              # App logo
└── README.md             # This file
```

## 🔍 Key Features Explained

### Real-time Data Loading
- Web scrapes CoinMarketCap for live cryptocurrency data
- Caches data for 24 hours to improve performance
- Handles API rate limiting gracefully

### Interactive Visualizations
- **Color-coded charts**: Green for positive changes, red for negative
- **Responsive design**: Charts adapt to different screen sizes
- **Dynamic labels**: Market cap units automatically adjust based on values

### Data Export
- Download selected cryptocurrency data as CSV
- Includes price, market cap, volume, and percentage change data

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 🙏 Acknowledgments

- **Data Source**: [CoinMarketCap](https://coinmarketcap.com) for providing cryptocurrency data
- **Web Scraping Inspiration**: Adapted from the Medium article *[Web Scraping Crypto Prices With Python](https://towardsdatascience.com/web-scraping-crypto-prices-with-python-41072ea5b5bf)* by [Bryan Feng](https://medium.com/@bryanf)
- **Libraries**: Streamlit, Pandas, Matplotlib, Seaborn, BeautifulSoup, and cryptocmd communities

## ⚠️ Disclaimer

This application is for educational and informational purposes only. Cryptocurrency investments carry significant risk, and past performance does not guarantee future results. Always do your own research and consult with financial advisors before making investment decisions.

