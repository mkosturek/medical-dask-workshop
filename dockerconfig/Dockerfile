FROM jupyter/base-notebook

USER root

RUN sudo apt update
RUN sudo apt install graphviz -y

RUN conda install --yes -c conda-forge \
	scikit-learn \
	numpy \
	pandas \
    dask \
    distributed \
	graphviz \
 	jupyter_contrib_nbextensions \
    && conda clean -tipsy
	

USER jovyan
COPY download_mnist.py /home/jovyan/download_mnist.py
RUN python /home/jovyan/download_mnist.py
