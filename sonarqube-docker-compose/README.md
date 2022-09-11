# sonar-docker-compose
A [docker-compose](https://docs.docker.com/compose/) sample to start `Sonar Qube` server.


# How to use?

1. Clone the project:

  ```shell
    $ git clone \
        --depth 1  \
        --filter=blob:none  \
        --sparse \
        https://github.com/ToanP/dockers \
  ```

  ```shell
  cd dockers
  ```

```shell
  git sparse-checkout set sonarqube-docker-compose
  ```
2. Start `Sonar Qube` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./sonarqube-docker-compose
    // Please add path 
    "./sonarqube_data"
    "./sonarqube_extensions"
    "./sonarqube_logs"
    "./postgresql"
    "./postgresql_data" 
    as the sharing folder for your Docker before
    $ docker-compose up -d
  ```

3. Vist http://localhost:9000 with credetial below:
  ```shell
    login: admin
    password: admin
  ```
 

4. Other commands maybe needed:
  ```shell
    # you can stop service by the command
    $ docker stop sonarqube
    # you can start service by the command
    $ docker start sonarqube
    # you can restart service by the command
    $ docker restart sonarqube
  ```
