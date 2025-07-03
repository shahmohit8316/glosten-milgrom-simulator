# 📈 Glosten-Milgrom Simulator

> “Markets reveal information through price — this simulator reveals how.”

A full-scale OCaml implementation of the legendary **Glosten-Milgrom (1985)** market microstructure model. This repo is not a toy project — it's a step toward building **live alpha-generating engines** based on asymmetric information and Bayesian price dynamics.

If Jane Street, Nasdaq, and a PhD in stochastic control had a child — it would look like this.

---

## 🚀 Purpose

This repo simulates an electronic market with **informed traders**, **noise traders**, and **Bayesian market makers**, enabling advanced experimentation with:

- **Belief dynamics**
- **Bid-ask spread evolution**
- **Signal-to-noise interactions**
- **PnL flows for informed agents**

---

## 📁 Folder Structure

| Folder | Description |
|--------|-------------|
| `alpha_extraction/` | Code to compute, visualize, and analyze alpha (e.g., `pnl_analysis.ml`, `alpha_curve.ml`) |
| `core_model/` | Core Glosten-Milgrom mechanics — Bayesian belief updater, bid-ask engine, signal model |
| `math_engine/` | Pure math modules for variance, expectation, and Bayes updates |
| `simulations/` | Realistic scenario scripts (base case, noisy vs informed, signal sweep) |
| `docs/` | Theoretical derivations, model summaries, parameter tables, equations |
| `README.md` | This file

---

## 🧠 Core Concepts Implemented

✅ Bayesian price updates  
✅ Informed vs uninformed flow  
✅ Spread dynamics from signal precision  
✅ Market maker's rational expectations  
✅ Noise masking + liquidity incentives

---

## 🧪 Example Simulations

| Name | File |
|------|------|
| Base Case | `simulations/base_case.ml` |
| Signal-Noise Sweep | `simulations/signal_noise_sweep.ml` |
| Spread PnL Evolution | `alpha_extraction/alpha_curve.ml` |
| Belief Drift | `core_model/belief_update.ml` |

---

## 📊 Outputs You Can Generate

- PnL vs information advantage
- Spread vs noise ratio
- Execution probability heatmaps
- Market maker revenue charts
- Belief timeline animations

---

## 🛠️ Tech Stack

- **Language**: OCaml (100%)
- **Build System**: `dune`, `make`
- **Visualization**: Interfaces with Python/matplotlib or JS frontends (future)
- **Style**: Modular FP + type-safe Bayesian inference

---

## 📦 How to Run

```bash
git clone https://github.com/shahmohit8316/glosten-milgrom-simulator.git
cd glosten-milgrom-simulator

# Build
dune build

# Run a simulation
dune exec simulations/base_case.ml
