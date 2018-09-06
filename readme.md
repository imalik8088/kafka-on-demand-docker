# Kafka on demand cluster with Docker

## Prerequisite

    * docker
    * docker-compose version at lease 1.5

## Getting started

Start with the setup that you want to have on your machine

```bash
docker-compose -f kafka.yml up

```
#### Whats included in the compose files

| file                | included                                                        | Port used                    |
|---------------------|-----------------------------------------------------------------|------------------------------|
| kafka.yml           | Zookeeper and Kafka                                             | 2181, 9092                   |
| confluent-stack.yml | Zookeeper, Kafka, Schema-Registry, Rest-Proxy and Kafka-Connect | 2181, 9092, 8081, 8082, 8083 |
| web-ui.yml          | Topics UI, Schema-Registry UI and Kafka-Connect UI              | 8001, 8002, 8003             |

## Confluent Versions

versions that can be set in the `.env` to start the setup that you need. Here some of the example tags and version for full disclosure the [confluent versions page][1]

| Confluent Platform | Kafka Version |
|--------------------|---------------|
| 5.0.0-1            | 2.0.x         |
| 4.1.1              | 1.1.x         |
| 4.0.2-2            | 1.0.x         |







[1]: https://docs.confluent.io/current/installation/versions-interoperability.html#cp-versions

