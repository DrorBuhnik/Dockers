FROM drorbuhnik/tensorflow:1.14.0-gpu-py3.7

RUN curl -sSL https://sdk.cloud.google.com | bash 

ENV PATH $PATH:/root/google-cloud-sdk/bin

# opencv require those packages
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        libsm6 \
        libxext6 \
        libxrender-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
