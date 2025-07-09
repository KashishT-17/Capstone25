#  Urban Parking Dynamic Pricing Model

##  Overview

This project simulates a dynamic, real-time pricing system for 14 urban parking spaces using real-world constraints. It adjusts prices based on:
- Demand fluctuations
- Queue length
- Vehicle type
- Nearby traffic
- Special events
- Competitive pricing (nearby lots)

 The goal is to optimize utilization and revenue through intelligent, explainable pricing strategies — all built **from scratch** using only `NumPy`, `Pandas`, `Bokeh`, and `Pathway`.

---

##  Tech Stack

| Component       | Description                                      |
|----------------|--------------------------------------------------|
|  Python       | Core language for model implementation           |
|  Pandas       | Data manipulation and preprocessing              |
|  NumPy        | Numerical operations and vectorization           |
|  Bokeh        | Real-time data visualization                     |
|  Pathway      | Real-time data streaming (simulated)             |
|  Google Colab | Interactive notebook environment                 |

---

##  Architecture Diagram (Mermaid)

```mermaid
flowchart TD
    A[Raw CSV Data (73 days)] -->|Preprocessing| B[Cleaned & Sorted Dataset]
    B --> C[Model 1: Linear Pricing]
    B --> D[Model 2: Demand-Based Pricing]
    D --> E[Model 3: Competitive Adjustment]
    E --> F[Real-Time Pricing Predictions]
    F --> G[Visualized via Bokeh]
    G --> H[Insights + Submission]
