# Multi-Agent Cryptocurrency Trading System

A sophisticated cryptocurrency trading system that employs multiple AI agents to analyze market data, generate trading signals, and execute trades automatically.

## Features

- Multi-agent architecture for comprehensive market analysis
- Real-time cryptocurrency data fetching using Yahoo Finance
- Automated trading signal generation
- Performance tracking and analytics
- Learning capabilities to improve trading strategies
- Configurable trading intervals and parameters

## Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/MULTIAGENT-Finance-Advisor.git
cd MULTIAGENT-Finance-Advisor
```

2. Install required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

### Running the Trading System

The system can be run using the following command:

```bash
python run_trading_system.py <symbol> <start_date> <end_date> [--interval] [--output]
```

Parameters:

- `symbol`: Cryptocurrency symbol (e.g., "BTC-USD" for Bitcoin)
- `start_date`: Start date in YYYY-MM-DD format
- `end_date`: End date in YYYY-MM-DD format
- `--interval`: Update interval in seconds (default: 60)
- `--output`: Output CSV file for trading results (default: 'trading_results.csv')

Example:

```bash
python run_trading_system.py BTC-USD 2024-01-01 2024-03-20
```

### Downloading Historical Data

To download historical cryptocurrency data:

```bash
python download_crypto.py <symbol> <start_date> <end_date> [--output]
```

Example:

```bash
python download_crypto.py BTC 2024-01-01 2024-03-20 --output Bitcoin.csv
```

## Project Structure

- `run_trading_system.py`: Main entry point for the trading system
- `continuous_trading_system.py`: Core trading system implementation
- `download_crypto.py`: Utility for downloading historical cryptocurrency data
- `agents.py`: Implementation of various trading agents
- `requirements.txt`: Project dependencies

## Trading Agents

The system employs several specialized agents:

- Financial Agent: Analyzes market data
- Strategy Agent: Develops trading strategies
- Trading Signal Agent: Generates trading signals
- Trading Zone Agent: Identifies optimal trading zones
- Automated Trading Agent: Executes trades
- Learning Agent: Improves trading performance over time

## Performance Tracking

The system tracks various performance metrics:

- Current balance
- Total profit/loss
- Win rate
- Total number of trades

## Disclaimer

This trading system is for educational and research purposes only. Cryptocurrency trading involves significant risk, and past performance does not guarantee future results. Always do your own research and consider consulting with financial advisors before making investment decisions.
