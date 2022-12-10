This repository contains some code used for the paper "Multiscale topology classifies and quantifies cell types in subcellular spatial transcriptomics".

The software package TopACT can be found separately: https://gitlab.com/kfbenjamin/topact

TopACT is necessary to run the code in this repository. You can install it with

```pip install git+https://gitlab.com/kfbenjamin/topact.git```.

## Synthetic data

We include here, in the `Figure 2` directory, code for generating synthetic spatial data. We also include the 100 synthetic samples analyzed in the paper, as well as TopACT and RCTD predicted outputs on these samples as well as code to generate the corresponding parts of Figure 2 in the manuscript. Note that we do not include specific code used to generate these TopACT predictions at this time -- see the below note on clinical data.

## Clinical data

Clinical data for the preprint is currently not available. As such, this repository does not contain specific code used to produce TopACT predictions for either clinical or synthetic data (the latter requiring a clinical snRNA-seq reference data set). Clinical data, and all relevant code, will be made available on publication.

For synthetic data, a pickled version of the classifier used is available on request. However, due to the security risks inherent with pickling python objects, we do not publish it here.

## RCTD

For experiments on synthetic data, we used RCTD on binned data. Please see the [spacexr package](https://github.com/dmcable/spacexr) for tutorials on using RCTD.

## Multiparameter persistent homology (MPH)

We used [RIVET](https://rivet.readthedocs.io/en/latest/) and the code available at https://github.com/MultiparameterTDAHistology/SpatialPatterningOfImmuneCells to compute MPH landscapes.
