# Taxi Extension
Assignment on “Deep Reinforcement Learning and Application to the Intrusion Response Case”

Consider the following extension to the Taxi-v3 environment provided by OpenAI gym:
the Taxi car has a fuel tank that can hold up to 10 (discrete) gallons of fuel.
- When a new episode starts, the fuel tank contains a random amount of fuel
(any discrete number from 1 to 10).
- There is at least one gas station at distance 1 from the taxi.
- There are at least 4 other gas stations in random positions on the map, totaling
5 gas stations.
- Every move of the taxi requires 1 gallon of fuel.
- When the taxi is in a position with a gas station, it can decide whether to make
gas or to keep on going. If the decision is to make gas, the tank is completely
replenished.
- If the tank is empty, the episode terminates with a penalty.

## The student is required to:
- Design and develop such extension and train an agent on it using Q-Learning.
- Write a short report (2 to 4 pages) explaining how the extension was designed
and comparing the experimental results (feasibility of the problem, time to
reach convergence, observed behavior) obtained by using the new
environment with those obtained with the Taxi-v3 environment.

## Solution
The new environment is implemented in the file `taxi_ext.py`.
In order to train the agent, run the file `train_ext.ipynb` (Jupyter Notebook) for the extended environment and `train_base.ipynb` for the original environment.
The results are saved in the folder `stats` and can be visualized with the file `results.ipynb`.

## Requirements
The code is written with Python 3.9. The required packages are listed in the file `requirements.txt`.

## Clone and Install
To clone the repository, run the following command:
```bash
git clone https://github.com/Marini97/taxi-extension.git
```

To install the required packages, run the following command:
```
pip install -r requirements.txt
```
