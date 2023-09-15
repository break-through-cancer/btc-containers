FROM rocker/tidyverse:4.3.1

RUN apt update && apt install -y libhdf5-dev build-essential patch

RUN git clone https://github.com/atuldeshpande/SpaceMarkers.git

RUN cd SpaceMarkers && Rscript -e "require('devtools'); devtools::install('.')"