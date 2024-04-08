This repository contains some of the code and data used for the preprint "Multiscale topology classifies and quantifies cell types in subcellular spatial transcriptomics". Please note that code requiring clinical data will be made available on publication.

The Python package TopACT can be found separately: https://gitlab.com/kfbenjamin/topact. It requires Python (3.10.0 or newer).

TopACT is necessary to run the code in this repository. You can install it with

```pip install git+https://gitlab.com/kfbenjamin/topact.git```.

## Figure 1

Code used to generate Figures 1E and 1F are included in the `Figure 1` directory.

## Synthetic data

The `Figure 2` directory contains code for generating synthetic data. This data is stored in `syntheticdata`:

- `syntheticdata/groundtruth` records the ground-truth cell type spatial maps
- `syntheticdata/expression` records the synthetic gene expression data

Also included are TopACT and RCTD predicted cell types generated from the expression data.

The `Model diffusion.ipynb` notebook contains the code used to perturb generated data according to the molecular diffusion model described in the paper. ALso included are the outputs of this process as well as the correspondong TopACT and RCTD predictions.

The `Figure 2` directory also includes notebooks generating each of Figures 2b,c,d, and e.

## Clinical data

Clinical data for the preprint is currently not available. As such, this repository does not contain specific code used to produce TopACT predictions for either clinical or synthetic data (the latter requiring a clinical snRNA-seq reference data set). Clinical data, and all relevant code, will be made available on publication.

For synthetic data, a pickled version of the classifier used is available on request. However, due to the security risks inherent with pickling python objects, we do not publish it here.

## RCTD

For experiments on synthetic data, we used RCTD on binned data. Please see the [spacexr package](https://github.com/dmcable/spacexr) for tutorials on using RCTD.

## Multiparameter persistent homology (MPH)

We used [RIVET](https://rivet.readthedocs.io/en/latest/) and the code available at https://github.com/MultiparameterTDAHistology/SpatialPatterningOfImmuneCells to compute MPH landscapes.
