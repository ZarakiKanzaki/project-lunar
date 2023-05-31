ARG VARIANT=0-1-bullseye
FROM mcr.microsoft.com/devcontainers/rust:${VARIANT}

#install libasound2-dev for alsa-sys
RUN apt-get update && apt-get -y install --no-install-recommends libasound2-dev \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*