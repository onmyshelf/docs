# OnMyShelf Administration Guide

**Note**: This documentation is not complete yet. More to come!

## Installation
The easiest way to install OnMyShelf is to use the [docker project here](https://github.com/onmyshelf/docker).

If you want to install the API manually, here are the instructions:

### Requirements
- A MariaDB (>10.3) database (should also work with a recent MySQL server)
- A web server with rewrite module enabled, PHP 8.0+ and the following PHP modules:
    - exif
    - gd
    - pdo
    - pdo_mysql
    - zip

[See this file](https://github.com/onmyshelf/docker/blob/master/api/Dockerfile) to help you find the good PHP extensions.

### Configuration
Copy `config.default.php` to `config.php` then edit it.

### Initialization
Go into the project folder then run:
```bash
php bin/oms install
```

## Upgrade
If you uses the docker project, you have nothing to do.

If you have installed the API manually, go into the project folder then run:
```bash
php bin/oms upgrade
```

## Logs
A file named `onmyshelf.log` is stored at the root of the project.
You can change the path of the log file and logs verbosity into:

- `.env` if using docker
- API's `config.php` if installed manually
