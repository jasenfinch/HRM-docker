FROM ghcr.io/jasenfinch/ubuntu-r

MAINTAINER "Jasen Finch" jsf9@aber.ac.uk

ARG GITHUB_PAT

## Install external dependencies
RUN apt-get install -y \
  libnetcdf-dev \
  libhdf5-dev

RUN Rscript -e \
  'BiocManager::install("xcms")'

RUN chmod -R 777 /R