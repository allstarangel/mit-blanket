# MIT Blanket — Flexible Magnetic Induction Tomography

A low-cost, flexible point-of-care imaging system 
designed for resource-constrained settings including 
disaster response, military medicine, and low-resource clinics.

## What This Is

This project implements a blanket-form Magnetic Induction 
Tomography (MIT) system using a 4×4 flexible coil array, 
adaptive regional activation, and Gauss-Newton reconstruction 
accounting for non-rigid coil geometry.

## Why It Matters

4.5 billion people worldwide lack access to medical imaging. 
This system aims to make internal tissue imaging as portable 
and affordable as a stethoscope.

## System Overview

- **Hardware:** 4×4 flexible coil grid, RTL-SDR, 
  Raspberry Pi 4, AD9833 waveform generator
- **Sensing:** Software-based contact detection, 
  multiplexed TX/RX cycling
- **Reconstruction:** Gauss-Newton iterative solver 
  with Tikhonov regularization
- **Target use cases:** Doctors Without Borders, 
  military medics, disaster response, small clinics

## Project Status

Phase 1 — Software simulation (in progress)  
Phase 2 — Hardware integration  
Phase 3 — Phantom validation  

## Repository Structure

mit-blanket/
├── config/          # Array geometry, frequency parameters
├── hardware/        # RPi GPIO, SDR interface
├── sensing/         # Contact detection, measurement cycling
├── reconstruction/  # Forward model, Jacobian, Gauss-Newton
├── visualization/   # Conductivity map plotting
├── results/         # Saved figures and outputs
├── tests/           # Unit tests for each module
├── notebooks/       # Jupyter exploration notebooks
└── docs/            # Notes, derivations, references

## Author

Jackymora Isa-Shei  
Independent Research — May 2026
