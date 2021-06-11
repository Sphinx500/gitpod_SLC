FROM ubuntu:20.04

LABEL description = "Imagen para web.py SLC"
LABEL mainteiner = "Fernando HV"
LABEL version = "0.1"

RUN apt-get update

RUN apt-get install -y python3
RUN apt-get install -y python3-pip
RUN apt-get install -y sqlite3

# Define ENV files
ENV requirements images/requirements.txt

# Copy requirements file
COPY requirements.txt ${requirements}

# Install python packages
RUN pip3 install -r images/requirements.txt