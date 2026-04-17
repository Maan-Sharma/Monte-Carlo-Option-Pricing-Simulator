# 📊 Monte Carlo Option Pricing Simulator

## 📌 What is this project about?

This project is a **professional financial simulator** for pricing **European Call and Put options** using **Monte Carlo methods**.

It simulates stock price paths using **Geometric Brownian Motion (GBM)**, compares Monte Carlo results with **Black-Scholes analytical pricing**, and visualizes everything with clean, animated plots.

Built for:

* 📈 Finance learners
* 🎓 Students
* 🔬 Research & experimentation

---

## 👨‍💻 Developer / Creator

**MANN-Sharma**

---

## 🚀 Features

* Simulate stock price paths using GBM
* Price European Call & Put options via Monte Carlo
* Compute Black-Scholes analytical prices
* Animated visualization of stock paths & pricing
* Clean, professional dark-themed interface

---

## 📁 Project Structure

```
├── main.py          # Entry point (simulation + visualization)
├── utils.py         # Core logic (GBM + pricing functions)
├── requirements.txt # Dependencies
├── README.md        # Documentation
```

---

## 📐 Mathematical Models

### 📉 Geometric Brownian Motion (GBM)

Stock price evolution:

[
S_t = S_0 \exp\left((r - 0.5\sigma^2)t + \sigma W_t\right)
]

Where:

* ( S_t ): Stock price at time ( t )
* ( S_0 ): Initial stock price
* ( r ): Risk-free rate
* ( \sigma ): Volatility
* ( W_t ): Wiener process (Brownian motion)

---

### 📊 Black-Scholes Formula

**Call Option:**
[
C = S_0 N(d_1) - K e^{-rt} N(d_2)
]

**Put Option:**
[
P = K e^{-rt} N(-d_2) - S_0 N(-d_1)
]

Where:
[
d_1 = \frac{\ln(S_0/K) + (r + 0.5\sigma^2)t}{\sigma\sqrt{t}}
]
[
d_2 = d_1 - \sigma\sqrt{t}
]

* ( N(\cdot) ): Standard normal CDF
* ( K ): Strike price
* ( t ): Time to maturity

---

## ⚙️ Usage

### 1. Install dependencies

```
pip install -r requirements.txt
```

### 2. Run the simulator

```
python main.py
```

---

## 🎛️ Parameters

You can customize:

* Strike Price
* Volatility
* Risk-Free Rate
* Time to Maturity

All parameters are clearly labeled and visualized in the plots.


## ⭐ Future Improvements (Optional Ideas)

* Add Greeks calculation (Delta, Gamma, Vega)
* Support American options
* Add real market data integration
* Build a web app interface

---
