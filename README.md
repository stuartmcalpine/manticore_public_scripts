# Manticore-Local Data Analysis Notebooks

Helper notebooks for reading and analyzing data from the **Manticore-Local** project.

## About Manticore-Local

Manticore-Local (McAlpine et al. 2025, MNRAS 540, 716) is a suite of Bayesian constrained simulations of the nearby Universe (R < 200 Mpc), produced by applying field-level inference to the 2M++ galaxy catalogue using the BORG algorithm. The inference yields 80 independent posterior realizations of the local matter density and velocity fields, each physically consistent with ΛCDM structure formation. The ensemble recovers the spatial positions, masses, and velocities of 14 major galaxy clusters — including Virgo, Coma, and Perseus — to within 1° of their observed sky positions, and achieves the highest Bayesian evidence for the local peculiar velocity field across five independent datasets. The local supervolume shows no significant deviation from ΛCDM expectations, with a mean density suppressed by only ~5% relative to the cosmic mean.

**Publication**: [McAlpine et al. 2025, MNRAS 540, 716](https://ui.adsabs.harvard.edu/abs/2025MNRAS.540..716M/abstract)

## Notebooks

### 1. `manticore_local_prominant_clusters.ipynb`

Reads and plots posterior properties of the 14 prominent galaxy clusters identified in the Manticore-Local paper, using 80 MCMC samples per cluster to characterize mass uncertainties.

- **Data**: `data/prominant_cluster/clusters.dat` (fixed-width format) — [VizieR J/MNRAS/540/716](https://cdsarc.cds.unistra.fr/viz-bin/cat/J/MNRAS/540/716)

### 2. `manticore_local_posterior_cluster_catalog.ipynb`

Reads and plots the full Manticore-Local posterior halo association catalog, which groups dark matter halos across all 80 posterior realizations into spatially consistent associations with three selection tiers.

- **Data**: `data/manticore_local_posterior_cluster_catalog.h5` (HDF5 format) — [www.cosmictwin.org](https://www.cosmictwin.org)
- **Publication**: [McAlpine et al. 2025b](https://ui.adsabs.harvard.edu/abs/2025arXiv251016574M/abstract)

### 3. `manticore_data_tutorial.ipynb`

Demonstrates how to download and visualize simulation field data (density and velocity) from the Manticore-Local suite using the `manticore_data` Python package.

- **Package**: [`manticore_data`](https://git.aquila-consortium.org/Aquila-Consortium/manticore_data) — install with `pip install git+https://git.aquila-consortium.org/Aquila-Consortium/manticore_data/`

## Project Links

- **Project Website**: [www.cosmictwin.org](https://www.cosmictwin.org)
- **Paper**: [McAlpine et al. 2025, MNRAS 540, 716](https://ui.adsabs.harvard.edu/abs/2025MNRAS.540..716M/abstract)
- **VizieR Data**: [J/MNRAS/540/716](https://cdsarc.cds.unistra.fr/viz-bin/cat/J/MNRAS/540/716)
- **Data Package**: [manticore_data](https://git.aquila-consortium.org/Aquila-Consortium/manticore_data)
