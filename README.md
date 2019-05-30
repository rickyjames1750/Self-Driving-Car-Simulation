# Self-Driving-Car-Simulation
## This code is a work in progress

Keras is used to train a convolutional neural network on images from the car's cameras as well as steering angles from human driving.

### Overview

This project is based upon Udacity's self driving car simulator as a testbed for training an autonomous car.

### Dependencies

All the necessary dependencies can be installed with the following commands below.
Anaconda is needed to use the environment settings. 

```
[//]: # Use Tensorflow without GPU  
conda env create -f environments.yml
[//]: # Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```
### Usage 
#### Run the pretrained model
Fire up the Udacity self-driving simulator, choose a map and press the Autonomous Mode button. Then, run the model as follows:
```
python drive.py model.h5
```
#### Train the model 
The data folder is needed which contains the training images
```
python model.py
```
This will generate a file model-<epoch>.h5 whenever the performance in the epoch is better than the previous best. For example, the first epoch will generate a file called model-000.h5.
  
#### Credits 
Udacity Self-Driving Car Simulator: https://github.com/udacity/self-driving-car-sim
