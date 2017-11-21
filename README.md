<h1><a href="http://www.lisym.org/" alt="LiSyM" target="_blank"><img src="./images/lisym.png" height="45"></a> 1st LiSyM Modeling Tutorial</h1>

[![GitHub version](https://badge.fury.io/gh/matthiaskoenig%2Flisym-tutorial.svg)](https://badge.fury.io/gh/matthiaskoenig%2Flisym-tutorial)
[![DOI](https://www.zenodo.org/badge/111459301.svg)](https://www.zenodo.org/badge/latestdoi/111459301)  
<b><a href="https://orcid.org/0000-0003-1725-179X" title="https://orcid.org/0000-0003-1725-179X"><img src="./images/orcid.png" height="15"/></a> Matthias König</b>

Modeling tutorial as part of the 1st LiSyM Retreat Meeting in Hünfeld (20-22 November 2017). The presentation slides are available [here](./presentation/lisym-tutorial.pdf). 

This tutorial gives a quick introduction into standards used in computational modeling and visualizes, simulates and analysis showcase example models. A basic introduction to simple kinetic models is provided.

The entry point for the notebooks is the [index.ipynb](./index.ipynb).

## Resources
#### Standard formats
* [Systems Biology Markup Language (SBML)](http://sbml.org/Main_Page)
* [Simulaltion Experiment Description Markup Language (SED-ML)](https://sed-ml.github.io/)

#### Model repositories
* [BioModels](https://wwwdev.ebi.ac.uk/biomodels/)

#### Network visualization of SBML models
* [Cytoscape](http://www.cytoscape.org/) network visualization software
* SBML visualization with [`cy3sbml`](http://github.com/matthiaskoenig/cy3sbml) (http://apps.cytoscape.org/apps/cy3sbml)

#### Modeling software
* [tellurium](http://tellurium.analogmachine.org/): A Python Environment for Reproducible Dynamical Modeling of Biological Networks
* [tellurium readthedocs](https://tellurium.readthedocs.io/en/latest/)
* [libroadrunner](http://libroadrunner.org/)

#### Interactive notebooks
* [Jupyter notebooks](https://jupyter.org/)


## License and citation
If you refer to this material or reuse it cite  
[![DOI](https://www.zenodo.org/badge/111459301.svg)](https://www.zenodo.org/badge/latestdoi/111459301)

* Source Code is licensed as [LGPLv3](http://opensource.org/licenses/LGPL-3.0)
* Documentation is licensed as [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)


## Funding
Matthias König is supported by the Federal Ministry of Education and Research (BMBF, Germany) 
within the research network Systems Medicine of the Liver (LiSyM, grant number 031L0054).

<a href="http://www.lisym.org/" alt="LiSyM" target="_blank"><img src="./images/lisym.png" height="45"></a> &nbsp;&nbsp;
<a href="http://www.bmbf.de/" alt="BMBF" target="_blank"><img src="./images/bmbf.png" height="45"></a> &nbsp;&nbsp;


## Instructions
To run the tutorial notebooks download the latest release from
https://github.com/matthiaskoenig/lisym-tutorial/releases  
Extract the files, the notebooks are in the `./notebooks/` folder.
 
### Running examples with tellurium-notebook 
For running the notebooks with tellurium-notebook [download the latest version](https://github.com/sys-bio/tellurium#installation-instructions). After installation open the notebooks via `File -> Open`.

### Running jupyter notebook in virtualenv
tellurium is also available as python package and can simply be installed in a virtual environment. Jupyter notebooks can than use the virtualenv as kernel.  
```
git clone https://github.com/matthiaskoenig/lisym-tutorial.git
cd lisym-tutorial
mkvirtualenv lisym --python=python3
(lisym) pip install -r requirements.txt

# install kernel for ipython
(lisym) python -m ipykernel install --user --name=lisym

# start jupyter notbook
jupyter notebook index.ipynb

# select notebook for model and run notbook with the dfba kernel
Kernel -> Change kernel -> dfba
Kernel -> Restart & Run All
```
