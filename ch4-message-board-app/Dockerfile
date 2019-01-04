# Pull base image
FROM python:3.7-slim

# Set environment varibles
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set work directory
WORKDIR /ch4-message-board-app

# Install dependencies
RUN pip install pipenv
COPY ./Pipfile /ch4-message-board-app/Pipfile
RUN pipenv install --system --skip-lock

# Copy project
COPY . /ch4-message-board-app/
