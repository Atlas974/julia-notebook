# jupyter/julia-notebook
Based on : https://raw.githubusercontent.com/jupyter/docker-stacks/master/datascience-notebook/Dockerfile

## Build
Run `docker build -t julia-notebook:1.5.3 .`.  

## Use
Run `docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan/work julia-notebook:1.5.3`.  
Make sure to save your files to `~/work` in the container so that they are written to the host, `--rm` removes the container when closing!
