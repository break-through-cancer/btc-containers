FROM python:3.11

RUN pip install --upgrade pip
RUN pip install anndata \
                spatialdata \
                scanpy \
                squidpy \
                spatialdata_io \
                seaborn \
                pandas \
                boto3
                
#grab new co-occurrence version
RUN pip install git+https://github.com/scverse/squidpy@32789aefd53b797ceee8c3153beded2f46a2cd4c           
