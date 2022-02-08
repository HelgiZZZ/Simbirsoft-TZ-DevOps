FROM ubuntu:18.04

RUN mkdir /var/src

WORKDIR /var/

COPY . .

RUN apt-get update -yq && \
    apt-get install -yq git && \
    apt-get install -yq python-pip

RUN cd /var/src/ && \
    pip install -r requirements.txt

CMD cd /var/src/ && python app.py

EXPOSE 5000
