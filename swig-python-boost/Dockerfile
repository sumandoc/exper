FROM debian:sid
ENV LANG=C.UTF-8 \
    LC_ALL=C.UTF-8

RUN apt-get update \
    && apt-get install -y g++ make swig libboost-python-dev python3-pip \
    && rm -rf /var/lib/apt/lists/* && pip3 install cython pybind11 ipython
  
CMD ["ipython"]
