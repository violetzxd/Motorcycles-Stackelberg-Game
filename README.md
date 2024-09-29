# Motorcycles-Stackelberg-Game
This repository contains the implementation of the multi-agent Stackelberg game framework for modeling motorcycle behavior in autonomous driving scenarios, as introduced in the paper: "Multi-Agent Behavior Modeling of Motorcycles in Autonomous Driving Scenarios: A Stackelberg Game Approach."

# "Multi-Agent Behavior Modeling of Motorcycles in Autonomous Driving Scenarios: A Stackelberg Game Approach"

This repository contains the implementation of the **multi-agent Stackelberg game framework** for modeling motorcycle behavior in autonomous driving scenarios, as introduced in the paper: **"Multi-Agent Behavior Modeling of Motorcycles in Autonomous Driving Scenarios: A Stackelberg Game Approach."** The framework simulates the complex interactions between autonomous vehicles (AVs) and motorcycles, focusing on aggressive and dangerous motorcycle behaviors in urban environments.

## Overview

In urban traffic environments, motorcycles present a unique challenge to AVs due to their high maneuverability and tendency to engage in risky behaviors such as running red lights, sudden lane changes, and wrong-way driving. Current AV testing frameworks have focused primarily on modeling car drivers and pedestrians, leaving motorcycle behavior underexplored.

This repository implements a **game-theoretic framework** to model motorcycle behaviors, specifically focusing on how aggressive leaders and conservative followers interact with AVs in complex traffic environments. The key features of this framework include:

- **Multi-Agent Stackelberg Game**: Motorcycles are divided into **leaders** (exhibiting aggressive behaviors) and **followers** (typically conservative but influenced by leaders).
- **K-Level Game Theory**: Captures varying levels of strategic reasoning among motorcycles, influencing their driving decisions.
- **AV Decision-Making Models**: Tests AVs using two decision-making models: 
  - **0-level decision-making**: No prediction of motorcycle behaviors.
  - **2-level decision-making**: Predictive model for anticipating dangerous behaviors.
- **Real-World Data Integration**: Defines the physical and dynamic parameters of motorcycles based on real-world data, categorizing behaviors into **safe**, **aggressive**, and **dangerous**.

## Key Contributions

1. **Motorcycle Behavior Modeling**: Provides a detailed model for capturing the dynamic and high-risk behaviors of motorcycles using a multi-agent Stackelberg game.
2. **Leader-Follower Dynamics**: Analyzes the long-tail effects of aggressive leader behaviors, showing how they propagate throughout the environment and influence the safety of AVs.
3. **Scenario Evaluation**: Uses **PanoSim** to test AV responses in simulated urban intersection scenarios, evaluating accident rates under different leader-follower configurations.
4. **Predictive Decision-Making**: Demonstrates the critical importance of AVs with predictive decision-making capabilities in mitigating accidents caused by high-risk motorcycle behaviors.

## Repository Structure

- `/src`: Contains the core Python code implementing the multi-agent Stackelberg game framework.
- `/data`: Includes example datasets and motorcycle behavior parameters used for modeling.
- `/simulations`: PanoSim configuration files and scripts for setting up intersection scenarios.
- `/docs`: Documentation for the framework, including setup instructions and detailed explanations of the game-theoretic models.

## Getting Started

### Prerequisites

- **Python 3.9**
- **PanoSim** for running the AV simulations
- Libraries: `numpy`, `pandas`, `matplotlib` for data analysis and visualization.

### Running the Simulations

1. Configure your simulation parameters in the `/simulations/config` folder.
2. Run the multi-agent interaction simulations:
   ```bash
   python src/xxxxxx(choose which scenario to simulate).py
   ```
3. Import the XML file for rebuild the testing scenarios in PanoSim

## Results and Evaluation

More detailed results and evaluation please refers to the paper.

## Notice

The relevant code, dataset, and demonstration video are currently being organized. Please be patient and wait for further results.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

