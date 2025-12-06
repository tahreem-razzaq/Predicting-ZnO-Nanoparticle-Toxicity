# Predicting-ZnO-Nanoparticle-Toxicity
📌 Overview

This repository contains my nanoinformatics project focused on predicting Zinc Oxide (ZnO) nanoparticle toxicity using a 1D Convolutional Neural Network (CNN), combined with SHAP explainability to interpret the model.

The goal was to identify which physicochemical properties most strongly influence toxicity and determine potential safety thresholds.

🎯 Model Performance

Model: 1D Convolutional Neural Network

Accuracy / R² Equivalent: ~91% prediction accuracy

Stable training curves with low generalization error

Preprocessing: MinMax scaling + feature normalization

Evaluation Metrics: Confusion matrix 

🔍 Key Scientific Findings
1️⃣ Hydrodynamic Size is the Primary Predictor

SHAP analysis revealed:

Hydrodynamic size (“hydro size”) is the strongest determinant of ZnO toxicity

Dose ranked second, showing a strong dose–response relationship

Additional contributors: zeta potential, band gap, morphology

2️⃣ Toxicity–Size Trend Clearly Observed

The ML analysis showed:

Particles < 20 nm (hydrodynamic size) → extremely high predicted toxicity

20–40 nm → toxicity decreases sharply

≈50 nm → model indicates a potential lower-toxicity threshold
📊 Explainable AI (XAI): SHAP

The explainability component provides:

SHAP summary plot (feature importance)

SHAP dependence plots for hydrodynamic size and dose

Insight into how each parameter pushes toxicity values higher or lower

Transparency in nanotoxicity predictions
Larger particles tend to be less reactive and cause reduced oxidative stress

These trends match known nanotoxicology behavior, confirming model validity.
