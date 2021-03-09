# jupyter/julia-notebook
Based on : https://raw.githubusercontent.com/jupyter/docker-stacks/master/datascience-notebook/Dockerfile

## Build
Run `docker build -t julia-notebook:1.5.3 .`.  

## Use
Run `docker run --rm -p 8888:8888 julia-notebook:1.5.3`.  
Download your files before closing, `--rm` removes the container when closing!
