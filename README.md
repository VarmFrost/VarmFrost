# Hi, I'm Leo

Building financial ML systems from first principles — from raw market data to working neural networks.

## FinancialML-dev

**[FinancialML-dev](https://github.com/FinancialML-dev)** is my organization for quantitative finance and machine learning projects.

### Projects

**[onboarding](https://github.com/FinancialML-dev/onboarding)** — PyTorch fundamentals series  
A progressive series of focused examples covering the core concepts behind every neural network:
autograd → linear regression → single neuron → overfitting → gradient descent → batch normalization.

**[financialProject](https://github.com/FinancialML-dev/projects)** — Crypto price direction predictor  
A full supervised ML pipeline built on ETH/USD data from the Alpaca API, implementing Lopez de Prado's *Advances in Financial Machine Learning*:
- Fetches and visualizes OHLCV candlestick data
- Constructs dollar bars (information-based sampling) — 9.21x compression vs raw minute bars
- Engineers 10 features: returns, volatility, RSI, MA(20) deviation, intra-bar momentum, bar range, VWAP deviation, order flow imbalance (OFI), MA(200) long-term context, ADX trend strength
- Trains two model architectures to predict next candle direction (up/down):
  - Feedforward baseline — 3-layer Multi-Layer Perceptron (MLP) — "what values are in this window?"
  - LSTM — stacked sequence model that captures temporal patterns across the lookback window. — "what happened across this window over time?"
- Mini-batch training with early stopping and best-weight restore
- **Best accuracy:** 53.08% ± 0.0007 (ETH/USD, LSTM + 200MA + ADX, $25K threshold)
- Walk-forward backtest: **191.58% gross return** vs 30.24% buy-and-hold
- Monte Carlo permutation test: **p=0.035** — statistically significant directional edge
- Evaluates with accuracy, precision, recall, F1, confusion matrix

## Tech Stack

- **Language:** Python
- **ML:** PyTorch, NumPy, pandas, scikit-learn
- **Finance:** Alpaca API, alpaca-py
- **Visualization:** Plotly, Matplotlib
- **Environment:** uv

## Connect

- [LinkedIn](https://www.linkedin.com/in/leonard-soukka-489657b/)
