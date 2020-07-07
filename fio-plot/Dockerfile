FROM python:3.7.8-slim

ENV DEBIAN_FRONTEND=noninteractive
ARG VERSION=3.12-2

ADD . /

WORKDIR /

RUN apt update && \
    apt install -y --no-install-recommends fio=${VERSION} && \
    pip install -r requirements.txt && \
    rm -rf /var/lib/apt/lists/* && \
    ln -s /bench_fio /usr/local/bin/bench_fio && \
    ln -s /fio_plot /usr/local/bin/fio_plot
