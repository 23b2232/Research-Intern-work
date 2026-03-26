# Exoplanet Research and Detection

## Overview

This repository combines two complementary projects in exoplanet science:

1. **Astrophysical Analysis of the Radius Valley**
2. **Machine Learning-based Exoplanet Detection using Kepler Light Curves**


## Project 1: Radius Valley Analysis

### Objective

Investigate the Radius Valley, a gap in exoplanet radii between 1.5–2.0 Earth radii, separating:

* Super-Earths
* Sub-Neptunes

### Context

Conducted during a research internship at the Tata Institute of Fundamental Research (TIFR).

### Dataset

* Source: NASA Exoplanet Archive
* ~3000+ multiplanetary systems (Kepler + TESS)

### Methodology

* Data cleaning (interpolation + imputation)
* Filtering:
  * Stellar temperature: 3000–7000 K
  * Planet radius ≤ 4 Earth radii
* Feature computation:
  * Luminosity: $L = 4\pi R_*^2 \sigma T_{eff}^4$
  * Irradiation: $S = \frac{L}{4\pi a^2}$
  * Atmospheric loss proxy: $\frac{\Delta R}{\Delta \log_{10}(S)}$


## Project 2: Exoplanet Detection using ML

### Objective

Detect exoplanets by identifying transit signals in light curve data.

### Dataset

* Kepler Telescope data
* `.fits` time-series format

### Pipeline

#### Data Processing

* FITS → Pandas conversion
* Missing value handling
* Normalization + smoothing

#### Feature Engineering

* Time-series segmentation
* Threshold-based labeling

#### Models Implemented

* Logistic Regression
* LSTM
* GRU
* 1D CNN (final model)

## Results & Observations

### ML Model

* High accuracy but poor recall due to **class imbalance**
* Demonstrates need for better labeling and balancing techniques

### Scientific Analysis

* Confirms **photoevaporation** as a key mechanism
* Variation across stellar types suggests **mass-dependent evolution**


## Author

**Yashasvee Taiwade**
