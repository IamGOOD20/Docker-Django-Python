# Pull base image
FROM python:3.12.2-slim

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set work directory
WORKDIR /code

# Copy project
COPY . /code/

# Install dependencies
#COPY Pipfile Pipfile.lock /code/
#RUN pip install pipenv && pipenv install --system
RUN pip install -r requirements.txt
