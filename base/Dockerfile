
ARG BASE_CONTAINER=ubuntu:18.04
FROM $BASE_CONTAINER

LABEL maintainer="ByungchanKim <kbc8894@gmail.com>"

ENV LANG C.UTF-8
ARG PYTHON_VERSION=3.7
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && \
    apt install -y --no-install-recommends \
        software-properties-common \
        wget \
        && \
    add-apt-repository ppa:deadsnakes/ppa &&\
    apt update && \
    apt install -y --no-install-recommends \
        python${PYTHON_VERSION} \
        python${PYTHON_VERSION}-dev \
        python3-distutils-extra \
        && \
    wget -O ~/get-pip.py \
        https://bootstrap.pypa.io/get-pip.py && \
    python${PYTHON_VERSION} ~/get-pip.py && \
    ln -s /usr/bin/python${PYTHON_VERSION} /usr/local/bin/python3 && \
    ln -s /usr/bin/python${PYTHON_VERSION} /usr/local/bin/python && \
    python -m pip --no-cache-dir install --upgrade \
        setuptools