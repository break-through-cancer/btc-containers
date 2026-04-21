FROM python:3.11

RUN pip install --upgrade pip

#avoid pyarrow EOF error in xenium
RUN pip install pyarrow==21 \
                scipy==1.12

RUN pip install anndata \
                spatialdata \
                scanpy \
                spatialdata_io \
                seaborn \
                pandas \
                boto3 \
                pydeseq2
                
#grab new co-occurrence version
RUN pip install git+https://github.com/scverse/squidpy@32789aefd53b797ceee8c3153beded2f46a2cd4c           
