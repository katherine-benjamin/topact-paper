This repository contains some code used for the paper "Multiscale topology classifies and quantifies cell types in subcellular spatial transcriptomics".

The software package TopACT can be found separately: https://gitlab.com/kfbenjamin/topact

TopACT is necessary to run the code in this repository. You can install it with

```pip install git+https://gitlab.com/kfbenjamin/topact.git```

## Clinical data

Clinical data for the preprint is currently not available. As such, this repository does not contain specific code used to produce TopACT predictions for either clinical or synthetic data (the latter requiring a clinical snRNA-seq reference data set). Clinical data, and all relevant code, will be made available on publication.

For synthetic data, a pickled version of the classifier used is available on request. However, due to the security risks inherent with pickling python objects, we do not publish it here.
