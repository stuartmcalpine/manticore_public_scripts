# Manticore-Local Data Analysis Notebooks

Helper notebooks for reading and analyzing data from the **Manticore-Local** project, a Bayesian constrained simulation suite of our cosmic neighborhood.

## About Manticore-Local

Manticore-Local presents high-fidelity reconstructions of the local Universe (R < 200 Mpc) using Bayesian field-level inference applied to the 2M++ galaxy catalogue. The project identifies and characterizes prominent galaxy clusters including Virgo, Coma, Perseus, and others through constrained cosmological simulations.

**Publication**: [McAlpine et al. 2025, MNRAS 540, 716](https://ui.adsabs.harvard.edu/abs/2025MNRAS.540..716M/abstract)

## Notebooks

### 1. `manticore_local_prominant_clusters.ipynb`

Demonstrates how to read and analyze the **14 prominent galaxy clusters** from the Manticore-Local paper.

- **Data**: `clusters.dat` (fixed-width format, 80 posterior samples per cluster)
- **Source**: [VizieR Catalog J/MNRAS/540/716](https://cdsarc.cds.unistra.fr/viz-bin/cat/J/MNRAS/540/716)
- **Contents**: Cluster positions, masses (M200/M500), velocities, and detection significance

**Examples**:
- Loading and parsing fixed-width cluster data
- Calculating median masses with 10th-90th percentile uncertainties
- Visualizing mass distributions with error bars
- Examining posterior distributions for individual clusters

### 2. `manticore_local_posterior_cluster_catalog.ipynb`

Demonstrates how to work with the **full Manticore-Local posterior cluster catalog** containing halo associations across the entire simulation ensemble.

- **Data**: `manticore_local_posterior_cluster_catalog.h5` (HDF5 format)
- **Source**: [www.cosmictwin.org](https://www.cosmictwin.org)
- **Publication**: [PLACEHOLDER: Insert catalog paper reference]
- **Contents**: Comprehensive halo properties including positions, masses, velocities, concentrations, and satellite fractions

**Examples**:
- Loading hierarchical HDF5 catalog structure
- Visualizing association positions on the sky (RA/Dec distributions)
- Accessing posterior samples for individual halo associations
- Analyzing mass-concentration relations
- Comparing properties across multiple associations

## Requirements

```python
numpy
matplotlib
pandas
h5py  # for HDF5 catalog
```

## Project Links

- **Project Website**: [www.cosmictwin.org](https://www.cosmictwin.org)
- **Paper**: [McAlpine et al. 2025, MNRAS 540, 716](https://ui.adsabs.harvard.edu/abs/2025MNRAS.540..716M/abstract)
- **VizieR Data**: [J/MNRAS/540/716](https://cdsarc.cds.unistra.fr/viz-bin/cat/J/MNRAS/540/716)
