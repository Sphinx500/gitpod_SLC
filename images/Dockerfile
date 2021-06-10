FROM ubuntu:20.04

LABEL description = "Imagen para web.py SLC"
LABEL mainteiner = "Fernando HV"
LABEL version = "0.1"

ENV requirements /app/requirements.txt

COPY requirements.txt ${requirements}

apt update
apt install -y python3
apt install -y python3-pip


