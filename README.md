# 🚁 1D Drone Altitude Control - Simulink & MATLAB Simulation

A MATLAB/Simulink simulation project modeling the dynamic system of a **1-Degree-of-Freedom (1D) Quadcopter/Drone** and designing a **PID Controller** to achieve stable altitude tracking and rapid response with minimal overshoot.

---

## 📌 Project Overview
Controlling a drone's altitude involves counteracting gravitational force through rotor thrust. This project models the vertical motion dynamics of a drone and implements a closed-loop feedback system using a tuned PID controller to maintain a target altitude.

### Key Objectives:
* Derive and model the **1D translational equations of motion** for altitude.
* Design a closed-loop **PID control system** in Simulink.
* Tune $K_p$, $K_i$, and $K_d$ parameters to meet performance specifications (minimal overshoot, zero steady-state error, fast rise time).
* Evaluate system step-response and reference tracking performance under external step disturbances.

---

## 🛠️ Tools & Environments
* **MATLAB** (Control System Toolbox)
* **Simulink** (Block diagram simulation & PID Tuner)

---

## 📊 System Architecture & Model Parameters

### 1. Dynamic Equations:
The vertical motion is governed by Newton's second law:
$$m \ddot{z}(t) = F_{thrust}(t) - m g$$

Where:
* $z(t)$: Altitude (m)
* $m$: Mass of the drone (kg)
* $g$: Acceleration due to gravity ($9.81 , m/s^2$)
* $F_{thrust}$: Combined rotor force

---

## 🚀 How to Run the Simulation

1. **Clone the repository:**
  ```bash
  git clone https://github.com/M-Pajouh/1d-drone-altitude-control.git
  ‍‍‍‍‍‍‍‍‍‍```
  
  2. **Open MATLAB:**
   * Navigate to the cloned folder in MATLAB.

  3. **Run the Simulink Model:**
   * Open the `.slx` model file.
   * Press **Run** to launch the simulation.
   * Open the **Scope** block to view the step response and tracking performance.
