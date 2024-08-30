# ZMB-IBEX-JOVE
Code to process multiplexing data, acquired with the MD ImageXpress microscope.

## Installation (Windows):

* Download and extract this repository at [https://github.com/ZMB-UZH/zmb-ibex-jove](https://github.com/ZMB-UZH/zmb-ibex-jove). (Either under 'Code' -> 'Download ZIP', or with `git clone git@github.com:ZMB-UZH/zmb-ibex-jove.git`)
* Change to the downloaded zmb-ibex directory:  
  e.g.: `cd C:\path\to\zmb-ibex-jove`
* Recommended: Install in separate conda environment (e.g. via [miniconda](https://docs.anaconda.com/miniconda/)):  
```
conda create -n zmb-ibex-jove python=3.9 -y
conda activate zmb-ibex-jove
```
* Install necessary packages:
```
pip install jupyterlab
pip install "jax[cpu]==0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
pip install ml-dtypes==0.2.0
pip install basicpy
pip install SimpleITK-SimpleElastix
pip install git+https://github.com/ZMB-UZH/zmb-hcs
```

## Start Jupyter:

* Activate the conda environment:  
  `conda activate zmb-ibex-jove`
* Change to directory, where jupyter-notebooks are:  
  e.g.: `cd C:\path\to\zmb-ibex-jove\examples`
* Start jupyter-lab:  
  `jupyter-lab`
* Edit and execute the notebooks
