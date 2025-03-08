# Use an official Python runtime as a parent image. We'll use the slim version to keep the image smaller.
FROM python:3.8-slim-buster

WORKDIR /app

COPY requirements.txt requirements.txt

RUN pip install --upgrade pip
RUN pip install -r requirements.txt


COPY . .

EXPOSE 8000

CMD python manage.py runserver