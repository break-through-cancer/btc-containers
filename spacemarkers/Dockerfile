FROM rocker/tidyverse:4

RUN git clone https://github.com/DeshpandeLab/SpaceMarkers.git spacemarkers
WORKDIR /spacemarkers

RUN sudo apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install libhdf5-dev build-essential patch -y

RUN Rscript -e 'install.packages("BiocManager");\
                BiocManager::install("CoGAPS")';

RUN Rscript -e 'devtools::install_deps()'

#https://github.com/r-lib/devtools/issues/2395
RUN Rscript -e 'devtools::install(dependencies = TRUE)'

#optoional packages - for vizualization
RUN Rscript -e 'install.packages("patchwork");\
                install.packages("ggplot2");\
                install.packages("dplyr");\
                install.packages("DT");\
                install.packages("Matrix");\
                install.packages("jsonlite");\
                install.packages("pheatmap");\
                install.packages("RColorBrewer")'
