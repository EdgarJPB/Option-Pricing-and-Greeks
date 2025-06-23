# Option-Pricing-and-Greeks

This project explores and compares multiple option pricing models, including **Black-Scholes**, **Binomial Trees**, **Monte Carlo Simulation**, and **Heston Stochastic Volatility**, along with real-world volatility forecasting via **GARCH(1,1)**. It also computes the **Greeks** for sensitivity analysis.

---

## Objective

Provide a unified framework for pricing European and American options using various models, estimate real-market volatility from historical returns, and compute sensitivity measures (Greeks) for hedging and risk management.

---

## Models Implemented

### 1. **Black-Scholes Model**
- Analytical solution for European options
- Supports calculation of Greeks: Delta, Gamma, Vega, Theta, Rho

### 2. **Binomial Tree Model**
- Handles both European and American options
- Flexible for path-dependent payoffs

### 3. **Monte Carlo Simulation**
- Based on Geometric Brownian Motion (GBM)
- Useful for exotic or path-dependent options

### 4. **Heston Model**
- Stochastic volatility model with mean-reverting variance
- Simulated using Euler-Maruyama scheme

### 5. **Ornstein-Uhlenbeck Process**
- For modeling mean-reverting underlying processes (e.g., interest rates, vol surface)

---

## Volatility Estimation

### 1. **Realized Volatility**
- Rolling standard deviation of recent returns

### 2. **GARCH(1,1) Forecast**
- Predicts future volatility using ARCH effects in time series

### 3. **Blended Volatility**
- Combines realized and GARCH estimates for more stable input

---

## Use Case: TSLA Options

- Option prices calculated at-the-money (ATM) with 6-month maturity
- Volatility derived from TSLA's historical returns
- Interest rates pulled from the 1-year Treasury (FRED: `DGS1`)
- Models compared: Black-Scholes, Binomial Tree, Monte Carlo

---

## Visualizations

- Plot of Black-Scholes option price vs. strike price
- Greeks displayed in console for ATM option
- Price comparisons printed with model breakdown

---
