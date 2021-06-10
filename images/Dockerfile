FROM ubuntu:20.04

LABEL description = "Imagen para web.py SLC"
LABEL mainteiner = "Fernando HV"
LABEL version = "0.1"

ENV requirements /home/requirements.txt

COPY requirements.txt ${requirements}

RUN apt update
RUN apt install -y python3
RUN apt install -y python3-pip
RUN apt install -y sqlite3

RUN pip3 install -r ${requirements}

RUN apt-get upgrade -y