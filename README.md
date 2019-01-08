# jupyter-docker
## modified to run with the controls and slycot library

# Build docker image:
## docker build . -t <name>
# spin up a container
# docker run -p 443:443  --name jup1 -it -v /homepath/:/root/work  <name of image>

This repositroy is forked from the [jupyter-alpine](https://github.com/Corneliuscob/jupyter-alpine) library and is installed with the controls and slycot library for the purpose of process control studies.

The default entrypoint is [jupyter-notebook-secure](util/jupyter-notebook-secure), which will generate a self-signed certificate and then launch the jupyter notebook server under HTTPS with an automatically-generated [authentication token](http://jupyter-notebook.readthedocs.io/en/stable/security.html).
