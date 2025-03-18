FROM rocker/tidyverse:4

RUN sudo apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install libhdf5-dev build-essential patch python3-venv python3-pip python3-dev -y

WORKDIR /app
RUN python3 -m venv venv && \
    . venv/bin/activate && \
    pip install --upgrade pip && \
    pip install anndata

RUN Rscript -e 'install.packages("reticulate", repos = "https://cloud.r-project.org")'
RUN Rscript -e 'devtools::install_github("dmcable/spacexr", dependencies = TRUE)'
