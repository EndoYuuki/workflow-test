FROM ubuntu:20.04

RUN apt-get update -y \
    && apt-get install -y --no-install-recommends \
       python3 python3-pip ca-certificates curl \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# poetry
RUN curl -sSL https://install.python-poetry.org | POETRY_HOME=/etc/poetry python3 - --preview --version 1.2.0b3
ENV PATH /etc/poetry/bin:$PATH
