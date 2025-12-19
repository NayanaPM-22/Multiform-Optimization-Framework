# Multiform Optimization Framework for Constrained Multiobjective Optimization

This repository contains a Python implementation of a **Multiform Optimization Framework (MFO)** with **Adaptive Knowledge Transfer (AKT)** for solving **Constrained Multiobjective Optimization Problems (CMOPs)**. The framework is experimentally validated on the **TNK benchmark problem** and compared against the **baseline NSGA-II algorithm**.

This project is based on the IEEE paper:

> R. Jiao, B. Xue, and M. Zhang,  
> *A Multiform Optimization Framework for Constrained Multiobjective Optimization*,  
> IEEE Transactions on Cybernetics, 2023.

---

## Key Features

- Dual-task optimization framework:
  - **Target Task (Tₜ)** with strict constraints
  - **Source Task (Tₛ)** with dynamically relaxed constraints
- **Adaptive Knowledge Transfer (AKT)** between target and source tasks
- Epsilon-based constraint handling strategy
- NSGA-II based non-dominated sorting and crowding distance
- Performance evaluation using **Hypervolume (HV)** and **Inverted Generational Distance (IGD)**
- Visualization of Pareto fronts
- Baseline comparison with standard **NSGA-II**

---

## 📁 Repository Structure

