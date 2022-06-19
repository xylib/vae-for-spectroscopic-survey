# Investigation of stellar magnetic activity using VAE

[![arXiv](https://img.shields.io/badge/arXiv-2206.07257-B31B1B.svg)](http://arxiv.org/abs/2206.07257)

The variational autoencoder (VAE) for the investigation of the stellar magnetic activity based on low-resolution spectroscopic surveys.

The purpose of this VAE model is to generate the inactive template spectra in an unsupervised manner. After subtracting the reference templates from the observed stellar spectra, we can measure the residual emissions of the chromospheric indicators, such as Halpha and Ca II IRT lines, to quantify the activity level of stars.

<p align="center"><img src="data/example.png" width="90%" height="90%"></p>

The unsupervised VAE model is efficient for the analysis of the stellar magnetic activity in large spectroscopic surveys, since it do not need to know any stellar parameters or perform the template matching with the stellar spectral library. We trained the model on the selected inactive spectra in the LAMOST-K2 database, and the details can be found in the paper.

We provide the Jupyter notebook as well as 1000 LAMOST spectra and the corresponding degraded ones (simulate the CSST slitless spectra) for the demo.

## Requirements

* h5py
* tqdm
* numpy
* joblib
* pytorch
* matplotlib
* scikit-learn
