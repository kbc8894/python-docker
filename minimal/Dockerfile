
ARG BASE_CONTAINER=kbc8894/python:deadsnakes-3.7
FROM $BASE_CONTAINER

LABEL maintainer="ByungchanKim <kbc8894@gmail.com>"
RUN python -m pip --no-cache-dir install --upgrade \
    numpy \
    scipy \
    pandas \
    cloudpickle \
    scikit-image \
    scikit-learn \
    matplotlib \
    Cython