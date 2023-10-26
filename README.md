# 9780_SalomeStierli
Multiplexing Project

## Installation:
Note: These steps work on the ZMB-VMs. Please adapt accordingly if used somewhere else.

* Open 'Anaconda Powershell Prompt (MinicondaZMB)'
* When logging into a VM, the necessary conda-environment might not be installed. To list all installed environments, execute:  
  `conda env list`
* If 'zmb_hcs' is listed, you can skip ahead to 'Start Jupyter'. Otherwise continue with the installation steps:
* Download the repository at [https://github.com/fstur/zmb_hcs](https://github.com/fstur/zmb_hcs). (Under 'Code' -> 'Download ZIP')
* In the Anaconda Powershell Prompt, change to the downloaded zmb_hcs directory:  
  e.g.: `cd \path\to\zmb_hcs`
* Create conda environment and install packages:  
```
conda create -n zmb_hcs -c conda-forge python=3.9 -y
conda activate zmb_hcs
conda install -y -c conda-forge jupyterlab
conda install -y -c conda-forge nb_conda_kernels
pip install "napari[all]"
pip install "jax[cpu]==0.3.14" -f https://whls.blob.core.windows.net/unstable/index.html --use-deprecated legacy-resolver
pip install basicpy
pip install SimpleITK-SimpleElastix
pip install .
```

## Start Jupyter:

* Open 'Anaconda Powershell Prompt (MinicondaZMB)'
* Activate the conda environment:  
  `conda activate zmb_hcs`
* Change to directory, where jupyter-notebook is:  
  e.g.: `cd Z:\home\u.sername\notebooks`
* Start jupyter-lab:  
  `jupyter-lab --browser='C:/Program Files/Mozilla Firefox/firefox.exe %s'`

