
# Overview
This project focuses on predicting antenna S11 characteristics using machine learning and custom mathematical modeling techniques combined with electromagnetic simulation tools.
The complete project was developed in three major phases:
- Altair FEKO + Initial ML Workflow
- CST Studio + Random Forest Regression
- Custom Mathematical ML Model using Gradient Descent

The final phase focuses on a fully custom ML model designed from scratch to learn antenna resonance behavior directly from CST-generated datasets.

# Phase 1 — Altair FEKO + Initial ML (20%)
Objective: To study antenna behavior using Altair FEKO simulations and generate datasets for machine learning assisted antenna prediction.
Work Done
- Designed antenna structures in FEKO
- Performed electromagnetic simulations
- Generated antenna datasets
- Studied S11 variation with antenna parameters
- Explored initial ML integration concepts

Output: Basic understanding of antenna parameter optimization using simulation-generated datasets.

# Phase 2 — CST Studio + Random Forest Regression (20%)
Objective: To improve antenna prediction using CST-generated datasets and standard machine learning algorithms.

Work Done: 
- Designed half-wave dipole antenna in CST Studio Suite
- Generated datasets using parameter sweeps
- Trained Random Forest Regression model
- Predicted antenna S11 values from geometry and frequency inputs

Results
-High prediction accuracy
-Close agreement between CST and ML results
-Reduced dependence on repeated CST simulations

# Phase 3 — Custom Mathematical ML Model (60%)
Objective: To develop a complete custom machine learning model without using built-in regression algorithms.

Model Features
- The custom model combines:
- Sinusoidal terms for wave behavior
- Resonance terms for S11 dip modeling
- Geometry interaction terms
- Nonlinear frequency relationships
- Optimization Method

Gradient descent was implemented manually using NumPy to optimize model parameters.

Inputs:
- Antenna Length
- Gap
- Frequency
- Output
- S11 (dB)

Final Results
R² ≈ 0.93
MSE ≈ 0.88
The custom model successfully captured antenna resonance characteristics and nonlinear electromagnetic behavior with strong agreement to CST simulation data.

Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- CST Studio Suite
- Altair FEKO
- Machine Learning
- Gradient Descent
- Random Forest Regression

# Project Highlights:
- Developed complete ML workflow for antenna prediction
- Reduced repeated EM simulation effort
- Implemented custom optimization algorithm from scratch
- Successfully modeled nonlinear antenna resonance behavior
