
# **Medical**.ml Dask & Pandas Workshops

<img src="medicalml.png" width="1000">

**Wroclaw University of Science and Technology** Faculty of Computer Science and Management

**medical**.**ml** Students Research Group

## Getting started - what is it about?
Medical.&#x200B;ml workshops on data processing tools:
 - pandas - processing tabular data
 - dask - parallel and cluster-distributed processing
## Prerequisites & Installation

### Docker 
At some point in the future...

### Local Environment

You can set up all requirements in your own environment without building Docker images. You'll need:
1. Conda or another python distribution with packages:
	- `pandas 0.20.0+`
	- `numpy 1.13.0+`
	- `dask 0.16.0+` (preinstalled with conda, make sure you have the latest version)
	- `bokeh 0.12.10+` (preinstalled with conda, make sure you have the latest version)
	- `scikit-learn`
2. (Optional) Graphviz:
	* Download from https://www.graphviz.org/download/
	(or `apt-get install graphviz` on Linux)
	* Install python package `graphviz`. 
		>**Note 1:** install with `pip install graphviz` rather than with `conda install`. Conda sometimes messes this up.
		> **Note 2:** On Windows you may need to manually set up your environment path, or do so right in your code with:
		```python
		import os
		os.environ["PATH"] += os.pathsep + 'disk/install/path/Graphviz2.38/bin/' 
		```
		> **Note 3:** The Graphviz provides a handy functionality to the Dask library but is not at all required for it to run properly, so it's up to you to decide whether to install it or not.


## Workshop notebooks
Workshop content is located in the `./notebooks/` directory in a form of Jupyter Notebook files. Their content may differ in the future, so be sure to pull the latest version :)


## But why all this? 
\> Ugly Data
\> Pandas, Numpy, **Dask**, ...
\> Beautiful Data
\> Machine Learning
\> ???
\> ???
\> ???
\> **Profit**
