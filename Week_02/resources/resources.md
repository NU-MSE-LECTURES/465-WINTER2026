# Week 02: Resources

## Key References

### 4D-STEM Data Analysis
- **py4DSTEM Documentation**: https://py4dstem.readthedocs.io/
- **py4DSTEM GitHub**: https://github.com/py4dstem/py4dstem
- **Multidimensional Data in Electron Microscopy**: Lectures and tutorials on navigating 4D datasets

### Crystallography and Bragg Calibration
- **International Tables for Crystallography**: Standard reference for crystal structure factors and d-spacings
- **FCC Crystal Structure (Au)**: 
  - Space group: Fm-3m (225)
  - Lattice parameter: a = 4.078 Å
  - Common reflections: 111 (d=2.36 Å), 220 (d=1.44 Å), 440 (d=0.72 Å)
- **Bragg's Law**: nλ = 2d·sin(θ)
- **Scattering Vector**: q = 1/d (reciprocal space)

### HyperSpy
- **HyperSpy Documentation**: https://hyperspy.org/
- **HyperSpy GitHub**: https://github.com/hyperspy/hyperspy
- **Signal Axes vs Navigation Axes**: Core concept for multidimensional data analysis

### Virtual Detectors and Image Formation
- **Bright Field (BF)**: Low-angle scattering detection
- **Annular Dark Field (ADF)**: High-angle scattering detection, sensitive to atomic number (Z-contrast)
- **Center of Mass (CoM) Correction**: Beam alignment and aberration correction

## Calibration Standards

### Au Nanoparticles
- Excellent reference material for detector calibration
- Well-defined FCC crystal structure
- High scattering power for clear Bragg rings
- Typical size: 10-100 nm
- Available from commercial sources (e.g., plasma cleaning standards)

### Si Reference
- Diamond cubic structure
- Well-characterized lattice parameter: a = 5.431 Å
- Common reflections: 220 (d=1.92 Å), 440 (d=0.96 Å)

## Software Setup

### Required Packages
- py4DSTEM >= 0.14.18
- HyperSpy >= 2.3.0
- NumPy >= 1.26.4
- SciPy >= 1.15.2
- Matplotlib >= 3.10.8

### Environment File
See `environment.yml` in the root directory for the complete conda environment used in this course.

## Tips for Colab

### Installation in Google Colab
```python
# Install required packages
!pip install py4dstem hyperspy scikit-image matplotlib

# For file I/O
from google.colab import files
```

### File Handling in Colab
- Upload files: `files.upload()`
- Download results: `files.download('filename.ipynb')`

## Further Reading

### Advanced Topics
1. **Strain Mapping**: Using center of mass analysis
2. **Momentum Transfer (q) Space**: Reciprocal space visualization
3. **Automated Peak Finding**: Advanced signal processing techniques
4. **Crystallographic Phase Identification**: From diffraction patterns

### Textbooks and Papers
- "Advanced Transmission Electron Microscopy" - various authors
- Research papers on 4D-STEM techniques (available via journal databases)

## Data Sources

### Week 02 Datasets
- **Si-SiGe**: Available in `assignments/raw_data/Si-SiGe.dm4`
- **Au Nanoparticles (Calibration)**: Available in `assignments/raw_data/Diffraction SI_Au_Calib.dm4`

### Open Data Repositories
- **FEI/Thermo Fisher Data**: Various sample datasets
- **Research Institutions**: Many universities provide open-access EM datasets

## Links and Contacts

### Course Resources
- Course GitHub: https://github.com/NU-MSE-LECTURES/465-WINTER2026
- Course Website: [Add your course website]

### Getting Help
- File issues on GitHub
- Ask questions in course discussion forums
- Contact: [Add instructor contact information]
