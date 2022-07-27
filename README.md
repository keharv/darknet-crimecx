<p align="center">
  <img src="http://pjreddie.com/media/files/darknet-black-small.png">
</p>

# Darknet #
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

# Crime.CX #
[Crime.CX](https://crime.cx/) aims to be the largest repository of cat images in the world. This fork of Darknet has been modified for this purpose.

# Setup #
```
gh repo clone keharv/darknet 
cd darknet
make
mkdir images
mkdir cats
```
NOTE: YOU MUST HAVE CUDA REQUIREMENTS INSTALLED, OTHERWISE CHANGE GPU=0 IN Makefile 


# Usage #
First, put images to test in ./images/
```
wget https://pjreddie.com/media/files/yolov3.weights
./crimecx cfg/yolov3.cfg yolov3.weights
```
Images containing cats will be copied into ./cats/
