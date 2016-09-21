FROM nvidia/cuda:7.5-cudnn5-devel

MAINTAINER senbong <senbong87@gmail.com>

RUN apt-get update && \
    apt-get install -y python-pip python-dev libatlas-base-dev gfortran && \
    apt-get clean && \
    pip install theano lasagne && \
    printf "[global]\nfloatX = float32\ndevice = gpu0\n" > /root/.theanorc
