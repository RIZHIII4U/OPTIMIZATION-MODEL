# OPTIMIZATION-MODEL TASK-4

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: RISHAB GANESH N

*INTERN ID*:  CTIS4236

*DOMAIN*: Data Science

*DURATION*: 4 Weeks

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*: Task-4: Smart EV Charging Station Location Optimization Integer Linear Programming using PuLP (Python)

## Project Overview

The rapid adoption of Electric Vehicles (EVs) requires efficient and well-planned charging infrastructure. Installing EV charging stations involves significant capital investment, making it essential to select optimal locations that balance cost, capacity, and demand.

This project applies **Integer Linear Programming (ILP)** using the **PuLP library in Python** to determine the optimal combination of EV charging station locations. The goal is to minimize total installation cost while satisfying charging demand and adhering to budget constraints. The solution supports data-driven infrastructure planning aligned with smart city and sustainability objectives.

---

## Problem Statement

A city government plans to install EV charging stations at selected candidate locations. Each location has:

* A fixed installation cost
* A maximum charging capacity

The city must:

* Stay within a limited total budget
* Ensure a minimum total charging capacity to meet EV demand

### Objective

Minimize total installation cost while meeting demand and staying within budget.

---

## Data Description

Five potential locations are available:

| Location | Installation Cost (₹) | Maximum Capacity |
| -------- | --------------------- | ---------------- |
| L1       | 50,000                | 40               |
| L2       | 70,000                | 60               |
| L3       | 40,000                | 30               |
| L4       | 60,000                | 50               |
| L5       | 55,000                | 45               |

**Total Budget:** ₹2,00,000
**Minimum Required Capacity:** 120 units

---

## Mathematical Model

### Decision Variable

Xi = 1 if location i is selected, 0 otherwise (Binary Variable)

### Objective Function

Minimize:
Z = Σ (Cost_i × Xi)

### Constraints

1. Budget Constraint
   Σ (Cost_i × Xi) ≤ 200000

2. Demand Constraint
   Σ (Capacity_i × Xi) ≥ 120

3. Binary Constraint
   Xi ∈ {0,1}

---

## Technologies Used

* Python 3.x
* PuLP (Linear Programming Library)
* Jupyter Notebook
* Matplotlib (Visualization)

---

## How to Run

1. Install dependencies:

```bash
pip install pulp matplotlib
```

2. Launch Jupyter Notebook:

```bash
jupyter notebook
```

3. Open and run the notebook file.

---

## Results

The model determines:

* Optimal set of charging station locations
* Minimum installation cost
* Total charging capacity achieved
* Solver status (Optimal/Feasible)

Visualization is included to display selected locations and capacity distribution.

---

## Key Insights

* Optimization ensures cost-efficient infrastructure planning.
* Binary integer programming is effective for location selection problems.
* Budget-constrained modeling supports financial feasibility.
* The model is scalable and can be extended to multi-zone or multi-period planning.

---

## Conclusion

This project demonstrates how Integer Linear Programming can address real-world infrastructure challenges. By integrating cost, capacity, and demand constraints, the model provides a practical framework for sustainable EV charging station deployment and smart city development.

---

If you want, I can also give you a **short 150-word abstract** for internship submission or a **resume-ready project description (3–4 lines)**.
