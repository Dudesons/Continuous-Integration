FROM ubuntu:16.04

RUN apt update && \
    apt install -y libfreetype6-dev \
                   python-dev \
                   pkg-config \
                   libpng-dev \
                   libffi-dev \
                   curl && \
    curl https://bootstrap.pypa.io/get-pip.py | python

ADD app /app

WORKDIR /app

RUN pip install -r requirements.txt -r test_requirements.txt
