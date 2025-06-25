# Base image with Python 3.11 and Linux tools
FROM mcr.microsoft.com/devcontainers/python:3.11-bookworm

# Install common tools used in SDN scripting and automation
RUN apt-get update && \
    apt-get install -y \
    iputils-ping \
    net-tools \
    curl \
    nano \
    vim \
    ssh \
    && apt-get clean

# Upgrade pip
RUN pip install --upgrade pip

# Create a non-root user for VS Code
ENV DEBIAN_FRONTEND=noninteractive
