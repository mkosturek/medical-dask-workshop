# **Medical**.ml Dask & Pandas Workshops

<img src="medicalml.png" width="1000">
**Wroclaw University of Science and Technology** Faculty of Computer Science and Management

**medical**.**ml** Students Research Circle

## Getting started - what is it about?
Medical.&#x200B;ml workshops on data processing tools:
 - pandas - processing tabular data
 - dask - parallel and cluster-distributed processing
## Prerequisites & Installation

### I. Docker
This project is distributed together with a `Dockerfile` (and some additional scripts) and a `docker-compose.yaml`

1. **First-time building and running docker image and container:**
	To set up a Docker image that will be used during workshops just enter a docker-compose command (after `cd`'ed into this project's directory):
	```
	$: docker-compose up
	```
	Then the `jupyter/base-notebook` docker image will be downloaded (about 800 MB) and configured (additional downloads, including MNIST dataset) to build the `medical/daskworkshop` image (about 2.27 GB).

	Also a container called `medical-dask-workshops` will be created. It will run the jupyter notebook by default with a token: **`magicalml`**.

2. **Second-and-succedent runs:**
	Again you can use command
	```bash
	docker-compose up
	```
	This time it will not build the image all over again but only run the existing container. (To force rebuilding the image just add `--build` argument)
	
	Alternatively you can enter:
	```bash
	docker start -it medical-dask-workshops
	```
3. **Accessing the container's bash terminal:**
	In order to get access to container's bash just enter this command in a separate terminal with container already up and running:
	```bash
	docker exec -it medical-dask-workshops bash
	```
	
	Alternatively you can use the terminal provided by the Jupyter Notebook.

### II. Your local environment
You can set up all requirements in your own environment without building Docker images. To do so just look inside the `./dockerconfig/Dockerfile` to see what prerequisites you will need. 

> **Note 1:** The Graphviz provides a handy functionality to the Dask library but is not at all required for it to run properly, so it's up to you to decide whether to install it or not.

> **Note 2:** The Graphviz installation on Windows is slightly more complex than on Linux (but still quite easy and you can easily google it).


## Workshop notebooks
Workshop content is located in the `./notebooks/` directory in a form of Jupyter Notebook files. Their content may differ in the future, so be sure to pull the latest version :)

> **Note:** The Docker configuration should in general stay unchanged. However when some change is required it will be prompted at the top of this README


## But why all this? 
\> Ugly Data
\> Pandas, Numpy, **Dask**, ...
\> Beautiful Data
\> Machine Learning
\> ???
\> ???
\> ???
\> **Profit**