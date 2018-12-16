# SonarQube docker-compose

[Using SonarQube Docker Image](https://github.com/SonarSource/docker-sonarqube)

## Installation

You need to give right user to directories in the volume

```bash
groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
chown sonarqube:sonarqube conf/ data/ extensions/ logs/
```

Create the `.env` file from [.env.dist](.env.dist) example with the
environment variables from [docker let's encrypt nginx proxy](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion/wiki/Basic-usage)

```bash
docker-compose up -d
```

## Update docker images

```bash
./updateDockerImages.sh
```
