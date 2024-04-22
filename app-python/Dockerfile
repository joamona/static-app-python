# pull official base image
FROM python:3.12-alpine

# set work directory
WORKDIR /usr/src/app

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# install psycopg2 dependencies
#pango es una dependencia de weasyprint
RUN apk update 
# install dependencies
RUN pip install --upgrade pip


COPY ./requirements.txt .

RUN pip3 install -r requirements.txt

# copy project
COPY . .

