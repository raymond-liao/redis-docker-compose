# redis-docker-compose
A docker-compose sample to start redis.


# How to use?

1. Start `Redis` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    docker-compose up -d
  ```

2. Connect to the Redis server:

  ```shell
    docker exec -ti redis redis-cli -h 127.0.0.1 -p 6379 -a 12345678
  ```
