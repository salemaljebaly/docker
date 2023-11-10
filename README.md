# Installing docker compose on arm64
# 
```
DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
mkdir -p $DOCKER_CONFIG/cli-plugins
```
## 32-bit (armv7) operating system:
```
curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-armv7 -o $DOCKER_CONFIG/cli-plugins/docker-compose
```
## 64-bit (aarch64) operating system:
```
curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-aarch64 -o $DOCKER_CONFIG/cli-plugins/docker-compose
```
## Make the binary executable:
```
chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose
```