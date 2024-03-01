#FROM python:3.10.13-slim-bookworm

#WORKDIR / code

#RUN pip install -r requirements.txt

# Pull base image
FROM python:3.10.13-slim-bookworm

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set work directory
WORKDIR /code

# Install dependencies
#COPY Pipfile Pipfile.lock /code/
RUN pip install -r requirements.txt
#RUN pip install pipenv && pipenv install --system

# Copy project
COPY . /code/
