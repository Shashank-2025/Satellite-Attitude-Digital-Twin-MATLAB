# 🛰️ Digital Twin of Satellite Attitude Control System (MATLAB)

## Overview
This project is a **MATLAB-based digital twin** of a satellite **Attitude Control System (ACS)**.  
It simulates how a satellite estimates its orientation using **noisy sensor data**, stabilizes itself using **control logic**, and compares **real behavior with an ideal mathematical model**.

The project combines:
- Physical modeling
- Control systems
- State estimation
- Digital twin concepts
- 3D visualization

This is a simplified but realistic representation of logic used in **real spacecraft attitude determination and control systems**.

---

## Problem Statement
In real space missions:
- Satellite sensors are noisy
- True orientation is never directly known
- External disturbances constantly affect motion

The challenge is to:
1. Estimate the satellite’s orientation accurately  
2. Control and stabilize it  
3. Monitor deviations using a digital twin  

This project solves that problem through simulation.

---

## Key Concepts Used

### 1. Satellite Attitude
- Orientation represented by **Roll, Pitch, and Yaw**
- Rotational motion modeled using basic physics

### 2. Attitude Control System (ACS)
- Uses a **PD controller** to correct orientation
- Applies corrective torque based on error and angular velocity

### 3. Kalman Filter (State Estimation)
- Estimates true orientation and angular velocity
- Combines:
  - Mathematical model (prediction)
  - Noisy sensor measurements (correction)
- Provides optimal state estimation

### 4. Digital Twin
- Runs an **ideal model** alongside the real system
- Allows comparison between:
  - Actual behavior (with noise & disturbances)
  - Ideal behavior (noise-free model)

---

## System Model

### State Vector
The system state consists of six variables:

\[
x = [\theta_x,\ \theta_y,\ \theta_z,\ \omega_x,\ \omega_y,\ \omega_z]^T
\]

Where:
- θ → orientation angles
- ω → angular velocities

---

## Methodology
1. Define satellite rotational dynamics  
2. Add external disturbances and sensor noise  
3. Design PD controller for stabilization  
4. Implement Kalman filter for state estimation  
5. Build a digital twin for comparison  
6. Visualize attitude correction using 3D animation  

---

## Final Outcomes

- ✔ Successful stabilization of satellite orientation  
- ✔ Accurate estimation of states despite noisy measurements  
- ✔ Convergence of estimation error using Kalman filter  
- ✔ Clear comparison between real system and digital twin  
- ✔ Intuitive 3D visualization of attitude correction  

---

## Why This Project Matters
- Demonstrates **real-world aerospace control concepts**
- Shows practical use of **Kalman filtering**
- Introduces **digital twin modeling**
- Bridges theory with real engineering systems

Used concepts are directly relevant to:
- Satellite systems
- Aircraft navigation
- Robotics
- Autonomous systems

---

## Tools Used
- MATLAB
- Control Systems
- Kalman Filter
- State-Space Modeling
- 3D Visualization

---

## How to Run
1. Open MATLAB
2. Place the file in the MATLAB working directory
3. Run:
```matlab
satellite_attitude_digital_twin
