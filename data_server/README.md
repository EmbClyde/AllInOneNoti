# Data Server

## Kafka << 메시징 큐

- Version : 3.2.1
- Dependency : Java 8 or Newer releases

## Kafka 운영 커맨드

```sh
# Must build kafka project first
$ ./gradlew jar -PscalaVersion=2.13.6

# Start Zookeeper service << Soon, Zookeeper will no longer be required by Apache Kafka
$ bin/zookeer-server-start.sh config/zookeeper.properties

# Start Kafka Broker service << Real Program for message streaming
$ bin/kafka-server-start.sh config/server.properties
```

## Kafka 설정

`config` 폴더 내의 `server.properties`를 수정하여 Kafka의 동작설정을 할 수 있다.
