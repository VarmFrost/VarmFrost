# Hi, I'm Leo

Building financial ML systems from first principles — from raw market data to working neural networks.

## FinancialML-dev

**[FinancialML-dev](https://github.com/FinancialML-dev)** is my organization for quantitative finance and machine learning projects.

### Projects

**[onboarding](https://github.com/FinancialML-dev/onboarding)** — PyTorch fundamentals series  
A progressive series of focused examples covering the core concepts behind every neural network:
autograd → linear regression → single neuron → overfitting → gradient descent → batch normalization.

**[financialProject](https://github.com/FinancialML-dev/projects)** — Crypto price direction predictor  
A full supervised ML pipeline built on BTC/USD data from the Alpaca API:
- Fetches and visualizes OHLCV candlestick data
- Constructs dollar bars (inspired by Lopez de Prado's *Advances in Financial Machine Learning*) for more information-rich sampling than fixed time intervals
- Engineers features: using sliding-window return sequences, rolling volatility, RSI, moving average deviation, order flow imbalance (OFI)
- Trains a 3-layer neural network to predict next candle direction (up/down)
- Evaluates with accuracy, precision, recall, F1, and confusion matrix

## Tech Stack

- **Language:** Python
- **ML:** PyTorch, NumPy, pandas, scikit-learn
- **Finance:** Alpaca API, alpaca-py
- **Visualization:** Plotly, Matplotlib
- **Environment:** uv

## Connect

- [LinkedIn](https://www.linkedin.com/in/leonard-soukka-489657b/)
