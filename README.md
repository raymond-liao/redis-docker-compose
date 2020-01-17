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

4. Other commands maybe needed:
  ```shell
    # you can stop service by the command
    $ docker stop redis
    # you can start service by the command
    # maybe you need this command after your computer restart
    $ docker start redis
    # you can restart service by the command
    # maybe you need this command after you made some update for [redis.conf]
    $ docker restart redis
  ```

# Q&A
1. How to change password?
  * Just change the line `requirepass 12345678` in file `redis.conf` to `requirepass [new password]`, and then restart the service with command `docker restart redis`
