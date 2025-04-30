# Computational_Methods_4options
Computational Finance exam project modeling option pricing under the Heston stochastic volatility model. Includes Monte Carlo (Euler &amp; QE), Fourier-based methods, implied volatility surface computation, PnL analysis, and VaR estimation under model uncertainty.

# Option Pricing and Risk Analysis under the Heston Model

This repository contains the final project for a Computational Finance exam. It models the evolution of an asset using the **Heston stochastic volatility model** and performs **option pricing**, **PnL analysis**, and **Value at Risk (VaR)** computation.

The project combines:
- Monte Carlo simulation (Euler and Quadratic Exponential schemes)
- Fourier-based pricing (Inverse Fourier Transform, COS, and Carr & Madan FFT)
- Implied volatility surface estimation
- Risk analysis under market model misspecification

## Contents

- `CODE_CF_MarchExam_PnL.ipynb`: Python notebook implementing the entire modeling and analysis pipeline.
- `ReportOptionMthds`: Full written report explaining the methodology, theory, and results.

##  Methodologies Used

###  Heston Model Simulation
- Implements stochastic volatility modeling with CIR process
- Discretized using:
  - Euler-Maruyama scheme
  - Andersen's Quadratic-Exponential (QE) scheme

###  Option Pricing
- Monte Carlo pricing of European put options
- Fourier techniques:
  - Inverse Fourier Transform
  - COS Method
  - Carr & Madan FFT pricing

###  Implied Volatility
- Computed using a bisection algorithm to back out BS volatility from Heston prices
- Surface and smile plots are generated

###  Profit & Loss (PnL) and Value at Risk (VaR)
- PnL estimated from Heston evolution, evaluated using Black-Scholes assumptions
- VaR calculated under implied volatility shifts (±5%, ±10%, ±50%)

## Results Summary
- Pricing methods compared in accuracy and speed
- Implied volatility surface validated against benchmark
- PnL distributions and corresponding VaR values analyzed and visualized

