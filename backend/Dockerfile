FROM python:3.11.4-bullseye
WORKDIR /app
COPY requirements.txt .
RUN  pip install --upgrade pip && pip install -r requirements.txt
COPY . ./
CMD gunicorn foodgram.wsgi:application --bind 0.0.0.0:8000