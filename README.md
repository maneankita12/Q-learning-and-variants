# Q-learning-and-variants

## Overview

This project reproduces and empirically evaluates the convergence guarantee 
established by Watkins and Dayan (1992), that Q-Learning converges to the 
optimal action-value function Q* with probability 1 under specific conditions. 
Four tabular reinforcement learning algorithms are implemented from scratch and 
evaluated across two environments.

**Algorithms implemented:**
- Q-Learning (paper-correct learning rate schedule α = 1/N(x,a))
- SARSA
- Expected SARSA
- Double Q-Learning

**Environments:**
- Custom 4×4 GridWorld: designed to directly satisfy the theorem's conditions
- Tic-Tac-Toe: agent learns by playing against a random opponent

## Reference Paper

Watkins, C. J. C. H., & Dayan, P. (1992). Q-learning. 
*Machine Learning, 8*(3–4), 279–292.

## Repository Structure
├── Grid_World_Environment.ipynb      
├── README.md   
└── Tic-Tac-Toe_Environment.ipynb

## Requirements
python >= 3.10
numpy
pandas
matplotlib

Install dependencies:
pip install numpy pandas matplotlib

## How to Run

1. Clone the repository
git clone https://github.com/maneankita12/Q-learning-and-variants

2. Open either notebook in Jupyter or Google Colab

3. Run all cells in order (no additional setup required)

## Results Summary

All four algorithms converged successfully in both environments. 
The paper-correct learning rate schedule α = 1/N(x,a) directly 
satisfied Watkins and Dayan (1992) Equation 3, and Q-value 
stabilization was confirmed empirically across 3000 training episodes.
