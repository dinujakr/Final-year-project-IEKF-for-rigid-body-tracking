# Intrinsic Extended Kalman Filter for rigid body attitude tracking
Simulation and experimental verification of Intrinsic Extended Kalman Filter for rigid body attitude tracking

An implementation of an **Intrinsic Extended Kalman Filter (IEKF)** for rigid body attitude estimation using IMU measurements. The project investigates the advantages of **Lie Group** filtering on **SO(3)** compared to conventional **Extended Kalman Filters (EKF)**, particularly under aggressive rotational motion.

The implementation is evaluated using sequences from the **EuRoC MAV Dataset**, with quantitative and qualitative comparisons against ground truth orientation.

---

## Project Overview

Accurate attitude estimation is fundamental in aerospace, robotics, autonomous vehicles, and UAV navigation. Conventional EKFs estimate orientation in Euclidean space, which introduces inconsistencies because rotations naturally evolve on the nonlinear manifold **SO(3)**.

This project implements an **Intrinsic Extended Kalman Filter** that:

- Represents attitude directly on the **Special Orthogonal Group SO(3)**
- Uses **Lie algebra** for error-state representation
- Preserves rotation matrix orthogonality throughout estimation
- Provides improved consistency during aggressive rotational maneuvers

---

## Features

- Intrinsic Extended Kalman Filter (IEKF)
- SO(3) rotation matrix formulation
- Lie Algebra (**so(3)**) exponential and logarithm maps
- IMU propagation using gyroscope measurements
- Accelerometer-based correction
- Gyroscope bias estimation
- EuRoC MAV Dataset support
- Ground truth comparison
- Root Mean Square Error (RMSE) evaluation
- Orientation visualization
- Error analysis
