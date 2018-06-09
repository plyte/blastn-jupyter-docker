# Blastn and Jupyter Docker source image

This repo contains source files for jupyter notebook which we pull from https://github.com/jupyter/docker-stacks/tree/master/base-notebook.
We modified the jupyter-notebook's Dockerfile inorder to add the blastn repository and created an ipython notebook based on the blastn tutorial from https://github.com/edamame-course/BLAST-tutorial/blob/master/running-BLAST.md. 

To use this image:
1) clone the repo
2) run this command: docker build -t blastn-jupyter-docker .
3) then once it finishes building run this: docker run -p 8888:8888 blastn-jupyter-docker
4) connect to the jupyter notebook in your browser using the link generated
5) navigate and run the jupyter notebook located in /work/

[![blastn-jupyter-notebook](/images/blast-jupyter-notebook.png)]()
