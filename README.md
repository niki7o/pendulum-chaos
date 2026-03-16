# N-Pendulum Chain — When Does Complexity Explode?

**Course:** Math Concepts for Developers, SoftUni 2026  
**Author:** Nikola Kolev

## Overview

This project investigates how chaos grows in a chain of N coupled pendulums.
We measure the Lyapunov exponent, fractal dimension, and Poincaré sections
for N = 2 to 8 and study how damping destroys chaos.

## How to Run

### Requirements

Make sure you have Python installed. Then install the required libraries:
```bash
pip install numpy scipy matplotlib sympy jupyter
```

### Running the notebook
```bash
cd pendulum-chaos
jupyter notebook pendulum-chaos.ipynb
```

Or if jupyter is not in your PATH:
```bash
python -m notebook pendulum-chaos.ipynb
```

### Important notes

- When prompted for number of pendulums, **6-8 is recommended**. Higher values may be slow.
- The animation opens in a **separate window** — do not close it manually.
- Run cells **in order** from top to bottom.
- If a cell seems frozen, wait — some simulations take 1-3 minutes.

## Project Structure
```
pendulum-chaos/
│
├── pendulum-chaos.ipynb    # main notebook with all analysis
└── README.md               # this file
```

## Methods Used

- Lagrangian mechanics (SymPy symbolic derivation)
- Inertia matrix numerical method (NumPy/SciPy)
- Lyapunov exponent (finite-time)
- Box-counting fractal dimension
- Phase diagram (chaos map)
- Poincaré sections
- Viscous damping analysis
- Energy conservation check

## Results Summary

- Lyapunov exponent λ ≈ 0.84–1.00 for all N — chaos is saturated at N=2
- Fractal dimension decreases from 1.42 (N=2) to 1.06 (N=8)
- 99.6% of initial conditions lead to chaos at N=2
- Damping of b≥0.5 completely eliminates chaos
```

---

После commit:
```
git add README.md
git commit -m "docs: add README with setup and run instructions"
git push
