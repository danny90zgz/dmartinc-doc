# Kafka

* Based on **openjdk:8**
* Gets http://apache.uvigo.es/kafka/2.1.0/kafka_2.11-2.1.0.tgz
* Executes kafka-server-start.sh

## Build image
```bash
docker build -t kafka .
```

## Run container
```bash
docker run --name kafka -p 9092:9092 --add-host zookeeper:$HOST_IP kafka
```