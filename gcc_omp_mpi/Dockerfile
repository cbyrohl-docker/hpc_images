FROM debian:10 

RUN apt-get -y -qq update && \
    apt-get -y -qq upgrade && \
    apt-get -y -qq install cmake gcc libopenmpi-dev && \
    apt-get -y -qq clean && \
    rm -rf /var/lib/apt/lists/*

ENV CC=mpicc CXX=mpic++
