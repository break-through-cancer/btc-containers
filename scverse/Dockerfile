FROM python:3.11

RUN pip install --upgrade pip
RUN pip install anndata \
                mudata \
                spatialdata \
                scanpy \
                muon \
                scvi-tools \
                scirpy \
                squidpy \
                spatialdata_io \
                seaborn \
                pandas \
                boto3
                
#cure ligrec p-value NaN 
RUN pip install git+https://github.com/scverse/squidpy@349b75afbd26a9a5b832b9243bcd3fdf79cf0ea6           
