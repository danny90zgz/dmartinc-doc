FROM openjdk:8

RUN wget http://apache.uvigo.es/kafka/2.1.0/kafka_2.11-2.1.0.tgz

RUN tar -xzf kafka_2.11-2.1.0.tgz

RUN rm kafka_2.11-2.1.0.tgz

ADD config /kafka_2.11-2.1.0/config

CMD ["/kafka_2.11-2.1.0/bin/kafka-server-start.sh", "/kafka_2.11-2.1.0/config/server.properties"]