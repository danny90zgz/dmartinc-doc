# Zookeeper

* Based on **openjdk:8**
* Gets http://apache.uvigo.es/kafka/2.1.0/kafka_2.11-2.1.0.tgz
* Executes zookeeper-server-start.sh

## Build image
```bash
docker build -t zookeeper .
```

## Run container
```bash
docker run --name zookeeper -p 2181:2181 zookeeper
```