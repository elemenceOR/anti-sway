1.run mpc_antisway.m for the complete simulation. It will run the simulink
%model as well.
2.crane_mode;_mpc.slx is for simulation. It won't run without running mpc_antisway.m file.

# Gantry Crane Anti-Sway Control System

## Project Overview

This project presents the modeling, analysis, and controller design of an anti-sway system for a gantry crane. The study focuses on controlling the nonlinear sway dynamics using both theoretical and simulation-based approaches, ultimately implementing a Model Predictive Controller (MPC) to suppress undesired load swings during crane operation.

## Contents

- Introduction to Gantry Crane Anti-Sway Systems
- Theoretical Background:
  - Stability Analysis (Lyapunov Method)
  - Controller Design Methods:
    - Feedback Linearization
    - Model Predictive Control (MPC)
- System Modeling and Equations
- Controller Design in MATLAB/Simulink
- Simulation Results and Tuning Parameters
- Conclusion and Comparison of Linear vs. Non-linear Control

---

## Key Technologies

- **MATLAB/Simulink** — for modeling and controller simulation
- **Control Theory** — including Lyapunov stability and feedback linearization
- **Model Predictive Control** — applied to the nonlinear system with a focus on sway suppression

---

## Results

- Successful sway suppression using MPC
- System is Lyapunov stable under given assumptions
- Feedback Linearization method was partially explored, but due to internal dynamics, MPC was chosen
- MPC was tuned for optimal results under noisy and noise-free conditions

---

## Final Controller Parameters

- **Sample Time (Ts):** 0.3 s  
- **Prediction Horizon:** 100 steps  
- **Control Horizon:** 10 steps  
- **Objective Weights:**  
  - Cart Position (x): 0.5  
  - Sway Angle (θ): 0.5


![image](https://github.com/user-attachments/assets/37ada985-6a17-4159-91ac-96d4bc9ce498)

x = dispalcement
x_dot = linear velocity
theta = sway angle
theta_do = angular velocity
---

Refer to report.pdf for more information
