# Materials Science 465: Computational Electron Microscopy - Test for git pull
Northwestern University - Winter Quarter 2026

## Course Information

**Instructor**: Prof. Dr. Roberto dos Reis
**Email**: roberto.reis@northwestern.edu
**Office**: Tech AB Wing AG90

## Course Repository Structure

This repository contains all materials for MS 465: Computational Electron Microscopy, organized by weekly topics.

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/NU-MSE-LECTURES/465_Computational_Microscopy_2026.git
   cd 465_Computational_Microscopy_2026
   ```

2. Set up the environment:
   ```bash
   conda env create -f environment.yml
   conda activate ms465-2026
   ```

3. Verify installation:
   ```bash
   jupyter lab Week_01/exercises/environment_check.ipynb
   ```

## Directory Structure

```
465_Computational_Microscopy_2026/
├── README.md                  # This file
├── environment.yml            # Conda environment specification
├── requirements.txt           # Python package requirements
├── common_utilities/          # Shared utility functions
├── datasets/                  # Sample datasets
├── Week_01/                   # Digital Data Foundations and Workflow Setup
├── Week_02/                   # Core Tools for Microscopy Data Analysis
├── Week_03/                   # Image Processing and Classical Analysis Methods
├── Week_04/                   # Machine Learning for Microscopy
├── Week_05/                   # Multislice and Image Simulation Techniques
├── Week_06/                   # Dynamical Diffraction and Bloch Waves
├── Week_07/                   # 4D-STEM and Quantitative Analysis
├── Week_08/                   # Electron Crystallography and AI-assisted Structure Analysis
├── Week_09/                   # Integration and High-Performance Computing
└── Week_10/                   # Final Projects and Future Trends
```

Each weekly folder contains:
```
Week_XX/
├── README.md           # Week overview and topics
├── lectures/           # Lecture materials and notebooks
├── code_examples/      # Example code and scripts
├── exercises/          # Practice problems
├── assignments/        # Assignment descriptions and templates
└── resources/          # Additional reading and references
```

## Course Schedule

### Week 1 (January 5-9): Digital Data Foundations and Workflow Setup
- Overview of modern computational microscopy
- Setting up computational environments
- Assignment 1: Environment setup and dataset exploration

### Week 2 (January 12-16): Core Tools for Microscopy Data Analysis
- Python ecosystem for EM data
- Structural metadata and data preprocessing
- Assignment 2: Virtual detector and diffraction analysis workflow

### Week 3 (January 19-23): Image Processing and Classical Analysis Methods
- Image processing foundations
- Classical image and diffraction analysis
- Assignment 3: Classical image segmentation pipeline

### Week 4 (January 26-30): Machine Learning for Microscopy
- Fundamentals of ML in EM
- Deep learning architectures and applications
- Assignment 4: Neural network for atomic-level pattern recognition

### Week 5 (February 2-6): Multislice and Image Simulation Techniques
- Multislice fundamentals
- Image simulation and model validation
- Assignment 5: Multislice simulation of image contrast versus thickness

### Week 6 (February 9-13): Dynamical Diffraction and Bloch Waves
- Dynamical diffraction theory
- Computational implementation of Bloch waves
- Assignment 6: Compute diffraction intensities using Bloch-wave model

### Week 7 (February 16-20): 4D-STEM and Quantitative Analysis
- Processing and analysis of 4D-STEM
- Advanced 4D-STEM applications
- Assignment 7: Full 4D-STEM analysis workflow

### Week 8 (February 23-27): Electron Crystallography and AI-assisted Structure Analysis
- Fundamentals of electron crystallography
- AI for automated structure analysis
- Assignment 8: AI-based crystallographic classification project

### Week 9 (March 2-6): Integration and High-Performance Computing
- Integrating simulation, experiment, and ML
- High-performance computing for microscopy
- Assignment 9: Mini-integration project with simulation and ML components

### Week 10 (March 9-13): Final Projects and Future Trends
- Final project presentations I
- Final project presentations II and course reflection
- Final Project Due: Technical report, GitHub repository, and oral presentation

## Key Technologies and Libraries

### Core Scientific Computing
- NumPy/SciPy: Numerical computing and scientific algorithms
- Matplotlib: Data visualization
- Pandas: Data manipulation and analysis
- HDF5: Efficient storage of large EM datasets

### Electron Microscopy Specific
- py4DSTEM: 4D-STEM data analysis and virtual imaging
- HyperSpy: Multi-dimensional data analysis framework
- pyXEM: Crystallographic diffraction analysis
- ASE: Atomic structure manipulation and visualization
- ncempy: Reading various EM data formats

### Machine Learning and AI
- PyTorch/TensorFlow: Deep learning frameworks
- scikit-learn: Traditional machine learning algorithms
- AtomAI: Physics-guided ML for atomic-resolution data

### Simulation Software
- abTEM: Pure Python multislice simulations
- Prismatic: GPU-accelerated STEM simulations
- MULTEM: Advanced electron scattering simulations

## Assessment Overview

- Weekly Programming Assignments (35%): 8 assignments building practical skills
- Major Computational Project (40%): Independent research project
- Project Presentation (15%): Conference-style presentation
- Participation and Peer Review (10%): Active engagement and collaboration

## Getting Help

### Office Hours
- Wednesday 1:00-3:00 PM: General questions and troubleshooting
- Friday 10:00-11:30 AM: Technical support and project guidance

### Online Resources
- GitHub Discussions: Course forum for questions and collaboration
- Documentation: Comprehensive guides in each week's resources folder

## Prerequisites

- Graduate standing in Materials Science, Physics, Chemistry, or related field
- Programming experience in Python
- Undergraduate courses in electron microscopy or materials characterization
- Familiarity with linear algebra and statistical methods

## Important Dates

- January 5: First day of classes
- January 19: No classes (Martin Luther King Jr. Day)
- February 13: Last day to drop a class
- March 21: End of Winter Classes, Final projects due

## Academic Integrity

All work must represent original effort with proper citation. Students may use Large Language Models (LLMs) for assistance but must cite usage and demonstrate full understanding. Collaboration is encouraged with proper attribution.

## Accessibility

Northwestern University is committed to providing equitable access. Students with documented learning differences should contact [AccessibleNU](https://www.northwestern.edu/accessiblenu/) for accommodations.
