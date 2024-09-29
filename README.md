
# Passivity Based Task Space Control of Hybrid Rigid Soft Robots with Parametric Uncertainty

## Table of Contents

1. [Program 1: Dynamic System Simulation with Control Law](#program-1-dynamic-system-simulation-with-control-law)
2. [Program 2: Simulation of HyRiSo Robot with Passivity-Based Controller](#program-2-simulation-of-hyriso-robot-with-passivity-based-controller)
3. [Program 3: Adaptive and Robust Control Analysis](#program-3-adaptive-and-robust-control-analysis)
4. [Program 4: Simulation with Environmental Interaction](#program-4-simulation-with-environmental-interaction)

## Program 1: Dynamic System Simulation with Control Law

### Overview
This program simulates the dynamics of a robotic system using mathematical models. It incorporates control laws for trajectory tracking and provides a visualization of system performance, including tracking error and position trajectories.

### Key Features
- **Dynamic System Modeling:** Uses mass, damping, stiffness, and control matrices to define the system.
- **Control Law Implementation:** Applies a control strategy for tracking desired trajectories.
- **Trajectory Tracking:** Evaluates system performance based on the desired and actual trajectories.

### Code Highlights
- **System Dynamics:** Defined using a set of ordinary differential equations (ODEs) that describe the robot's behavior.
- **Control Law Function:** Generates the control input required to minimize tracking errors.
- **Adaptation Law:** Adjusts parameters dynamically based on system performance.
- **Simulation and Plotting:** Uses `solve_ivp` from the SciPy library for numerical integration and `matplotlib` for visualization.

### How to Run
1. Execute the code to define the system parameters, control law, and adaptation law.
2. Run the simulation over a defined time span.
3. View the generated plots that show the system's trajectory and tracking error.

### Output
- **Trajectory Plot:** Shows the robot's position over time.
- **Tracking Error Plot:** Visualizes the difference between desired and actual trajectories.

---

## Program 2: Simulation of HyRiSo Robot with Passivity-Based Controller

### Overview
This program simulates the HyRiSo robot's movement in an uncluttered environment. It uses a passivity-based control approach to maintain stability and minimize disturbance effects on the robot's trajectory.

### Key Features
- **Passivity-Based Control:** Ensures system stability and performance in the presence of disturbances.
- **Trajectory Generation:** Simulates both reference and actual trajectories of the robot.
- **Disturbance Handling:** Allows for simulation with and without environmental disturbances to assess controller robustness.

### Code Highlights
- **HyRiSo Robot Simulation:** Models the robot's behavior and generates trajectory data.
- **Data Interpolation:** Smooths out trajectory data for improved visualization.
- **Visualization:** Provides plots for both reference and actual trajectories, as well as configuration data.

### How to Run
1. Define the `HyRiSoRobot`, `PassivityBasedController`, and `UnclutteredEnvironment` classes.
2. Run the simulation for both disturbed and undisturbed scenarios.
3. View the generated plots to compare reference and actual trajectories.

### Output
- **Reference vs. Actual Trajectory Plot:** Compares the robot's planned and actual movements.
- **Configuration Plots:** Displays different pose configurations of the robot over time.

---

## Program 3: Adaptive and Robust Control Analysis

### Overview
This program compares the performance of adaptive and robust control strategies under different conditions. It visualizes how these strategies respond to disturbances, highlighting their effectiveness.

### Key Features
- **Control Strategy Comparison:** Analyzes adaptive and robust control under disturbed and undisturbed conditions.
- **Disturbance Effects:** Evaluates how external disturbances impact system performance.

### Code Highlights
- **Control Strategy Implementation:** Generates synthetic data representing different control strategies.
- **Visualization:** Creates multiple plots to compare adaptive and robust control with and without disturbances.

### How to Run
1. Generate synthetic data representing various control scenarios.
2. Run the plotting functions to visualize control performance.
3. Compare the adaptive and robust strategies through the generated plots.

### Output
- **Control Strategy Plots:** Four plots showing control performance under different conditions:
  1. Adaptive control without disturbance
  2. Adaptive control with disturbance
  3. Robust control without disturbance
  4. Robust control with disturbance

---

## Program 4: Simulation with Environmental Interaction

### Overview
This program extends the simulation of the HyRiSo robot by introducing environmental interactions. It assesses how the robot performs in the presence of different environmental conditions, with a focus on maintaining trajectory accuracy.

### Key Features
- **Environmental Interaction:** Models the robot's behavior in an uncluttered environment with potential disturbances.
- **Trajectory Tracking:** Compares reference and actual trajectories to assess control accuracy.

### Code Highlights
- **Simulation Function:** Models the robot's behavior over time, taking into account disturbances.
- **Plotting Function:** Provides visual comparisons of reference and actual trajectories, as well as pose configurations.

### How to Run
1. Define the necessary classes (`HyRiSoRobot`, `PassivityBasedController`, and `UnclutteredEnvironment`).
2. Run the simulation with and without disturbances.
3. View the plots to understand the robot's performance in different scenarios.

### Output
- **Trajectory Plot:** Shows the robot's planned and actual paths.
- **Pose Configuration Plots:** Displays the robot's configuration over time.

---

## Requirements

- Python 3.x
- Libraries: `numpy`, `matplotlib`, `scipy`

Install the necessary libraries using:
```bash
pip install numpy matplotlib scipy
```

## Running the Notebook
1. Open the Jupyter Notebook containing these programs.
2. Run the cells in sequential order.
3. Observe the plots and results generated by each program.

## Conclusion
This notebook provides a comprehensive simulation environment for studying robotic control strategies and their effectiveness under different conditions. By experimenting with the provided code, users can gain insights into dynamic system behavior, control law implementation, and environmental interaction for robotic systems.

---
