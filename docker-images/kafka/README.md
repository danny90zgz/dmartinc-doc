# Kafka

## Build image
```bash
docker build -t kafka .
```

## Run container
```bash
docker run --name kafka -p 9092:9092 --add-host zookeeper:$HOST_IP kafka
```