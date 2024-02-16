# Gammapy, a Python package for gamma-ray astronomy

This repository collects the material for the course on Gammapy.

These presentation and 
hand-on sessions are made during the **school of the Astroparticle Physics Group at the São Carlos Institute of 
Physics of the University of São Paulo**, during the period of **February 17th to March 5th 2024**.

## Table of Contents
1. [Introduction to Gammapy](#intro)
2. [Installation and set-up](#install)
3. [First Hands-on](#first): spectrum and 3D analysis
4. [Second Hands-on](#second): data simulation
5. [Third Hands-on](#third): estimation of systematic errors 

## Introduction to Gammapy <a name="intro" />
During this presentation, Gammapy will be introduced. This open Python research software aims to analyse high-level 
data (under the [GADF](https://gamma-astro-data-formats.readthedocs.io/en/v0.3/) or 
[OGIP](https://heasarc.gsfc.nasa.gov/docs/heasarc/ofwg/docs/spectra/ogip_92_007/ogip_92_007.html) formats) from 
gamma-ray instruments, like H.E.S.S/MAGIC/VERITAS/CTA (using the Imaging Atmospheric Cherenkov Technique) or 
HAWC/SWGO (using the Water Cherenkov Technique), as well as Fermi-LAT. This software permits the production of the 
common very-high-energy astrophysical products (like flux maps, spectral energy distribution, time domain analysis). 
This talk will describe the library based on its version v1.1, its main features and data flow, the 
organization of the Gammapy project.

Link towards the general Presentation 

The basic data structures can be discovered with this 
[overview](https://docs.gammapy.org/1.1/tutorials/starting/overview.html).

The general web site of Gammapy is: https://gammapy.org/ .

The documentation web site of Gammapy is: https://docs.gammapy.org/1.1/index.html .

The GitHub repository of the Gammapy projet is: https://github.com/gammapy . 

## Installation and set-up <a name="install" />
The **version 1.1** of Gammapy will be used. See the 
[Quickstart Setup](https://docs.gammapy.org/1.1/getting-started/index.html#quickstart-setup) 
of the documentation to install the Gammapy v1.1 environment. You need also to download the datasets as explained.

Finally, **to get the tutorials** for these hands-on gammapy sessions, you can clone this repository on your machine using

```
git clone https://github.com/bkhelifi/Brazil_2024.git
```

To access the tutorials:

```
cd Brazil_2024
jupyter lab
```

To update your directory on disk:
```
cd Brazil_2024
git pull
```


## First hands-on session <a name="first" />
This first session aims to learn on your own laptop the basic uses of Gammapy, by using Jupyter Notebooks. We will 
work on the **extraction of a spectrum** from a point source, and on the **realization of a 3D analysis** of an extended 
source.

### [Spectral analysis of PKS 2155-304](https://github.com/bkhelifi/Brazil_2024/blob/main/1D_analysis.ipynb):
A full 1D (spectral) analysis tutorial from A to Z for a point-like extra-Galactic source.
### [3D analysis of MSH 15-52](https://github.com/bkhelifi/Brazil_2024/blob/main/3D_analysis_exercise.ipynb):
Exercise about a full 3D analysis for an extended Galactic source. The solution will be seen together.


## Second hands-on session <a name="second" />
This lecture will focus on the **simulations of data**, which then permits to asset the performances of an instrument 
to a given source or to realize studies on reconstruction quality (assessment of systematics errors). We will firstly
experience the simulations of a reduced binned dataset for a steady source and a time-variable object. The simulation
of a full event list will be introduced at the end.

### [Simulation of an extended source](https://github.com/bkhelifi/Brazil_2024/blob/main/simulate_3d.ipynb):
A full simulation tutorial from A to Z for an extented source having a power-law spectrum. The model parameters of the simulated dataset are retrieved.

### [Solution of the two exercises](https://github.com/bkhelifi/Brazil_2024/blob/main/simulate_3d_solution.ipynb):
- Exercise 1: retrieve the SkyModel parameters from the simulated dataset, compate them to the initial paramters, get the significance of the simulated source.
- Exercise 2: using simulations, determine the minimal time to detect significantly an exponential cut-off in the spectrum of a weak source

## Third hands-on session <a name="third" />
The last session will aim to **quantify systematic errors using simulations**. We will derive the errors on spectral 
parameters caused by a possible absolute energy scale bias or a possible background rate bias.

### [Spectral systematics study](https://github.com/bkhelifi/Brazil_2024/blob/main/Crab_simulations_systematic_errors_Exercise.ipynb)
