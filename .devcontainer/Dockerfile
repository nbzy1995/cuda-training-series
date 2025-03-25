# Use an official CUDA base image (adjust the tag as needed)
FROM nvidia/cuda:11.8.0-base-ubuntu20.04

# Avoid interactive prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Update apt and install tools
RUN apt-get update && apt-get install -y \
    build-essential \
    cmake \
    git \
    gdb \
    vim \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /workspace
