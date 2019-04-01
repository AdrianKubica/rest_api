FROM python:3.7-alpine
LABEL maintainer="adrian.kubica.ak@gmail.com"

ENV PYTHONUNBUFFERED 1
WORKDIR /app

COPY ./requirements.txt ./
RUN pip install -r ./requirements.txt
RUN adduser -D user
USER user

COPY ./app /app
