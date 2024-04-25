FROM python:3.9-alpine

WORKDIR /app

ENV PYTHONUNBUFFERED=1

COPY requirements.txt .
RUN pip install gunicorn
RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000
EXPOSE 9000