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
conda install matplotlib
```

`ROOT` may have some trouble working with `python3`. You can create a virtual environment specifying root with `python2.7` like this:

```
conda config --env --add channels conda-forge
conda create --name pyroot root python=2.7
```

And then you can enter and exit the environment with 
```
conda activate pyroot
conda deactivate pyroot
```
 3. **Running Jupyter Notebook**

 in order to run the notebook, execute the following command:

 ```root --notebook <notebook_name>```

 To run this notebook, execute:

 ```root --notebook 01-Introduction.ipynb```
