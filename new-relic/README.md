# GrandChef - App Base Image
Imagem base para criação do container da aplicação.

## Build

Criar imagem base
```sh
docker build -t grandchef/app:2.82.3-new-relic new-relic
```

Roda o shell na imagem criada
```sh
docker run -it --rm grandchef/app:2.82.3-new-relic /bin/bash
```

## Release

Envia imagem para o hub.docker
```sh
docker push grandchef/app:2.82.3-new-relic
```
