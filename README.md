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

##  Benchmark Problem

- **TNK Problem**
  - Two objective functions
  - Nonlinear constraints
  - Known constrained Pareto front
  - Widely used benchmark for CMOP evaluation

---

##  Methodology Overview

1. Initialize a shared population
2. Solve the **Target Task** using strict constraint handling
3. Solve the **Source Task** using relaxed constraints
4. Gradually shrink the constraint relaxation boundary
5. Perform adaptive knowledge transfer between tasks
6. Apply evolutionary operators (SBX crossover and Polynomial Mutation)
7. Perform non-dominated sorting and environmental selection
8. Extract final feasible Pareto-optimal solutions

---
##  How to Run

Clone this repository:

git clone https://github.com/your-username/multiform-optimization-framework.git
cd multiform-optimization-framework


Run the main script:

python mfo_framework.py


The script will:

Generate the true Pareto front for the TNK problem

Run MFO/AKT

Run Baseline NSGA-II

Compute HV and IGD metrics

Plot and save Pareto front comparison

##  Academic Context

- **Course**: Optimization Techniques  
- **Degree**: Bachelor of Technology (B.Tech)  
- **Branch**: Artificial Intelligence / Information Technology  
- **Institute**: National Institute of Technology Karnataka, Surathkal  

---

##  Authors

- **Nayana Yogeshwari P M** (231AI023)  
- **Nandeesh V Nayak** (231AI022)

---

##  License

This project is intended strictly for **academic and research purposes**.  
If you use or extend this work, please cite the original IEEE publication.

---

##  Acknowledgements

- Authors of the original Multiform Optimization Framework
- `pymoo` library for providing multiobjective optimization tools

