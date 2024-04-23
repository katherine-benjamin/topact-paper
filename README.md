NOTE: This repository is currently being updated to reflect a new version of the manuscript and so details may be innacurate, incomplete, and inconsistent.

This repository contains code used for the experiments in the paper "Multiscale topology classifies cells in subcellular spatial transcriptomics".

The Python package TopACT can be found separately: https://gitlab.com/kfbenjamin/topact. It requires Python (3.10.0 or newer).

TopACT is necessary to run the code in this repository. You can install it with

```pip install git+https://gitlab.com/kfbenjamin/topact.git```.

## Data

TopACT output, and related output data, are available at DOI GOES HERE. You should download this data set and place it in the base level of this directory before running any code.

Raw data files are available online as described in the paper.

## Figure 1

Code used to generate Figures 1E and 1F are included in the `Figure 1` directory.

## Figure 2

The `Figure 2` directory contains code for generating synthetic data.

The `Model diffusion.ipynb` notebook contains the code used to perturb generated data according to the molecular diffusion model described in the paper.

The directory also includes notebooks generating each of Figures 2b,c,d, and e.

## Figure 3

The `Figure 3` directory contains code necessary to extract PVM loci from the TopACT output on the adult mouse brain data set (Chen et al., 2022). Since the data set is very large, we include the relevant subsets of the data in helper files in this directory. Once PVM loci are extracted, two further notebooks detail the generation of the relevant scatter and violin plot figures.

## Figure 4

The `Figure 4` directory contains analysis code for the human kidney Xenium experiment. It also contains the Xenium output cell boundaries and corresponding supervised annotation for convenience. `dapi.png` and `hande.png` are images used to generate figures. 

## Figure 5

This directory contains analysis code for the Stereo-seq and Vectra mouse kidney experiments. Also included is source data for producing Vectra-related graphs, which is also available with the paper.

## Extended Data Figure

The Extended Data Figure showing ssDNA-based cell segmentation of mouse kidney in comparison to TopACT predictions can be generated with the notebook in the `Extended Figures` directory.

## RCTD

For experiments on synthetic data, we used RCTD on binned data. Please see the [spacexr package](https://github.com/dmcable/spacexr) for tutorials on using RCTD.

## Multiparameter persistent homology (MPH)

We used [RIVET](https://rivet.readthedocs.io/en/latest/) and the code available at https://github.com/MultiparameterTDAHistology/SpatialPatterningOfImmuneCells to compute MPH landscapes.
