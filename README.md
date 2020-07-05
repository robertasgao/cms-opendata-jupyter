# cms-opendata-jupyter
Jupyter notebooks demo using CMS opendata


## Getting the software ready

 1. **Anaconda**
 
In this tutorial, we are going to use the common analysis software in High Energy Experiment(HEP) called ROOT.
The easiest way to obtain it on a MAC is through anaconda.

Anaconda is a source-code distribution platform that help you download and manages a lot of scientific/data science packages. It helps you to maintain a correct dependency of each package,

You can obtain anaconda here:
https://www.anaconda.com/products/individual

I would recommend using the python3 version.

 2. **ROOT and Jupyter Notebook**
 
 The minimal packages we need are ROOT and jupyter notebook, which can be simply downloaded with:

```
conda install -c conda-forge root
conda install -c conda-forge notebook
```

`ROOT` may have some trouble working with `python3`. You can create a virtual environment specifying root with `python2.7` like this:

```
conda create --name pyroot root python=2.7
```

And then you can enter and exit the environment with 
```
conda activate pyroot
conda deactivate pyroot
```

 3. ** Download the datafile (~3GB) **

 After installing `ROOT`, open a terminal and execute the following command:

 `xrdcp root://eospublic.cern.ch//eos/root-eos/cms_opendata_2012_nanoaod/Run2012B_DoubleMuParked.root .`

