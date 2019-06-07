FROM python:3
ENV PYTHONBUFFERED 1
RUN mkdir /code
WORKDIR /code
COPY requirements.txt /code/
RUN apt-get update
RUN apt-get install python3-dev default-libmysqlclient-dev  -y
RUN pip install -r requirements.txt
COPY ./app/ /code/
