# redis-docker-compose
A [docker-compose](https://docs.docker.com/compose/) sample to start `Redis` database.


# How to use?

1. Clone the project:

  ```shell
    $ git clone https://github.com/gaoshanyu/redis-docker-compose.git
  ```

2. Start `Redis` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./redis-docker-compose
    $ docker-compose up -d
  ```

3. Connect to the Redis server:

  ```shell
    $ docker exec -ti redis redis-cli -h 127.0.0.1 -p 6379 -a 12345678
  ```
