This guide teaches you how to setup a ROS2 environment in Docker for learning and testing ROS.

## Docker Installation

Visit [docker installation](https://www.docker.com/), to install appropriate Docker desktop for your OS. Once installed, start the docker runtime by starting the docker desktop.

## Setting up ROS

run `docker pull osrf/ros:humble-desktop` to get the ROS humbe image, and to start a container using the image, run `docker run -it --rm osrf/ros:humble-desktop` this will start an interactive terminal running the container.
