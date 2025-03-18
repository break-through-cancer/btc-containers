FROM rocker/tidyverse:4

RUN git clone https://github.com/dmcable/spacexr spacexr
WORKDIR /spacexr

RUN sudo apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install libhdf5-dev build-essential patch -y

RUN Rscript -e 'install.packages("reticulate")'

RUN Rscript -e 'devtools::install_deps()'

#https://github.com/r-lib/devtools/issues/2395
RUN Rscript -e 'devtools::install(dependencies = TRUE)'
