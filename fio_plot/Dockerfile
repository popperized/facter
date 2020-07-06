FROM python:3.7.8-slim

ADD . /

WORKDIR /

RUN apt update && \
    apt install -y fio && \
    pip install -r requirements.txt