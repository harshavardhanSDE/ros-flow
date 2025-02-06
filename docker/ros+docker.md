This guide teaches you how to setup a ROS2 environment in Docker for learning and testing ROS.

## Docker Installation

Visit [docker installation](https://www.docker.com/), to install appropriate Docker desktop for your OS. Once installed, start the docker runtime by starting the docker desktop.

## Setting up ROS

run `docker pull osrf/ros:humble-desktop` to get the ROS humbe image, and to start a container using the image, run `docker run -it --rm osrf/ros:humble-desktop` this will start an interactive terminal running the container.

changes made.

## Docker manual installation: BASH script

```

# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```
