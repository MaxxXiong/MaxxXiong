# 🏛️ STEVEN: Systemic Tactical Economic Volatility Engine Network

![License](https://img.shields.io/badge/License-Proprietary-red.svg?style=flat-square)
![Build](https://img.shields.io/badge/Build-Passing-00FF00.svg?style=flat-square)
![Uptime](https://img.shields.io/badge/Uptime-99.99%25-brightgreen.svg?style=flat-square)

**STEVEN** is a high-performance quantitative framework designed for automated futures trading and macro-economic hedging. It leverages recursive Bayesian estimation to predict volatility spikes in leveraged derivatives markets.

---

### 🧬 Core Logic
STEVEN operates on three primary layers to ensure capital preservation during tail-risk events:

1.  **Macro Overlay:** Aggregates real-time fiscal data and yield curve inversions.
2.  **Liquidity Scraper:** Monitors order book depth and liquidation clusters in futures markets.
3.  **Execution Layer:** Deploys capital using a dynamic Kelly Criterion for optimal position sizing.

---

### 📊 Technical Specifications

| Component | Architecture | Purpose |
| :--- | :--- | :--- |
| **Engine** | Rust (Low-Latency) | Sub-millisecond order execution. |
| **Analysis** | Python / Pandas | Statistical arbitrage and mean reversion. |
| **Risk** | C++ | Monte Carlo simulations for VaR (Value at Risk). |
| **Storage** | TimescaleDB | High-velocity time-series economic data. |

---

### 🚀 Implementation (CLI)

To initialize the STEVEN environment and begin the data ingestion cycle:

```bash
# Clone the private repository
git clone [https://github.com/GarrettBullish/STEVEN.git](https://github.com/GarrettBullish/STEVEN.git)

# Initialize the Macro-Environment variables
export LEVERAGE_LIMIT=10x
export RISK_TOLERANCE=AGGRESSIVE

# Boot the engine
./steven --mode automated --asset BTC-PERP --strategy mean-reversion
