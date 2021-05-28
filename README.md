# jupyter/julia-notebook
Based on : https://raw.githubusercontent.com/jupyter/docker-stacks/master/datascience-notebook/Dockerfile

## Build
Run (for ./jupyter) `docker build -t julia-notebook:1.5.3 .`.  
Run (for ./python) `docker build -t julia-notebook:python .`.  

## Use
Run (for ./jupyter) `docker run --rm -p 8888:8888 -v "${PWD}:/home/jovyan/work" julia-notebook:1.5.3`.
Run (for ./python) `docker run --rm -p 8888:8888 -v "${PWD}:/root/work" julia-notebook:python`.  
Make sure to save your files to `~/work` in the container so that they are written to the host, `--rm` removes the container when closing!
