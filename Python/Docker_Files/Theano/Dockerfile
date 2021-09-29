FROM ghcr.io/deephaven/grpc-api

# Python installs followed by Theano optimization dependencies
RUN pip3 install theano; \
    pip3 install pymc3; \
    pip3 install mkl; \
    apt-get -y install python3-dev; \
    apt-get update; \
    apt-get -y install g++; \
    apt-get -y install libblas-dev
