FROM debian:bullseye 

RUN apt-get -y -qq update && \
    apt-get -y -qq upgrade && \
    apt-get -y -qq install git cmake gcc g++ libopenmpi-dev libhdf5-openmpi-dev cppcheck && \
    apt-get -y -qq install python3 python3-matplotlib python3-numpy python3-h5py python3-astropy && \
    apt-get -y -qq clean && \
    rm -rf /var/lib/apt/lists/*

ENV CC=mpicc CXX=mpic++

RUN useradd -ms /bin/bash dummy
USER dummy 
WORKDIR /home/dummy
