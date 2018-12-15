# SonarQube

## Installation

You need to give right user to directories in the volume

```bash
groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
chown sonarqube:sonarqube conf/ data/ extensions/ logs/
```
