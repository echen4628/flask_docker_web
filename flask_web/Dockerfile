FROM ubuntu:22.04

MAINTAINER Eric Chen "echen4628@gmail.com"

RUN apt-get clean -y && \
apt-get update -y && \
apt-get install -y python3-pip python3-dev

COPY ./requirements.txt /app/requirements.txt

WORKDIR /app

RUN pip3 install -r requirements.txt

COPY . /app

ENTRYPOINT [ "python3" ]

CMD [ "app.py" ]
