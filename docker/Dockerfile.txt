# docker/Dockerfile
# NOTE: Replace this with the actual Dockerfile you used to successfully run the FVP.
FROM ubuntu:22.04

RUN apt-get update && apt-get install -y \
    git make build-essential \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
CMD ["/bin/bash"]