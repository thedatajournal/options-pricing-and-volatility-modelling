# Options Pricing and Volatility Modelling

A Python-based quantitative finance project focused on derivative valuation, options pricing, volatility estimation, and risk analysis. The project explores analytical and numerical pricing techniques, Monte Carlo simulation, implied volatility, and volatility surface construction.

## Project Overview

Options are financial derivatives whose values depend on the price movements of an underlying asset. Accurate pricing requires mathematical modelling of uncertainty, market volatility, and time-dependent risk.

This project implements multiple options pricing methodologies and compares their numerical behaviour under different market conditions.

## Key Features

### 1. Black-Scholes-Merton Model
- European call and put option valuation.
- Analytical pricing using the Black-Scholes framework.
- Calculation of option sensitivities (Greeks).

### 2. Binomial Tree Model
- Cox-Ross-Rubinstein (CRR) binomial tree.
- European and American option valuation.
- Early exercise analysis.

### 3. Monte Carlo Simulation
- Geometric Brownian Motion (GBM) price simulations.
- Risk-neutral valuation.
- Pricing of path-dependent and exotic options.
- Variance reduction techniques.

### 4. Options Greeks
- Delta
- Gamma
- Vega
- Theta
- Rho

### 5. Implied Volatility
- Numerical implied volatility estimation.
- Newton-Raphson optimisation.
- Brent root-finding fallback.

### 6. Volatility Surface Modelling
- Implied volatility across strike prices and maturities.
- Volatility skew and term structure analysis.
- Three-dimensional volatility surface visualisation.
- Basic static arbitrage diagnostics.

## Technology Stack

- **Language:** Python
- **Numerical Computing:** NumPy, SciPy
- **Data Analysis:** Pandas
- **Visualisation:** Matplotlib
- **Development:** Jupyter Notebook
- **Testing:** Pytest

## Project Structure

```text
options-pricing-volatility-modelling/
│
├── src/
│   ├── simulation.py
│   ├── black_scholes.py
│   ├── binomial.py
│   ├── monte_carlo.py
│   ├── implied_vol.py
│   └── forward_surface.py
│
├── tests/
├── tools/
├── notebooks/
├── requirements.txt
├── compare_ql.py
└── README.md
```

## Installation

Clone the repository:

```bash
git clone <YOUR_REPOSITORY_URL>
cd options-pricing-volatility-modelling
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it:

**Windows**
```bash
.venv\Scripts\activate
```

**macOS / Linux**
```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Explore the notebooks to understand the mathematical foundations, pricing implementations, simulations, and volatility analysis.

Run the test suite:

```bash
pytest -v
```

## Further Development

Planned extensions include:

- SABR stochastic volatility model calibration.
- SVI parameterisation of implied volatility surfaces.
- Implied volatility forecasting using statistical and machine learning models.
- Volatility arbitrage strategy development.
- Delta-hedging and dynamic portfolio rebalancing simulations.
- Historical options data analysis and backtesting.

## References

- John C. Hull — *Options, Futures, and Other Derivatives*.
- Paul Glasserman — *Monte Carlo Methods in Financial Engineering*.
- Jim Gatheral — *The Volatility Surface*.
- Black and Scholes — *The Pricing of Options and Corporate Liabilities* (1973).

---

**Disclaimer:** This project is intended for educational and quantitative research purposes. It does not constitute investment advice or a recommendation to trade financial instruments.
