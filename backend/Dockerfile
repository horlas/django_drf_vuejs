# Pull base image
FROM python:3.6

ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWRITEBYTECODE 1

#WORKDIR /app

RUN pip install pipenv
ADD Pipfile* /code/
WORKDIR /code
RUN pipenv install --system --ignore-pipfile
COPY scripts/start.sh /
ADD . /code/


