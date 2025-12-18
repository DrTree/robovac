# syntax=docker/dockerfile:1

ARG VARIANT="3.13-bullseye"
FROM mcr.microsoft.com/devcontainers/python:${VARIANT}

# Install common build tooling used by Home Assistant deps.
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y --no-install-recommends \
        build-essential \
        python3-dev \
    && rm -rf /var/lib/apt/lists/*
