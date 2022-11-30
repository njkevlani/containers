# Kafka setup

## Usage

### To start
```shell
podman-compose up
```

This will start
- zookeeper.
- kafka (port=9092). Applications from localhost can connect `localhost:9092`.
- [redpanda-console](https://github.com/redpanda-data/console) (port=9093). You can open `localhost:9093` in your browser.

### To stop
```shell
podman-compose down
```

### To clear data
```shell
podman volume rm kafka_kafka_data
podman volume rm kafka_zookeeper_data
```
