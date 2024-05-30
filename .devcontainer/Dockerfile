FROM mcr.microsoft.com/devcontainers/python:1-3.10-bullseye

ENV PYTHONUNBUFFERED 1

WORKDIR /hello

# [Optional] If your requirements rarely change, uncomment this section to add them to the image. 
COPY requirements.txt ./
RUN pip3 --disable-pip-version-check --no-cache-dir install -r requirements.txt 

COPY  ./ ./

# [Optional] Uncomment this section to install additional OS packages.
# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>

RUN  apt update && apt upgrade -y && apt install -y python3-pyqt5 
RUN  pip install pandas



