
ARG BASE_CONTAINER=kbc8894/python:deadsnakes-3.7-minimal
FROM $BASE_CONTAINER

LABEL maintainer="ByungchanKim <kbc8894@gmail.com>"
RUN python -m pip --no-cache-dir install --upgrade \
    torch==1.7.1+cpu \
    torchvision==0.8.2+cpu \
    torchaudio==0.7.2 \
    -f https://download.pytorch.org/whl/torch_stable.html