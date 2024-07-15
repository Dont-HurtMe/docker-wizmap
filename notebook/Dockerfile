FROM python:3.12-slim

RUN apt-get update --fix-missing
RUN apt install -y git gcc g++

RUN pip install jupyter
WORKDIR /jupyter

COPY ./requirements.txt requirements.txt
RUN pip install -r requirements.txt

ADD . /jupyter/
WORKDIR /jupyter