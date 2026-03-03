# 🚀 Classical–Quantum Probabilistic Financial Forecasting

> A unified framework integrating classical machine learning and quantum circuits for probabilistic financial market analysis.

---

## 🧠 Overview

Financial markets are stochastic, nonlinear, and regime-driven.  
Instead of predicting exact prices, this project models **probabilities** across four fundamental market dimensions:

- 📈 Trend Probability
- 🔄 Reversal Probability
- 🌪 Volatility Probability
- 🎯 Bayesian Directional Probability

Each indicator is implemented in **two structurally symmetric versions**:

| Classical Model | Quantum Analog |
|----------------|---------------|
| Logistic Regression | Variational Quantum Circuit (VQC) |
| Random Forest | 4-Qubit Parameterized Circuit |
| Bayesian Frequency Estimation | 2-Qubit Hadamard + CNOT Circuit |

All outputs are normalized to:

P̂ ∈ [0,1]

This enables **direct cross-paradigm comparison** between classical ML and quantum computation.

---

# 📊 Problem Domains Covered

## 1️⃣ Volatility Probability Estimation

Predicts probability of high-volatility regime.

### Classical
- Random Forest
- Features: rolling volatility, ATR, momentum, volume spike, log returns
- Accuracy: 73.19%
- AUC-ROC: 0.589

### Quantum
- 4-qubit parameterized circuit
- Angle encoding: θ = xπ
- CNOT entanglement chain
- Measurement-based probability extraction
- Result: P ≈ 0.951 (high-volatility encoding)

---

## 2️⃣ Trend Probability Indicator (CTPI / QTPI)

Estimates probability of sustained uptrend.

### Classical
- Logistic Regression
- Binary Cross-Entropy optimization
- Deployed in TradingView Pine Script
- Validated on Nifty 50 (1D)

### Quantum
- 3-qubit Variational Quantum Circuit
- Angle encoding of financial features
- Pauli-Z expectation mapping:

P̂ = (1 − ⟨Z⟩) / 2

- Result: P ≈ 0.615

---

## 3️⃣ Reversal Probability Indicator (CRPI / QRPI)

Models probability of trend transition events.

### Classical
- Logistic Regression
- Features:
  - Momentum exhaustion
  - Volatility expansion
  - RSI divergence
  - Volume anomaly
- Validated on Nifty 50 (10-min timeframe)

### Quantum
- 3-qubit VQC (same architecture as QTPI)
- Feature-specific angle encoding
- Result: P ≈ 0.60–0.65

---

## 4️⃣ Bayesian Forecast Indicator (CBFI / QBFI)

Estimates directional probability using rolling frequency counts.

### Classical

P_up = UpMoves / (UpMoves + DownMoves)

- Lookback window: 30
- Nifty 50 result: Pup ≈ 0.60

### Quantum
- 2-qubit circuit
- RY encoding (θ = Pupπ)
- Hadamard superposition
- CNOT entanglement
- Dominant |10⟩ state mapping
- Result: P ≈ 0.50

---

# 🔬 Quantum Implementation

All quantum circuits are implemented and validated in:

- IBM Quantum Composer
- 1,024-shot measurement histograms
- Q-sphere visualization
- Parameter Shift Rule compatibility

Key concepts used:

- Angle Encoding
- Variational Quantum Circuits (VQC)
- CNOT Entanglement
- Pauli-Z Expectation Mapping
- NISQ-compatible architecture

---

# 🏗 Architecture Comparison

| Property | Classical | Quantum |
|-----------|------------|------------|
| Feature Space | Euclidean ℝⁿ | Hilbert Space ℋ²ⁿ |
| Decision Boundary | Linear (LR, Bayes) | Nonlinear (Entanglement) |
| Gradient Method | Backpropagation | Parameter Shift Rule |
| Deployment | TradingView / Python | IBM Quantum |
| Output Semantics | P ∈ [0,1] | P ∈ [0,1] |

---

# 📈 Data Sources

- Nifty 50 (NSE) via TradingView  
  - Daily timeframe (trend & Bayesian)
  - 10-minute timeframe (reversal)
  - Period: Jan 14 – Mar 2, 2026

- Synthetic Data:
  - Geometric Brownian Motion (GBM)
  - 1,000 daily observations
  - Used for volatility modeling

---

# 🧩 Unified Probabilistic Decomposition

The framework models financial uncertainty across orthogonal dimensions:

P_trend + P_reversal + P_neutral = 1

- Trend ≠ Reversal (not complementary)
- Volatility operates on amplitude dimension
- Bayesian provides directional prior

This creates a **multi-dimensional probabilistic market state representation**.

---

# 🚀 Why This Project Matters

- Demonstrates classical–quantum structural symmetry  
- Encodes financial uncertainty probabilistically  
- Provides cross-paradigm benchmarking  
- NISQ-compatible quantum design  
- Fully deployable classical models  

---

# ⚠️ Current Limitations

- Quantum circuits validated under simulation
- Limited live data window
- Volatility module partially uses synthetic GBM data
- Variational parameters not fully optimized on live market data

---

# 🔮 Future Work

- Real hardware execution on IBM Q
- Multi-asset benchmarking
- Hybrid classical–quantum training loop
- Multi-class quantum probability modeling
- Integration with LSTM / Transformer models

---

# 🛠 Tech Stack

- Python
- Scikit-learn
- TradingView Pine Script
- IBM Quantum Composer
- Variational Quantum Circuits

---
# 👥 Contributors

## 🧠 Punith V
- Volatility Probability Estimation (Classical + Quantum)
- Bayesian Forecast Indicator (CBFI / QBFI)
- Quantum circuit architecture design
- Unified framework formulation

## 📈 Rithwik M
- Trend Probability Indicator (CTPI / QTPI)
- Reversal Probability Indicator (CRPI / QRPI)
- Logistic regression modeling
- TradingView Pine Script validation
---

# ⭐ If You Found This Interesting

Give the repo a ⭐ and explore the intersection of:

Finance × Machine Learning × Quantum Computing
