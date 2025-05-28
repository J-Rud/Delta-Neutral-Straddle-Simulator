# Delta-Neutral Options Trading Simulator

This project simulates a delta-neutral long straddle options strategy using the Black-Scholes model and dynamic delta hedging. It evaluates how daily rebalancing affects the profit/loss of the portfolio over one year using SPY.

## Strategy Summary

- **Position**: Buy 1 call + 1 put (ATM, same expiry) = Long straddle
- **Delta-Neutral**: Offset options' combined delta with SPY positions
- **Goal**: Profit from large movements in SPY regardless of direction

## Features

- Prices call/put options using the Black-Scholes formula
- Simulates SPY price path using geometric Brownian motion
- Recalculates delta daily and rebalances with SPY shares
- Tracks portfolio value and visualizes cumulative P&L

## Files

- `delta_neutral_simulation.py`: Main simulation script
- `requirements.txt`: Install dependencies with `pip install -r requirements.txt`

## Getting Started

Clone the repo and run the simulation:
```bash
pip install -r requirements.txt
python delta_neutral_simulation.py
