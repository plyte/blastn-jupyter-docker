# Blastn and Jupyter Docker source image

This repo contains source files for a Dockerfile which contains two tools and a sample notebook:
 - Jupyter notebook container pulled from [source](https://github.com/jupyter/docker-stacks/tree/master/base-notebook).  
 - blastn genomics tool (installed during the container build via `'apt-get...`)
 - IPython notebook based on the blastn tutorial from [source](https://github.com/edamame-course/BLAST-tutorial/blob/master/running-BLAST.md). 

To use this image:
1) Clone the repo
2) Run `docker build -t blastn-jupyter-docker .`
3) Wait for the build to complete (takes ~15 minutes)
4) Run `docker run -p 8888:8888 blastn-jupyter-docker`
4) Connect to the sample Jupyter notebook in your browser using the link generated
5) Navigate and run the jupyter notebook located in /work/

[![blastn-jupyter-notebook](/images/blast-jupyter-notebook.png)]()
