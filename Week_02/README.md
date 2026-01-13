# Week 2: Multidimensional Data Structures and 4D-STEM Foundations
January 12-16, 2026

## Overview
This week focuses on understanding multidimensional data structures in electron microscopy, with particular emphasis on 4D-STEM data. Students will learn to distinguish between navigation and signal axes, work with 4D datasets, and implement virtual detector reconstructions.

## Monday: Introduction to 4D-STEM Data Structures
- Distinguishing Navigation vs. Signal Axes
- Loading and calibrating 4D-STEM datasets
- Basic data inspection and metadata handling

## Wednesday: Virtual Detectors and Post-Acquisition Imaging
- Virtual Bright Field (BF) and Annular Dark Field (ADF) reconstruction
- Center of Mass (CoM) correction for beam alignment
- Publication-quality visualization with scale bars and colormaps

## Assignment 2: 4D-STEM Foundations
- **assignment_02_setup.ipynb**: Assignment tasks and empty code cells
- **assignment_02_solutions.ipynb**: Complete solutions with working code
- **Data**: Si-SiGe.dm4 4D-STEM dataset available in assignments/raw_data/
- Topics: Axes management, data loading, virtual detectors, visualization

## Exercises
- **exercise_02_hyperspy_basics.ipynb**: Practice with HyperSpy signals, axes, and operations
- **exercise_02_4dstem_basics.ipynb**: Hands-on 4D-STEM data creation, virtual detectors, and calibration

## Directory Structure
```
Week_02/
├── README.md                              # This file
├── lectures/                              # Lecture materials and notebooks
├── code_examples/                         # Example code and scripts
├── exercises/
│   ├── exercise_02_hyperspy_basics.ipynb  # HyperSpy practice exercises
│   └── exercise_02_4dstem_basics.ipynb    # 4D-STEM practice exercises
├── assignments/
│   ├── assignment_02_setup.ipynb          # Assignment tasks
│   └── assignment_02_solutions.ipynb      # Assignment solutions
└── resources/                             # Additional reading and references
```

## Key Concepts
- **Navigation Axes**: Spatial coordinates where measurements are made (x, y scan positions)
- **Signal Axes**: Data measured at each navigation point (diffraction patterns, spectra)
- **Virtual Detectors**: Post-acquisition image formation from diffraction data
- **4D-STEM**: Four-dimensional scanning transmission electron microscopy data

## Learning Objectives
By the end of this week, students should be able to:
1. Explain the difference between navigation and signal axes in multidimensional data
2. Load and calibrate 4D-STEM datasets using py4DSTEM
3. Implement virtual detector reconstructions (BF, ADF)
4. Create publication-quality visualizations of microscopy data
5. Understand how virtual detectors enable flexible post-acquisition imaging
