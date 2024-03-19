FROM python:3.10.13-slim-bookworm

RUN mkdir code

WORKDIR code

ADD . /code/
ADD .env.docker /code/.env

ENV APP_NAME=DOCKER_DEMO_CONFIG

RUN pip install -r requirements.txt

CMD gunicorn docker_demo_config.wsqi:applecation -b 0.0.0.0:8000