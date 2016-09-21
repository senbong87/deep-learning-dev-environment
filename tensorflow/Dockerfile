FROM nvidia/cuda:7.5-cudnn5-devel

MAINTAINER senbong <senbong87@gmail.com>

RUN apt-get update && \
    apt-get install -y python-pip python-dev python-pil libatlas-base-dev gfortran && \
    apt-get clean && \
    pip install --upgrade pip && \
    pip install numpy scipy && \
    pip install https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow-0.10.0-cp27-none-linux_x86_64.whl
