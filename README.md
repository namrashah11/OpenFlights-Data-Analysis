# 🌍 A Network Analysis of Global Connectivity

## 📘 Overview

This project applies **graph theory**, **optimization**, **dynamic programming**, and **machine learning** to analyze the **global airline transportation network** using the **OpenFlights Airports and Routes datasets**. The goal is to uncover key structural patterns, identify major hubs, and derive actionable insights for airlines, logistics, and policy planning.

---

## 👥 Team

**CFA Final Project – MGMT 59000 – Spring 2025**  
Avanti Chandratre, Chhaya Tundwal, Namra Shah

---

## 🗂️ Dataset

The project uses two datasets from OpenFlights:
- `airports.dat`: Contains 7,000+ airports with location and identity attributes.
- `routes.dat`: Contains 60,000+ airline routes connecting airport pairs.

Each record represents a **direct flight**, making it ideal for modeling a **real-world network** of global air connectivity.

---

## 🧠 Analytical Insights & Algorithms

### 1. ✈️ Busiest Airports by Degree Centrality
- **Algorithm**: Degree Centrality (using `networkx.degree()`)
- **Insight**: Frankfurt, CDG, Amsterdam, Atatürk, and Atlanta are the top 5 most connected airports.
- **Business Use**: Leverage Europe’s hub dominance for partnerships and route optimization.

---

### 2. 🛫 Optimal Shortest-Path Connections
- **Algorithm**: Dijkstra’s Algorithm (`networkx.shortest_path_length`)
- **Metric**: Haversine-based distances
- **Insight**: Identified shortest connections like FRA → AMS (367 km) that could serve as express corridors.
- **Business Use**: Build premium shuttle products for frequent business travel.

---

### 3. 🏢 Major Global Hubs by Betweenness Centrality
- **Algorithm**: Approximate Betweenness Centrality (sampled via `networkx.betweenness_centrality`)
- **Insight**: Anchorage and Keflavik, while less busy, are strategic global connectors.
- **Business Use**: Invest in under-the-radar hubs for polar/transatlantic routes and resiliency.

---

### 4. 🕓 Optimized 48-Hour Itinerary (Bitmask DP)
- **Technique**: Dynamic Programming with NumPy
- **Goal**: Maximize airport visits within 48 hours from Frankfurt.
- **Result**: 11 airports across multiple continents can be visited efficiently.
- **Use Case**: Executive travel, logistics planning, or high-value charter routing.

---

### 5. 🧮 Route Optimization with ILP
- **Tool**: Integer Linear Programming using PuLP
- **Goal**: Select 100 routes to cover maximum hubs.
- **Result**: Achieved 75%+ global hub coverage.
- **Use Case**: Route pruning for efficiency or lean startup airline planning.

---

### 6. 🧊 Community Detection via Spectral Clustering
- **Algorithm**: `sklearn.cluster.SpectralClustering`
- **Insight**: Revealed regional clusters (e.g., Arctic, Canada, Alaska, global mix).
- **Business Use**: Tailor equipment and partnerships based on regional subnetworks.

---

### 7. 🌐 Country-Level MST Backbone
- **Algorithm**: Minimum Spanning Tree (`networkx.minimum_spanning_tree`)
- **Goal**: Efficient global connection of all countries
- **Insight**: 225 countries connected with 224 minimum-cost links.
- **Use Case**: Emergency routing, diplomatic corridors, humanitarian airlifts.

---

## 🛠️ Tools & Libraries

- **Python**
  - `networkx` for graph algorithms
  - `NumPy` for dynamic programming
  - `scikit-learn` for clustering
  - `PuLP` for optimization modeling
- **Haversine Formula**: Used for geospatial distance calculations

---

## 💼 Strategic Impact

The project delivers actionable insights for:
- **Airlines**: Optimize global operations, route planning, alliance strategies
- **Logistics & Charters**: Build premium, time-efficient services
- **Governments/NGOs**: Design resilient emergency and trade networks

---

## 📍 Conclusion

This project showcases how **computational methods** can effectively model **complex, global-scale systems** like air transportation networks. From identifying superhubs to crafting 48-hour itineraries, our work illustrates the **real-world power of data science** in infrastructure, logistics, and operations strategy.

---

> _“Data meets the skies: Optimizing connectivity through networks, algorithms, and strategy.”_

