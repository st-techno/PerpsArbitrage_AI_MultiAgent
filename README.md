# Copyright @ ST Technologies

## PerpsArbitrage_AI_MultiAgent

Perps Arbitrage using AI MultiAgent CrewAI Framework on Binance, BitMEX and OKX

## Production-Grade Features

Logging: Uses loguru for granular, structured logs.

Secure Credentials: API keys loaded via .env (never hardcoded).

Health Checks: On startup, ensures all exchange connections are live.

Graceful Shutdown: Handles SIGINT/SIGTERM for safe exit.

Error Handling: All critical sections wrapped with try/except and logging.

Rate Limiting: Respects exchange API rate limits.

Compliance: KYC, AML, and position size checks before every trade.

PnL & KPI Reporting: Real-time reporting of PnL and Sharpe ratio.

RL Model: Continuously retrained on latest trade history.

MEV Protection: Placeholder for Flashbots/private tx (extendable).

Extensible: Modular agents, easy to add new exchanges, features, or reporting.

# Dependencies:

bash
pip install crewai ccxt web3 tensorflow pandas sklearn requests python-dotenv loguru

# .env 

BINANCE_API_KEY=your_binance_key
BINANCE_SECRET=your_binance_secret
BITMEX_API_KEY=your_bitmex_key
BITMEX_SECRET=your_bitmex_secret
OKX_API_KEY=your_okx_key
OKX_SECRET=your_okx_secret
OKX_PASSPHRASE=your_okx_passphrase
GLASSNODE_KEY=your_glassnode_key
