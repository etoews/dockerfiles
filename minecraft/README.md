# Minecraft

## Versions

* Docker 1.8.2
* Docker Machine 0.4.1
* Docker Compose 1.4.0

## Docker Machine

```bash
export OS_USERNAME=your-rackspace-username
export OS_API_KEY=your-rackspace-api-key
export OS_REGION_NAME=IAD

docker-machine create \
  --driver rackspace \
  minecraft

docker-machine ssh minecraft \
  "wget -q https://raw.githubusercontent.com/everett-toews/dockerfiles/master/script/secure"
docker-machine ssh minecraft \
  "chmod u+x secure"
docker-machine ssh minecraft \
  "./secure 25565"

eval "$(docker-machine env minecraft)"
```

## Docker Compose

```bash
docker-compose up
```
