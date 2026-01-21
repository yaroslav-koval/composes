# Composes

A bunch of useful docker composes for real projects

This repository contains different docker compose files to start:

| Service                                          | Description                                                     |
|--------------------------------------------------|-----------------------------------------------------------------|
| [Postgres](composes/postgres.yml)                | Postgres server with data persistence in a Volume               |
| [MongoDB](composes/mongodb.yml)                  | MongoDB server with data persistence in a Volume                |
| [Redis](composes/redis.yml)                      | Redis server with a replica                                     |
| [Kafka](composes/kafka.yml)                      | Single instance of Kafka + Kafdrop UI                           |
| [Kafka (3 brokers)](composes/kafka.3brokers.yml) | Three instance of Kafka brokers connected by KRaft + Kafdrop UI |
| [Minio (3 nodes)](composes/minio.yml)            | Three instances of Minio (OSS alternative of S3)                |

Single docker-compose file can be run through:

```shell
docker compose -p <project-name> -f <file-name> up -d
```
