FROM python:3.8-slim

RUN apt-get update && apt-get install unzip -y

WORKDIR /usr/src/app

COPY app.zip .
RUN unzip app.zip
RUN pip install Flask
RUN pip install mysql-connector-python

EXPOSE 5000

CMD ["python", "app.py"]
