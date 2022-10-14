
# Diffusion Model


This repository focuses on Diffusion Models: A generative modelling approach. 
All the code is taken from various repositories with power of wandb and docker


## Methodology

![Understanding Diffusion Models : A Unified Perspective](https://arxiv.org/abs/2208.11970)


## Tech Stack

[![Pytorch](https://img.shields.io/badge/Framework-PyTorch-orange.svg)](https://pytorch.org/)

[![Python](https://img.shields.io/badge/Language-Python-green.svg)](https://python.org/)

[![WandB](https://img.shields.io/badge/Visual-WandB-yellowgreen.svg)](https://wandb.ai/)

[![Docker](https://img.shields.io/badge/Virtual-Docker-blue.svg)](https://www.docker.com/)

- All the libraries used can be found in the requirements file 
## Datasets

- [CIFAR10/100](https://www.cs.toronto.edu/~kriz/cifar.html)


## Docker Run

### Docker Build
`sudo time docker build -f Dockerfile_train -t diffusion .`

### Docker Run
`wandb docker run --gpus 1 -v /local_path/cifar10: /src/cifar10 -ti diffusion /bin/bash -c "cd ../src && source activate diffusionModel && python diffusionModel.py"`




## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`pip install -r requirements.txt`


## Run Locally


`$ python diffusionModel.py`

