# Docker infrastructure for Elasticsearch and Kibana

#### TL;DR

  

**- setup and run**

0. Clone repository

  

1. Edit .env

  

2. make init (only the first time)

  

3. make rebuild (if you change something)

  

#### Develop env

**- require**

Docker version: >= 18.09.6

docker-compose version: >= 1.24.0

  

**- make command**

    version: Print version of Docker, Docker Compose, and PHP

    init: Setup application use it the only first time

    build: Build all container of docker-compose file

    up: Up all container of docker-compose file with -d mode

    down: Down all container started

    run: Run container

    rebuild: Re-build and up all container

    exec: Exec bash of the container.
  

[manual push](https://docs.docker.com/engine/reference/commandline/push/) in registry

  

### Features

**Application env**

-Webserver Nginx 1.17-alpine

-Elastisearch 7.6.1 (Official image)

-Kibana 7.6.1 (Official image)

  

### Cautions

  

1. This is a developing environment, elasticsearch (elsearch) is exposed to the public network on port 9200 and 9300.

2. No HTTPS for NGINX.

3. Enable authentication for Kibana and Elasticsearch client.

3. Discourage production deployment without a fix of these issues.

  

## License

  

This project is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)