# tailsitter-flight-control
# Tailsitter UAV Flight Dynamics and Control

## Overview

This project focuses on the simulation and implementation of flight dynamics and control approaches for a tailsitter Unmanned Aerial Vehicle (UAV) using MATLAB and Simulink.

A tailsitter UAV takes off and lands vertically, like a multirotor, and transitions to forward flight for efficient fixed-wing operation. Modelling and controlling the aircraft across these different flight conditions presents an interesting control problem.

As part of this project, two research-based control approaches were implemented by following published research papers. The implementations and their corresponding simulation results are organized separately below.

## 1. Global Incremental Flight Control for Agile Maneuvering of a Tailsitter Flying Wing

**Reference:** Tal and Karaman (2022)

This implementation follows the global incremental flight-control approach presented by Ezra Tal and Sertac Karaman. The work focuses on controlling a tailsitter across different flight conditions and tracking reference trajectories.

### Simulation Scenarios

The simulation demonstrates three trajectory-tracking scenarios:

- **VTOL:** Vertical take-off and flight.
- **Circular Trajectory Tracking:** Tracking a circular reference trajectory.
- **Lemniscate Trajectory Tracking:** Tracking a figure-eight-shaped reference trajectory.

These simulations demonstrate the controller's behaviour during vertical flight and while following different reference trajectories.

### Files

The `global_indi/` directory contains the relevant MATLAB/Simulink implementation files and simulation results.

**Simulation videos:**
- [VTOL Simulation](global_indi/videos/your_vtol_video.mp4)
- [Circular Trajectory Tracking](global_indi/videos/your_circular_video.mp4)
- [Lemniscate Trajectory Tracking](global_indi/videos/your_lemniscate_video.mp4)

## 2. Modeling and Control of a Tailsitter UAV

**Reference:** Chiappinelli and Nahon (2018)

This implementation follows the quaternion-based control approach presented by Romain Chiappinelli and Meyer Nahon. The approach uses a cascaded control structure for modelling and controlling tailsitter flight.

### Simulation Scenario

A complete flight sequence was simulated to demonstrate the aircraft's behaviour during vertical take-off, hover, forward flight, transition back to vertical flight, and landing.

The simulated sequence consists of:

1. **Vertical Take-Off:** The aircraft climbs vertically to an altitude of approximately 5 m.
2. **Hover:** The aircraft maintains its position at the target altitude.
3. **Forward Flight:** The aircraft transitions from vertical flight to forward flight.
4. **Back Transition:** The aircraft transitions back towards vertical flight while at altitude.
5. **Descent and Landing:** The aircraft gradually descends and lands.

The simulation demonstrates the complete flight sequence within a single trajectory.

### Files

The `quaternion_based_control/` directory contains the relevant MATLAB/Simulink implementation files and the corresponding simulation video.

**Simulation video:** [Watch the VTOL, transition and landing simulation](quaternion_based_control/videos/your_video.mp4)

*The folder and video filenames above are examples. Replace them with the actual names and locations in your repository.*

## Software and Tools

- MATLAB
- Simulink

Add the specific MATLAB release and toolboxes used in the simulations if you want to document the software environment.

## References

1. E. Tal and S. Karaman, “Global Incremental Flight Control for Agile Maneuvering of a Tailsitter Flying Wing,” *Journal of Guidance, Control, and Dynamics*, vol. 45, no. 12, December 2022. [https://doi.org/10.2514/1.G006645](https://doi.org/10.2514/1.G006645)

2. R. Chiappinelli and M. Nahon, “Modeling and Control of a Tailsitter UAV,” in *Proceedings of the 2018 International Conference on Unmanned Aircraft Systems (ICUAS)*, Dallas, Texas, USA, June 12–15, 2018.

## Acknowledgements

This project was carried out by studying and implementing control approaches described in the cited research papers. Credit for the original control methods belongs to their respective authors.

## Disclaimer

This repository documents simulation and implementation work for educational and research purposes. Simulation results alone do not establish real-world flight performance or flight readiness.
