Step-by-Step Procedure:

1. Install Docker
   For Windows: Download Docker Desktop from https://www.docker.com/products/docker-desktop
   Install and launch Docker Desktop

   For Ubuntu/Linux:
   sudo apt update
   sudo apt install docker.io
   sudo systemctl start docker
   sudo systemctl enable docker

2. Verify Docker Installation
   docker --version
   Output should show the Docker version installed.

3. Pull a Base Docker Image
   To pull a basic image (for example, Ubuntu): docker pull ubuntu

   <!-- Or for NVIDIA GPU support (if GPU is available and NVIDIA drivers are installed):
   docker pull nvidia/cuda:12.2.0-base -->

4. Run a Docker Container
   For normal container: docker run -it ubuntu

   <!-- For NVIDIA Docker (with GPU support): First, install NVIDIA Container Toolkit:
   sudo apt install -y nvidia-container-toolkit
   sudo systemctl restart docker
   Then, run the container:
   docker run --gpus all -it nvidia/cuda:12.2.0-base /bin/bash -->

5. Create a file named Dockerfile:
   Dockerfile

   # Use Ubuntu as base image

   FROM ubuntu:latest

   # Install packages

   RUN apt update && apt install -y python3

   # Set working directory

   WORKDIR /app

   # Copy files to container

   COPY . /app

   # Run a command

   CMD ["python3"]

6. Build and run the container:
   docker build -t mycontainer .
   docker run -it mycontainer
