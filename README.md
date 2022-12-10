This repository contains some code used for the paper "Multiscale topology classifies and quantifies cell types in subcellular spatial transcriptomics". Please note that code requiring clinical data will be made available on publication.

The software package TopACT can be found separately: https://gitlab.com/kfbenjamin/topact

TopACT is necessary to run the code in this repository. You can install it with

```pip install git+https://gitlab.com/kfbenjamin/topact.git```.

## Figure 1

Code used to generate Figures 1E and 1F are included in the `Figure 1` directory.

## Synthetic data

We include here, in the `Figure 2` directory, code for generating synthetic spatial data. The `syntheticdata` directory contains the synthetic ground truth cell type maps, TopACT predictions, and RCTD predictions analyzed in the paper. Code for producing Figure 2B, showing example classifications, and Figure 2C, showing the accuracies of these methods, is also included in the `Figure 2` directory. Note that we do not include specific code used to generate these TopACT predictions at this time -- see the below note on clinical data.

## Clinical data

Clinical data for the preprint is currently not available. As such, this repository does not contain specific code used to produce TopACT predictions for either clinical or synthetic data (the latter requiring a clinical snRNA-seq reference data set). Clinical data, and all relevant code, will be made available on publication.

For synthetic data, a pickled version of the classifier used is available on request. However, due to the security risks inherent with pickling python objects, we do not publish it here.

## RCTD

For experiments on synthetic data, we used RCTD on binned data. Please see the [spacexr package](https://github.com/dmcable/spacexr) for tutorials on using RCTD.

## Multiparameter persistent homology (MPH)

We used [RIVET](https://rivet.readthedocs.io/en/latest/) and the code available at https://github.com/MultiparameterTDAHistology/SpatialPatterningOfImmuneCells to compute MPH landscapes.
