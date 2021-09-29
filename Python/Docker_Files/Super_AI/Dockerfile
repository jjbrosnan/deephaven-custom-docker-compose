FROM ghcr.io/deephaven/grpc-api

# Python installs followed by Theano optimization dependency installs
RUN pip3 install theano; \
    pip3 install pymc3; \
    pip3 install mkl; \
    pip3 install tensorflow; \
    pip3 install torchvision; \
    pip3 install torchsummary; \
    pip3 install nltk; \
    pip3 install sklearn; \
    apt-get -y install python3-dev; \
    apt-get update; \
    apt-get -y install g++; \
    apt-get -y install libblas-dev
