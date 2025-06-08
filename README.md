# Adaptive Traffic Signal Control Using Deep Reinforcement Learning and V2I Data

This repository contains my part of my Research project that implements an adaptive traffic signal control system leveraging V2I communication data and deep reinforcement learning.

## Project Overview
The project extends V2I speed guidance models by shifting optimization responsibility from the vehicles to the infrastructure (traffic signal controllers). A DRL agent (Deep Q-Network) was trained to optimize real-time signal timing based on vehicle arrival data, queue lengths, and V2I infrastructure messages.

## Data Sources
- **NGSIM Peachtree Vehicle Trajectories** (U.S. FHWA): High-resolution vehicle trajectories.
- **NYC Connected Vehicle Pilot** (U.S. DOT ITS): SPaT messages & safety alerts.

## Methodology
- Data Preprocessing in Python (Pandas, Matplotlib)
- State Vector Construction (vehicle counts, queued vehicles, excessive speed warnings)
- Reinforcement Learning with DQN (PyTorch, Stable-Baselines3)
- Simulation Environment: SUMO + TraCI API

## Repository Contents
- `data/`: Raw and processed datasets.
- `notebooks/`: Preprocessing, feature engineering, and RL training code (Google Colab).
- `reports/`: Problem description, dataset preprocessing report, and presentation slides.

## Sample Results
- Clear congestion patterns visualized from NGSIM.
- V2I message trends extracted from NYC CV dataset.
- DRL agent trained for adaptive signal control (initial DQN implementation).

## Potential Future Work
- Implement PPO algorithm for improved stability.
- Incorporate more realistic traffic scenarios.
- Explore multi-intersection coordination.

## 🔗 Dataset Links
- [NGSIM Dataset](https://ops.fhwa.dot.gov/trafficanalysistools/ngsim.htm)
- [NYC Connected Vehicle Pilot Dataset](https://data.transportation.gov/Automobiles/NYC-Connected-Vehicle-Pilot-Deployment-BSM-and-SPaT-D/vxut-9scr)
