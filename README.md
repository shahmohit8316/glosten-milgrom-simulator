# glosten-milgrom-simulator
Deep simulation of Glosten-Milgrom microstructure model for $500M+/year alpha extraction

# 🧠 Glosten-Milgrom Alpha Simulator (1985)
> Full-stack, belief-driven, market-making simulation framework designed to extract up to **£200 million/year alpha** under asymmetric information.

---

## 🔥 Purpose

This project simulates the **Glosten-Milgrom (1985)** market microstructure model from first principles.

The simulator models:
- Bayesian market maker belief updates
- Strategic order flow under private information
- Spread formation dynamics under asymmetric risk
- Real-time **alpha extraction** pipelines

> 💡 *Unlike most academic toy examples, this repo evolves toward a live-ready quant engine replicating real-time market dynamics.*

---

## 🧮 Core Ideas

| Concept | Description |
|--------|-------------|
| **Asymmetric Info** | Some agents (insiders) have private knowledge of the true asset value. |
| **Market Maker (MM)** | Sets bid/ask prices based on belief updates after each trade. |
| **Belief Update** | MM uses Bayesian inference to update their estimate of the asset value. |
| **Spread Formation** | Reflects MM’s risk premium due to information asymmetry. |
| **Alpha Opportunity** | Extracted from modeling agent interaction before equilibrium is fully priced in.

---

## 📂 Directory Structure

```bash
glosten-milgrom-simulator/
├── alpha_extraction/       # Real-time alpha curves, PnL computation
├── benchmarks/             # Performance tests, stress tests, adversarial setups
├── config/                 # Tunable parameters: signal noise, MM risk aversion
├── core_model/             # Core files: belief update, signal model, bid/ask engine
├── docs/                   # Theoretical documentation, model derivations
├── experiments/            # Empirical test setups across signal ranges
├── math_engine/            # Bayesian, expectation, variance computation modules
├── simulations/            # Simulation scripts (main loops, multi-agent)
├── visuals/                # Charts, heatmaps, spread visualizations
└── README.md               # This file

