FROM python:3.6 AS base
ENV PIP_NO_CACHE_DIR off
ENV PYTHONPATH="/app:${PYTHONPATH}";
RUN pip3 install pipenv==2018.5.18

WORKDIR /app

COPY Pipfile .
COPY Pipfile.lock .

RUN pipenv install --system --dev
