# Upgrade

## Upgrade using docker
If you uses the docker project, read the upgrade section in the [documentation here](https://github.com/onmyshelf/docker#upgrade).

## Upgrade manually
If you have installed the API and web interface manually:

1. Pull the last modifications of the API from the git repository.
2. Go into the project folder then run:
```bash
php bin/oms upgrade
```
3. Pull the last modifications of the Web interface, build and deploy files.