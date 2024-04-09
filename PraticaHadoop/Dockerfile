FROM ubuntu:latest

WORKDIR /

COPY . .

RUN apt-get update \
 && apt-get install -y openjdk-8-jdk python3 wget
RUN cat bash.txt >> /.bashrc
RUN wget https://dlcdn.apache.org/hadoop/common/hadoop-3.4.0/hadoop-3.4.0.tar.gz \
 && tar xf hadoop-3.4.0.tar.gz \
 && rm hadoop-3.4.0.tar.gz

CMD bash
