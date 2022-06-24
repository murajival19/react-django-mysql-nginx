# backend/Dockerfile
# set base image
FROM python:3.10.5

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# set work directory
WORKDIR /backend

# install dependencies
COPY backend/requirements.txt .
RUN python3 -m pip install --upgrade pip setuptools
RUN pip install -r requirements.txt

# Copy project
COPY backend/ .