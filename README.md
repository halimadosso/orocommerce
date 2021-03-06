# OROCommerce Docker Image
The docker image contains source code of OROCommerce application.
This image are used as part of docker stack (see compose configs).

## Requirements

1. [Docker](https://www.docker.com/)
2. [Docker Compose](http://docs.docker.com/compose)

## Usage
**OROCommerce stack with web installation**

For more information [see compose config](./compose/webinstall/docker-compose.yml)

Run stack 

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/orocommerce/master/compose/webinstall/docker-compose.yml) up
```
Navigate to [http://localhost:3080](http://localhost:3080) in your web browser, and install application via web wizard

Stop stack

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/orocommerce/master/compose/webinstall/docker-compose.yml) stop
```

**OROCommerce stack with automated installation**

For more information [see compose config](./compose/autoinstall/docker-compose.yml)

default login: `admin` default password: `admin1111`

Run stack

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/orocommerce/master/compose/autoinstall/docker-compose.yml) up
```
Navigate to [http://localhost:3080](http://localhost:3080) in your web browser, and login

Stop stack

```
docker-compose -f <(curl https://raw.githubusercontent.com/djocker/orocommerce/master/compose/autoinstall/docker-compose.yml) stop 
```

## Docker Cloud

Also you can use stack files from [stackfile.io](https://stackfiles.io/registry/56fc345c416a1001004d39cc) to deploy via [cloud.docker.com](https://cloud.docker.com)
