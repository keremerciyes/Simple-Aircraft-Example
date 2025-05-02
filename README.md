# Aircraft Pitch Control Simulation

## Description

This project simulates the pitch control system for an aircraft using MATLAB and Simulink. It involves defining the aircraft's pitch dynamics with a transfer function and implementing a Proportional-Derivative (PD) controller to regulate the pitch angle.

## Files

* **Simulink Model (`.slx` or `.mdl` - name not specified in provided files):** Contains the block diagram representation of the closed-loop control system, including the aircraft dynamics and the PD controller[cite: 8].
* **(Optional) MATLAB Script (`.m` - name not specified):** Might contain the definition of the aircraft transfer function and controller parameters, along with analysis commands (based on Aircraft\_example.pdf contents [cite: 1, 2, 3, 6]).

## Aircraft Model

The linearized model for the aircraft pitch dynamics is represented by the following transfer function[cite: 2]:

$G_{p}(s)=\frac{\Theta(s)}{\Delta(s)}=\frac{1.151s+0.1774}{s^{3}+0.739s^{2}+0.921s}$

Where:
* $\Theta(s)$ is the Laplace transform of the pitch angle.
* $\Delta(s)$ is the Laplace transform of the elevator deflection angle.

## Controller

A Proportional-Derivative (PD) controller is implemented to control the aircraft's pitch[cite: 6, 8]. The controller aims to achieve desired performance criteria, such as minimizing overshoot and settling time[cite: 6]. The controller transfer function used in the example analysis is[cite: 6]:

$C(s) = K_p + K_d s = 53.287 + 13.32175 s$

*(Note: The specific parameters might be defined within the Simulink model or a separate MATLAB script).*

## How to Run

1.  Ensure you have MATLAB and Simulink installed, including the Control System Toolbox.
2.  Open the Simulink model file (`.slx` or `.mdl`).
3.  (If applicable) Run the associated MATLAB script (`.m`) first to initialize variables and parameters.
4.  Run the simulation from the Simulink model window.
5.  Observe the outputs, such as the pitch angle response, typically displayed using a Scope block[cite: 8].

## Dependencies

* MATLAB
* Simulink
* MATLAB Control System Toolbox