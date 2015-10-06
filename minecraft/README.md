# Minecraft

## Versions

* Docker 1.8.2
* Docker Machine
* Docker Compose

## Docker Machine

export OS_USERNAME=your-rackspace-username
export OS_API_KEY=your-rackspace-api-key
export OS_REGION_NAME=IAD

docker-machine create \
  --driver rackspace \
  minecraft
