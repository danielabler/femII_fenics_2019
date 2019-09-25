# README

## Install FEniCS using Anaconda

- create conda environment *fenicsenv* for FEniCS, including [FEniCS](https://fenicsproject.org/), [mshr](https://bitbucket.org/fenics-project/mshr/src/master/),
 [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/), [NumPy](https://numpy.org/) and [matplotlib](https://matplotlib.org/). 
    ```shell script
    conda create --name fenicsenv -c conda-forge python=3.7 fenics jupyterlab mshr matplotlib numpy 
    ```
  or using the *conda-environment.yaml* file
    ```shell script
    conda env create -f conda-environment.yaml
    ```
  
- After activating this environment
    ```shell script
    source activate fenicsenv
    ```
  you should see *(fenicsenv)* at the beginning of your commandline.
- Optionally install [dolfin-adjoint](http://www.dolfin-adjoint.org/en/release/)
    ```shell script
    conda install -c conda-forge dolfin-adjoint
    ```
- You can now call *python*, *ipython* or *jupter lab*
    ```shell script
    jupyter lab
    ```
  
## Links

- For general links about FEniCS see `00_intro_to_fenics.ipynb` in this repository.
- [This website](http://comet-fenics.readthedocs.io/en/latest/index.html) discusses the solution of several mechanics 
problems using FEniCS. 
- [This repository](https://shaddenlab.gitlab.io/fenicsmechanics/index.html) provides an 
abstraction layer for mechanics simulation in FEniCS.