FROM ghcr.io/deephaven/grpc-api

# Install theano and pymc3
RUN pip3 install theano
RUN pip3 install pymc3
RUN pip3 install mkl

# Install GCC
RUN apt-get -y install python3-dev
RUN apt-get update && apt-get -y install g++
RUN apt-get -y install libblas-dev
