# Development Environment for Deep Learning

This repository contains the docker files which are used to construct my development environment.

# Instruction

To build these these images, please run the following commands in the project root:

```
docker build -t senbong/lasagne:base -f lasagne/Dockerfile lasagne
docker build -t senbong/tensorflow:base -f tensorflow/Dockerfile tensorflow
```

To run the image:

```
nvidia-docker run --rm -it --volume <host-workspace>:/root/Workspace senbong/<image-name>:base /bin/bash
```

# Dependency

* [Docker](https://www.docker.com/)
* [Nvidia Docker](https://github.com/NVIDIA/nvidia-docker)
