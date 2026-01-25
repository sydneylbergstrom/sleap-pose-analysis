# SLEAP Pose Analysis
## Overview
This repository includes an anonymized analysis pipeline for SLEAP pose-tracking outputs. It loads a SLEAP-exported '.h5' file, extracts keypoints, handles missing data, applies optional smoothing, and computes basic kinematic features such as velocity. 

## What this notebook does
- Loads SLEAP 'tracks' and 'node_names' from an exported HDF5 file
- Selects nodes by name
- Fills missing values via interpolation
- Smooths trajectories (Gaussian smoothing by default; optional Kalman smoothing)
- Fills missing values via interpolation
- Computes per-node velocity magnitude over time
