FROM nvcr.io/nvidia/pytorch:19.11-py3
LABEL maintainer="wfedorko@triumf.ca"

RUN apt-get update
RUN apt-get --yes upgrade && apt-get --yes install strace locate pydb ddd libxtst6 libxtst-dev 

RUN pip install xgboost lightgbm seaborn h5py plotly torchviz line_profiler

RUN wget https://download.jetbrains.com/python/pycharm-community-2019.2.3.tar.gz?_ga=2.141719730.1677997767.1570599993-1937107941.1570599993 && tar xfz pycharm-*.tar.gz* -C /opt/ && rm -r pycharm-*.tar.gz*

