# Robustness of Sampling-Based MPC Under Model Mismatch

Implementation and robustness analysis of a Cross-Entropy Method Model Predictive Controller (CEM-MPC) for nonlinear pendulum swing-up under model mismatch and uncertainty.

## Overview

This project investigates how sampling-based MPC degrades when the controller's internal model differs from the true system dynamics.

The controller uses:
- Cross-Entropy Method (CEM) trajectory optimization
- Phase-aware MPC for swing-up and stabilization
- RK4 dynamics integration
- Noise and disturbance simulation

We systematically evaluate robustness under:
- Mass mismatch
- Length mismatch
- Damping mismatch
- Observation noise
- Process noise
- Combined stress conditions

## Key Findings

- Length mismatch is the dominant failure factor
- Observation noise is significantly more damaging than process noise
- The controller exhibits sharp robustness thresholds
- Combined uncertainties create strong synergistic failures

## Technologies

- Python
- NumPy
- Matplotlib
- Scientific Computing
- Nonlinear Control
- Model Predictive Control (MPC)


## Example Results

- 100% baseline stabilization success
- Failure beyond ~1.5× length mismatch
- Observation noise threshold near 0.10 rad
- Robust damping tolerance up to 50×

## Future Improvements

- Online parameter adaptation
- Learned dynamics models
- State estimation with Kalman filtering
- Extension to higher-dimensional systems

## References

- Cross-Entropy Method MPC
- Nonlinear Control
- Robust Model Predictive Control
