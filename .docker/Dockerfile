FROM ubuntu:20.04

RUN apt-get update -y \
    && apt-get install -y --no-install-recommends \
       python3 curl \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# poetry
ENV POETRY_HOME /etc/poetry
RUN curl -sSL https://install.python-poetry.org | python3 - --preview --version 1.2.0b3

ENV PATH /etc/poetry/bin:$PATH
