# Analytics-of-Crypto-Metals-and-Property-Markets

<h2>1. Project Title / Headline</h2>
A concise, descriptive name for the dashboard.

📊 Analytics of Crypto, Metals, and Property Markets

An end‑to‑end data analytics and visualization system designed to compare cryptocurrencies, precious metals, and Irish residential property using a unified analytical framework.

<h2>2. Short Description / Purpose</h2>

This project builds a complete data‑engineering and visualization pipeline to help non‑expert investors understand how cryptocurrencies, metals, and property differ in terms of price trends, volatility, drawdowns, and risk‑return characteristics. The system integrates heterogeneous datasets, processes them through a modern ETL pipeline, and presents insights through an interactive Streamlit dashboard.

<h2>3. Tech Stack</h2>

The project was built using the following tools and technologies:

- 🐍 Python – Core language for ETL, data processing, and analytics
  
- 🗄️ MongoDB – Staging layer for raw JSON and CSV ingestion
  
- 🐘 PostgreSQL – Analytical warehouse for cleaned, structured data
  
- ⚙️ Dagster – Orchestration framework for ETL pipelines and data lineage
  
- 📈 Streamlit – Interactive dashboard for visual analytics
  
- 📦 Pandas / NumPy – Data wrangling and numerical computation
  
- 📉 Altair – Declarative charting library for clean, interpretable visuals
  
- 🔗 APIs & Open Data – Binance API, Kaggle datasets, Property Price Register

<h2>4. Data Sources</h2>

The project integrates three heterogeneous datasets:

- Cryptocurrencies (BTC & ETH)
  
- Source: Binance Spot API
  
- Data: OHLCV candlestick data, timestamps, volumes
  
- Precious Metals (Gold & Silver)
  
- Source: Kaggle dataset
  
- Data: Daily gold and silver prices, ratios, currencies
  
- Irish Residential Property
  
- Source: Property Price Register (Government Open Data)
  
- Data: Sale date, county, address, sale price
  
These datasets were selected to represent assets with distinct volatility, liquidity, and risk profiles.


<h2>5. Features / Highlights</h2>

<h3>• Business Problem</h3>

Investors often compare crypto, metals, and property using isolated sources, inconsistent metrics, or anecdotal evidence. This fragmentation makes it difficult to understand:

- How volatile each asset class is
  
- How deep their drawdowns can be
  
- How their long‑term returns compare
  
- Whether crypto behaves like a hedge or a speculative asset
  
- How property prices evolve across counties
  
This project solves that by placing all assets on a common analytical footing.

<h3>• Goal of the Project</h3>

To build a unified, reproducible analytics environment that:

- Ingests heterogeneous financial datasets
  
- Cleans, transforms, and stores them in a structured warehouse
  
- Computes consistent metrics across all asset classes
  
- Visualizes trends, volatility, and risk‑return profiles
  
- Helps users compare investment categories side‑by‑side

<h2>6. ETL Architecture Overview</h2>

The system follows a layered ETL architecture:

- Raw Layer:
  
- Binance API JSON
  
- Kaggle CSV
  
- Property Register CSV
  
- Staging Layer (MongoDB):
  
- Flexible schema‑less storage
  
- Ideal for heterogeneous raw formats
  
- Processing Layer (Python + Pandas):
  
- Cleaning, filtering, type conversions
  
- Log‑return computation
  
- Handling missing values
  
- Warehouse Layer (PostgreSQL):
  
- Normalized tables: crypto_prices, metal_prices, ppr_processed
  
- Uniqueness constraints for data integrity
  
- Orchestration (Dagster):
  
- Software‑defined assets
  
- Dependency tracking
  
- Pipeline scheduling
  
- Data lineage visualization

<h2>7. Walkthrough of Key Visuals</h2>

<h3>📍 Property Visualizations</h3>

- Monthly median sale price (national trend)
  
- County‑wise transaction volume
  
- Top 5 counties by median price (yearly comparison)
  
- Clean, aggregated visuals for long‑term market behaviour

<h3>📍 Metals Visualizations</h3>

- Gold vs Silver (Dual‑Axis Chart)
  
- Indexed performance since 2020
  
- Daily & weekly return histograms
  
- Drawdown curves
  
- Moving averages (50‑day & 200‑day)

<h3>📍 Crypto Visualizations</h3>

- Bitcoin vs Ethereum (Dual‑Axis Chart)
  
- Indexed cumulative performance
  
- Return distributions
  
- Drawdown analysis
  
- Moving average overlays

<h3>📍 Multi‑Asset Analytics</h3>

- Rolling volatility comparison
  
- Annual returns
  
- Approximate 5‑year returns
  
- ARIMA(1,1,1) forecasts with confidence intervals
  
- Sharpe‑like risk‑return metrics

<h2>8. Key Insights</h2>

- Cryptocurrencies
  
- Highest growth potential
  
- Highest volatility
  
- Deepest drawdowns
  
- Precious Metals
  
- Moderate returns
  
- Hedge‑like behaviour
  
- Lower volatility than crypto
  
- Irish Property
  
- Smooth, steady appreciation
  
- Strong regional variation
  
- Low volatility but slower growth

<h2>9. Screenshots / Demos</h2>

Dashboard Overview:

![Dashboard Overview](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/Dashboard%20Overview.png)

Property Visuals:

![Property Visuals](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/Property%20Visuals.png)

Metals Visuals:

![Metals Visuals](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/Metals%20Visuals.png)

Crypto Visuals:

![Crypto Visuals](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/Crypto%20Visuals.png)

Multi-Asset Analytics:

![Multi-Asset Analytics](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/Multi-Asset%20Analytics.png)

Dagster ETL pipeline:

![Dagster ETL pipeline](https://github.com/suyogbrid/Analytics-of-Crypto-Metals-and-Property-Markets/blob/main/ETL%20pipeline.png)




