# Electric Vehicle Routing Optimization

## Overview
This project develops a **capacitated vehicle routing optimization model** for an electric shuttle service, integrating **demand, capacity, and energy constraints**.  
The goal is to design efficient delivery routes while considering **battery limitations** and **charging requirements**, ensuring reliability and minimal operational cost.

The model is formulated and solved using **Python (PuLP)**, leveraging linear programming techniques to optimize route assignments and minimize total travel distance and time.

---

## Problem Description
Electric vehicles (EVs) present new challenges in logistics optimization due to limited battery capacity and the need for charging schedules.  
This project addresses:
- **Energy-aware routing** — routes must satisfy vehicle range and charging needs  
- **Capacity constraints** — each vehicle has limited load capacity  
- **Demand variability** — customers or service points have different demands  
- **Solver efficiency** — complex constraints are linearized for faster optimization  

---

## Methodology
1. **Data Preparation**  
   Input data includes node coordinates, demands, distances, and energy consumption rates.  
2. **Model Formulation**  
   - Decision variables for route selection, load, and energy usage  
   - Objective: minimize total travel time and number of vehicles  
   - Constraints: capacity, demand satisfaction, battery, and flow balance  
3. **Implementation**  
   - Solver: PuLP (CBC or Gurobi)
   - Visualization: Matplotlib for route plotting
4. **Validation**  
   - Tested under multiple demand and range scenarios
   - Evaluated solver runtime and constraint satisfaction

---

## Tools & Libraries
- **Python 3.x**
- **PuLP** – Linear optimization solver
- **Pandas / NumPy** – Data processing and computation
- **Matplotlib** – Route visualization and performance plots

---

## Key Results
- Achieved **15% reduction in total travel time**
- **Optimized fleet size** while maintaining service reliability
- Demonstrated **battery-aware scheduling** under variable demand
- Verified feasibility under multiple charging and demand scenarios

---
