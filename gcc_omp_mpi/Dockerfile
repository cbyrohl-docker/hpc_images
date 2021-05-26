FROM debian:10 

RUN apt-get -y -qq update && \
    apt-get -y -qq upgrade && \
    apt-get -y -qq install git cmake gcc g++ libopenmpi-dev libhdf5-openmpi-dev && \
    apt-get -y -qq clean && \
    rm -rf /var/lib/apt/lists/*

ENV CC=mpicc CXX=mpic++
