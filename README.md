### docker compose with redis and node containers

1. tag and build image

```sh
docker build -t dockerusername/projectname .
```

2. run redis

```sh
docker run redis
```

3. run container

```sh
docker run dockerusername/projectname
```

### port mapping

- route incoming requests to port inside container

```sh
  docker run -p LOCAL_HOST_PORT_INCOMING:PORT_INSIDE_CONTAINER <image name>
```

e.g.

```sh
docker run -p 8080:8080 dockerusername/projectname
```

### start containers in the background

```sh
docker-compose up -d
```
