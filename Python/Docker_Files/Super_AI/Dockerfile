FROM ghcr.io/deephaven/grpc-api

# Install Theano and PyMC3
RUN pip3 install theano
RUN pip3 install pymc3
RUN pip3 install mkl
# Install TensorFlow
RUN pip3 install tensorflow
# Install PyTorch
RUN pip3 install torchvision
RUN pip3 install torchsummary
# Install NLTK
RUN pip3 install nltk
# Install SciKit-Learn
RUN pip3 install sklearn

# Install GCC and other Theano dependencies
RUN apt-get -y install python3-dev
RUN apt-get update && apt-get -y install g++
RUN apt-get -y install libblas-dev
