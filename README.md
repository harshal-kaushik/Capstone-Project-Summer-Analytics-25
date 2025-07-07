# Capstone-Project-Summer-Analytics-25

# 🚗 Dynamic Pricing for Urban Parking Lots

### Capstone Project | Summer Analytics 2025

---

## 📌 Overview

Urban parking spaces are often underutilized or overcrowded due to static pricing. This project presents a **dynamic pricing engine** for 14 parking spaces using real-time data to update prices based on demand and environmental factors.

The system simulates a smart city scenario where prices are updated every 30 minutes, encouraging efficient usage and reducing congestion. The pricing models are built from scratch using Python, NumPy, and Pandas, and simulate real-time streaming via Pathway.

---

## 🧰 Tech Stack

| Tool/Library | Purpose                              |
| ------------ | ------------------------------------ |
| **Python**   | Core programming language            |
| **NumPy**    | Mathematical computations            |
| **Pandas**   | Data handling & manipulation         |
| **Pathway**  | Real-time data ingestion & streaming |
| **Bokeh**    | Real-time interactive visualizations |
| **Mermaid**  | Architecture diagram (via markdown)  |

---

## 🏗️ Architecture Diagram

```mermaid
graph TD
    A[CSV Dataset] -->|Streaming with Delay| B(Pathway Ingestion)
    B --> C{Feature Engineering}
    C --> D[Model 1: Linear Price]
    C --> E[Model 2: Demand-Based Pricing]
    E --> F[Price Stream Output]
    F --> G[Bokeh Plot: Real-time Price Display]
