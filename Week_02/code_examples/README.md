# Week 2: 4D-STEM Calibration Code Examples

This directory contains practical code examples demonstrating how to calibrate 4D-STEM data using py4DSTEM. All examples use the Si-Au reference dataset (`SI_Au_calib.dm4`) located in `raw_data/`.

## Contents

### 1. `example_01_calibration.ipynb`
**Basic Calibration Workflow**

This notebook covers the fundamentals of 4D-STEM calibration:
- Loading experimental datasets with py4DSTEM
- Understanding diffraction pattern coordinates and reciprocal space
- Basic origin calibration (finding the diffraction pattern center)
- Converting detector pixels to reciprocal space (k-space)
- Converting scan pixels to real space
- Creating virtual detectors by integration
- Saving calibration parameters for future use

**Key Learning Points:**
- Dataset structure and indexing
- Reciprocal space concept
- Manual parameter calibration
- Virtual image generation

**Duration:** ~15 minutes to run

---

### 2. `example_02_bragg_calibration.ipynb`
**Advanced Calibration: Bragg Spot Detection**

This notebook demonstrates automated calibration using crystallographic Bragg spots:
- Peak finding in diffraction patterns
- Identifying Bragg reflections
- Using known lattice parameters for calibration
- Automated pixelsize determination
- Validation with multiple crystallographic reflections
- Refining origin position using symmetry

**Key Learning Points:**
- Image processing for peak detection
- Crystal structure and reciprocal lattice
- Bragg's law and scattering vectors
- Automated calibration workflow
- Cross-validation with multiple reflections

**Duration:** ~20 minutes to run

**Requirements:** More sophisticated image processing than Part 1

---

### 3. `example_03_calibration_practices.ipynb`
**Best Practices and Troubleshooting**

This notebook provides practical guidance for reliable calibration:
- Systematic calibration workflow
- Data quality assessment
- Common calibration mistakes and how to avoid them
- Quality metrics for calibration
- Comprehensive calibration record storage
- Reproducibility checklist

**Key Learning Points:**
- How to assess data quality
- Common pitfalls and solutions
- Uncertainty quantification
- Best practices for reproducibility
- When to recalibrate

**Duration:** ~10 minutes to run

---

## Quick Start

### Run all examples:
```python
# In terminal or VS Code
jupyter notebook Week_02/code_examples/
```

### Or run individually:
```python
# Load one example
import jupyter
jupyter.run_line_magic('run', 'example_01_calibration.ipynb')
```

## Data Requirements

All examples require the SI-Au calibration reference dataset:
- **File:** `raw_data/SI_Au_calib.dm4`
- **Material:** Silicon-gold heterostructure
- **Orientation:** [110] zone axis (typical)
- **Quality:** Well-crystallized with clear Bragg spots

If the file is missing:
1. Check that `raw_data/SI_Au_calib.dm4` exists
2. If not, download from the course repository
3. Place in the `raw_data/` folder

## Learning Path

**Recommended order:**
1. Start with `example_01_calibration.ipynb` for fundamentals
2. Move to `example_02_bragg_calibration.ipynb` for automation
3. Finish with `example_03_calibration_practices.ipynb` for practical tips

**If short on time:**
- Quick overview: Run Part 1 only (~15 min)
- Intermediate: Parts 1 + 3 (~25 min) 
- Full understanding: All three (~45 min)

## Concepts Covered

### Part 1: Fundamentals
- [ ] Dataset loading and inspection
- [ ] Diffraction pattern visualization
- [ ] Origin determination
- [ ] Reciprocal space mapping
- [ ] Real-space calibration
- [ ] Virtual detector integration
- [ ] Parameter storage

### Part 2: Advanced Techniques  
- [ ] Peak detection algorithms
- [ ] Bragg spot identification
- [ ] Lattice parameter lookup
- [ ] Automated calibration calculation
- [ ] Multi-feature validation
- [ ] Symmetry analysis

### Part 3: Practical Considerations
- [ ] Data quality metrics
- [ ] Common mistakes and fixes
- [ ] Uncertainty quantification
- [ ] Calibration validation
- [ ] Metadata storage
- [ ] Reproducibility practices

## Key Takeaways

1. **Calibration is Essential:** Converting pixel coordinates to physical units is fundamental for quantitative analysis

2. **Multiple Methods:** Simple geometric estimation vs. sophisticated crystallographic methods - choose based on accuracy needs

3. **Validation is Critical:** Always verify calibration with independent measurements and multiple samples

4. **Documentation Matters:** Record detailed metadata for reproducibility and future reference

5. **Quality Assessment:** Quantify uncertainties - the best calibration is useless if you don't know its accuracy

## Further Resources

### Related Exercises
- `exercise_02_4dstem_basics.ipynb` - Basic 4D-STEM data handling
- `exercise_02_hyperspy_basics.ipynb` - HyperSpy integration

### Assignment
- `assignment_02_setup.ipynb` - Full assignment with calibration tasks
- `assignment_02_solutions.ipynb` - Reference solutions

### External References
- [py4DSTEM Documentation](https://py4dstem.readthedocs.io/)
- [py4DSTEM Tutorials](https://github.com/py4dstem/py4DSTEM_tutorials/)
- [4D-STEM Review Paper](https://advances.sciencemag.org/content/4/9/eaap9437)

## Tips & Tricks

### Speed up loading:
```python
# Load only the data you need
dataset = py4DSTEM.io.import_file(filepath, 
                                  select_scan=[100:200, 100:200])
```

### Better peak detection:
```python
# Use Gaussian fitting instead of max pixel
from scipy.optimize import curve_fit
# ... (see example_02 for full implementation)
```

### Validate across scan area:
```python
# Check calibration consistency
calib_by_region = {}
for i in range(0, dataset.shape[2], 50):
    for j in range(0, dataset.shape[3], 50):
        # Calibrate this region
        # Store in dict
```

## Troubleshooting

### "File not found: SI_Au_calib.dm4"
- Verify file location: `/Week_02/raw_data/SI_Au_calib.dm4`
- Check file exists: `ls -lh raw_data/SI_Au_calib.dm4`

### "No peaks detected"
- Check data quality (not too noisy or saturated)
- Lower the percentile threshold (default: 99th)
- Try different neighborhood sizes for peak detection

### "Calibration values seem wrong"
- Verify reference lattice parameters
- Check zone axis orientation
- Look for detector distortion or rotation

## Questions or Issues?

Refer to the assignment solutions or discuss with the instructor during office hours.

---

**Last updated:** January 2026
**Course:** MATS 465 - Computational Microscopy
**Instructor:** [Your Name]
