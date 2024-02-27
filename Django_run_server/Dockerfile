FROM python:3.12.2-slim

RUN mkdir code

WORKDIR code

ADD . /code/
ADD .env.docker /code/.env

ENV APP_NAME=DOCKER_DEMO_CONFIG

RUN pip install -r requirements.txt

CMD gunicorn docker_demo_config.wsqi:applecation -b 0.0.0.0:8000
