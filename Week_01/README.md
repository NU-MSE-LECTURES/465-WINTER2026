# Week 1: Digital Data Foundations and Workflow Setup
January 5-9, 2026

## Overview
This week introduces the fundamentals of computational microscopy, focusing on setting up your development environment and understanding the data types and tools used throughout the course. You'll learn about the evolution of microscopy techniques, key data formats in electron microscopy (EM), and best practices for reproducible research.

## Learning Objectives
By the end of this week, you should be able to:
- Understand the role of computation in modern microscopy
- Set up a Python environment with essential libraries for microscopy data analysis
- Use version control (Git) and GitHub for managing code and data
- Load and visualize basic EM image data
- Organize projects for reproducible research

## Schedule

### Monday: Overview of Modern Computational Microscopy
- Historical context and evolution of computational microscopy
- Data types in EM: image, diffraction, and 4D-STEM
- Introduction to open-source tools used in this course (HyperSpy, NumPy, Matplotlib, etc.)

### Wednesday: Setting up Computational Environments
- Installing Python, Jupyter Lab, and essential libraries
- Version control and GitHub workflows
- Best practices for data organization and reproducible research

## Assignment 1: Environment Setup and Dataset Exploration
- **Due Date:** January 16, 2026
- Tasks include verifying your Python environment, creating project directories, demonstrating reproducibility with random seeds, and exploring EM image data.
- See `assignments/assignment_01_setup.ipynb` for the assignment details.
- Solutions are provided in `assignments/assignment_01_solutions.ipynb`.

## Directory Structure
```
Week_01/
├── README.md                    # This overview file
├── lectures/                    # Lecture materials and notebooks
│   ├── lecture_01_overview.ipynb
│   └── lecture_02_environment_setup.ipynb
├── code_examples/               # Example code and scripts
├── exercises/                   # Practice problems
│   ├── exercise_01_python_practice.ipynb
│   ├── exercise_02_4dstem_basics.ipynb
│   └── exercise_02_hyperspy_basics.ipynb
├── assignments/                 # Assignment descriptions, templates, and solutions
│   ├── assignment_01_setup.ipynb
│   ├── assignment_01_solutions.ipynb
│   ├── assignment_01_output/    # Output directory for assignment 1
│   │   ├── data/
│   │   │   ├── processed/
│   │   │   └── raw/
│   │   ├── figures/
│   │   └── src/
│   └── raw_data/                # Raw data files for assignments
│       └── Si-SiGe.dm4
├── resources/                   # Additional reading and references
│   └── resources.md
└── raw_data/                    # Additional raw data (if any)
```

## Getting Started
1. **Environment Setup:** Follow the instructions in `lectures/lecture_02_environment_setup.ipynb` to install required software.
2. **Clone the Repository:** Ensure you have the latest version of the course materials.
3. **Run Lectures:** Start with `lectures/lecture_01_overview.ipynb` to understand the course context.
4. **Complete Exercises:** Work through the exercises in the `exercises/` folder to practice concepts.
5. **Submit Assignments:** Use the templates in `assignments/` and submit via the course platform.

## Prerequisites
- Basic knowledge of Python programming
- Familiarity with command-line interfaces
- Access to a computer with internet connection for software installation

## Resources
- [HyperSpy Documentation](https://hyperspy.org/)
- [NumPy User Guide](https://numpy.org/doc/stable/user/index.html)
- [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html)
- Course resources in `resources/resources.md`

For questions or issues, please post on the course discussion forum or contact the instructor.
